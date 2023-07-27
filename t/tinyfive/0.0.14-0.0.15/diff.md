# Comparing `tmp/tinyfive-0.0.14.tar.gz` & `tmp/tinyfive-0.0.15.tar.gz`

## Comparing `tinyfive-0.0.14.tar` & `tinyfive-0.0.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-0.0.14/tinyfive/__init__.py
--rw-r--r--   0        0        0    32325 2020-02-02 00:00:00.000000 tinyfive-0.0.14/tinyfive/machine.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-0.0.14/LICENSE
--rw-r--r--   0        0        0    27375 2020-02-02 00:00:00.000000 tinyfive-0.0.14/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 tinyfive-0.0.14/pyproject.toml
--rw-r--r--   0        0        0    27975 2020-02-02 00:00:00.000000 tinyfive-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-0.0.15/tinyfive/__init__.py
+-rw-r--r--   0        0        0    32329 2020-02-02 00:00:00.000000 tinyfive-0.0.15/tinyfive/machine.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-0.0.15/LICENSE
+-rw-r--r--   0        0        0    28769 2020-02-02 00:00:00.000000 tinyfive-0.0.15/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 tinyfive-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0    29369 2020-02-02 00:00:00.000000 tinyfive-0.0.15/PKG-INFO
```

### Comparing `tinyfive-0.0.14/tinyfive/machine.py` & `tinyfive-0.0.15/tinyfive/machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #   - Part II implements encoding and decoding functions around the instructions
 #     defined in part I.
 # Part I is sufficient for emulating RISC-V. Part II is only needed if you want
 # to emulate the instruction encoding of RISC-V.
 
 class machine:
   def __init__(s, mem_size):  # for brevity we use 's' instead of 'self'
-    """create state of CPU: memory, register file 'x[]', program counter 'pc'"""
+    """create state of CPU: memory mem[], regfiles x[] and f[], program counter 'pc'"""
     s.mem = np.zeros(mem_size, dtype=np.uint8)  # memory 'mem[]' is unsigned int8
     s.x   = np.zeros(32, dtype=np.int32)        # regfile 'x[]' is signed int32
     s.f   = np.zeros(32, dtype=np.float32)      # regfile 'f[]' for F-extension
     s.pc  = np.zeros(1, dtype=np.uint32)        # program counter (PC) is uint32
     s.label_dict = {}  # label dictionary (for assembly-code labels)
 
     # performance counters: ops-counters, regfile-usage
@@ -25,18 +25,18 @@
 
   #-------------------------------------------------------------------------------
   # Part I
   #-------------------------------------------------------------------------------
   def i8(s,x): return np.int8(x)    # convert to 8-bit signed
   def u (s,x): return np.uint32(x)  # convert to 32-bit unsigned
 
-  def ipc(s):
-    """increment pc by 4 and make sure that x[0] is always 0"""
+  def ipc(s, incr=4):
+    """increment pc by 'incr' and make sure that x[0] is always 0"""
     s.x[0] = 0
-    s.pc += 4
+    s.pc += incr
 
   #-------------------------------------------------------------------------------
   # Base instructions (RV32I)
 
   # arithmetic
   def ADD (s,rd,rs1,rs2): s.x[rd] = s.x[rs1] + s.x[rs2]; s.ipc()
   def ADDI(s,rd,rs1,imm): s.x[rd] = s.x[rs1] + imm;      s.ipc()
@@ -62,23 +62,23 @@
   # set to 1 if less than
   def SLT  (s,rd,rs1,rs2): s.x[rd] = 1 if s.x[rs1]      < s.x[rs2]      else 0; s.ipc()
   def SLTI (s,rd,rs1,imm): s.x[rd] = 1 if s.x[rs1]      < imm           else 0; s.ipc()
   def SLTU (s,rd,rs1,rs2): s.x[rd] = 1 if s.u(s.x[rs1]) < s.u(s.x[rs2]) else 0; s.ipc()
   def SLTIU(s,rd,rs1,imm): s.x[rd] = 1 if s.u(s.x[rs1]) < s.u(imm)      else 0; s.ipc()
 
   # branch
-  def BEQ (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      == s.x[rs2]      else 4
-  def BNE (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      != s.x[rs2]      else 4
-  def BLT (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      <  s.x[rs2]      else 4
-  def BGE (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      >= s.x[rs2]      else 4
-  def BLTU(s,rs1,rs2,imm): s.pc += imm if s.u(s.x[rs1]) <  s.u(s.x[rs2]) else 4
-  def BGEU(s,rs1,rs2,imm): s.pc += imm if s.u(s.x[rs1]) >= s.u(s.x[rs2]) else 4
+  def BEQ (s,rs1,rs2,imm): s.ipc(imm if s.x[rs1]      == s.x[rs2]      else 4)
+  def BNE (s,rs1,rs2,imm): s.ipc(imm if s.x[rs1]      != s.x[rs2]      else 4)
+  def BLT (s,rs1,rs2,imm): s.ipc(imm if s.x[rs1]      <  s.x[rs2]      else 4)
+  def BGE (s,rs1,rs2,imm): s.ipc(imm if s.x[rs1]      >= s.x[rs2]      else 4)
+  def BLTU(s,rs1,rs2,imm): s.ipc(imm if s.u(s.x[rs1]) <  s.u(s.x[rs2]) else 4)
+  def BGEU(s,rs1,rs2,imm): s.ipc(imm if s.u(s.x[rs1]) >= s.u(s.x[rs2]) else 4)
 
   # jump
-  def JAL (s,rd,imm): s.x[rd] = s.pc + 4; s.pc += imm; s.x[0] = 0
+  def JAL (s,rd,imm): s.x[rd] = s.pc + 4; s.ipc(imm)
   def JALR(s,rd,rs1,imm): t = s.pc + 4; s.pc = (s.x[rs1] + imm) & ~1; s.x[rd] = t; s.x[0] = 0
 
   # load immediate
   def LUI  (s,rd,imm): s.x[rd] = imm << 12;          s.ipc()
   def AUIPC(s,rd,imm): s.x[rd] = s.pc + (imm << 12); s.ipc()
 
   # load, note the different argument order, example: 'lb rd, offset(rs1)'
```

### Comparing `tinyfive-0.0.14/LICENSE` & `tinyfive-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfive-0.0.14/README.md` & `tinyfive-0.0.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # TinyFive
 
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20"> </a>
 [![Downloads](https://static.pepy.tech/badge/tinyfive)](https://pepy.tech/project/tinyfive)
+
+<!--- view counter is currently commented out
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FOpenMachine-ai%2Ftinyfive&title_bg=%23555555&icon=&title=views+%28today+%2F+total%29&edge_flat=false)](https://hits.seeyoufarm.com)
+ --->
 
 TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python:
-- It's useful for running neural networks on RISC-V: Simulate your RISC-V assembly code along with your neural network in Python (and without relying on RISC-V toolchains). Custom instructions can be easily added.
-- TinyFive is also useful for ML scientists who are using ML/RL for compiler optimization (see e.g. [CompilerGym](https://github.com/facebookresearch/CompilerGym/blob/development/README.md)).
-- If you want to learn how RISC-V works, TinyFive lets you play with instructions and assembly code.
+- Useful for running neural networks on RISC-V: Simulate your RISC-V assembly code along with a neural network in Keras or PyTorch (and without relying on RISC-V toolchains).
+- Custom instructions can be added for easy HW/SW codesign in Python (without C++ and compiler toolchains).
+- If you want to learn how RISC-V works, TinyFive lets you play with instructions and assembly code in [this colab](https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb).
+- TinyFive might also be useful for ML scientists who are using ML/RL for compiler optimizations (see e.g. [CompilerGym](https://github.com/facebookresearch/CompilerGym/blob/development/README.md)) or to replace compiler toolchains by AI.
 - Can be very fast if you only use the upper-case instructions defined in the [first ~200 lines of machine.py](machine.py#L1-L200).
 - [Fewer than 1000 lines](machine.py) of code (w/o tests and examples)
 - Uses NumPy for math
 
 ## Contents
 - [Installation](#installation)
 - [Usage](#usage)
   - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers)
   - [Example 2: Add two vectors](#example-2-add-two-vectors)
   - [Example 3: Multiply two matrices](#example-3-multiply-two-matrices)
   - [Example 4: Neural network layers](#example-4-neural-network-layers)
+  - [Example 5: MobileNet](#example-5-mobilenet)
 - [Running in colab](#running-in-colab)
 - [Running without package](#running-without-package)
-- [Speed](#speed)
+- [Contribute](#contribute)
 - [Latest status](#latest-status)
+- [Speed](#speed)
 - [Comparison](#comparison)
 - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise)
 
 ## Installation
 ```
 pip install tinyfive
@@ -373,23 +379,28 @@
 ref = np.matmul(A, B)            # golden reference
 print(np.array_equal(res, ref))  # should return 'True'
 # Output: True
 ```
 The table below shows a speedup of 1.7 with the following caveats:
 - The bit-widths don't make sense for fixed point (in general, multiplying two 32-bit integers produces a 64-bit product; and adding 4 of these products requires up to 66 bits).
 - For runtime calculations, we assume that our RISC-V CPU can only perform one instruction per cycle (while many RISC-V cores can perform multiple instructions per cycle).
+- We assume all 31 registers can be used, which is unrealistic because we ignore register allocation conventions such as the procedure
+calling conventions specified [here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc).
 - For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
 ### Example 4: Neural network layers
-Coming soon, see [file layer_examples.py](layer_examples.py)
+Coming soon, see [file layer_examples.py](layer_examples.py) for now
+
+### Example 5: MobileNet
+Coming soon-ish, see [file mobilenet_v1_0.25.py](mobilenet_v1_0.25.py) for now
 
 ## Running in colab
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20">
 </a>  This is the quickest way to get started and should work on any machine.
 
 If you have a free Google Drive account, you can make a copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
@@ -427,26 +438,30 @@
 
 # run examples
 !python3 examples.py
 
 # run test suite
 !python3 tests.py
 ```
+## Contribute
+If you like this project, give it a ⭐ and share it with friends!  And if you are interested in helping make TinyFive better,
+I highly welcome you to do so. I thank you in advance for your interest.  If you are unsure of what you could do to improve the project, you may have a look [here](https://github.com/OpenMachine-ai/tinyfive/issues/5).
+
+## Latest status
+- TinyFive is still under construction, many things haven't been implemented and tested yet.
+- 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
+- Remaining work: improve testing, add more extensions. See TODOs in the code for more details.
+- Stay updated by following us on [Twitter](https://twitter.com/OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn](https://www.linkedin.com/in/nilsgraef/).
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
 - You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
-## Latest status
-- TinyFive is still under construction, many things haven't been implemented and tested yet.
-- 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
-- Remaining work: improve testing, add perhaps more extensions. See TODOs in the code for more details.
-
 ## Comparison
 The table below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects.
 
 | ISS | Author | Language | Mature? | Extensions | LOC |
 | --- | ------ | -------- | ------- | ---------- | --- |
 | [TinyFive](https://github.com/OpenMachine-ai/tinyfive)             | OpenMachine          | Python    | No               | I, M, some F  | < 1k |
 | [Pydgin](https://github.com/cornell-brg/pydgin)                    | Cornell University   | Python, C | Last update 2016 | A, D, F, I, M | |
@@ -456,23 +471,24 @@
 | [riscvOVPsim](https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas              | C         | Yes              | All           | |
 | [Whisper](https://github.com/chipsalliance/SweRV-ISS)              | Western Digital      | C, C++    | Yes | Almost all                 | |
 | [Sail Model](https://github.com/riscv/sail-riscv)                  | Cambridge, Edinburgh | Sail, C   | Yes | All                        | |
 | [PiMaker/rvc](https://github.com/PiMaker/rvc)                      | PiMaker              | C         |     |                            | |
 | [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)             | Charles Lohr         | C         |     | A, I, M, Zifencei, Zicsr   | < 1k |
 
 ## References
+- [HuggingFive :raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
 - Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf)
 - See [this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions. See also the [RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf).
-- Book "The RISC-V Reader: An Open Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
+- Book [The RISC-V Reader: An Open Architecture Atlas](https://www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
 other free versions are [available here](http://riscvbook.com).
 - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk)
 - [Online simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for debug
 
 ## Tiny Tech promise
-Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://github.com/karpathy/micrograd), and other “tiny tech” projects, we believe that core technology should be simple and small (in terms of LOC). Therefore, we will make sure that the core of TinyFive (without tests and examples) will always be below 1000 lines.
+Similar to [TinyEMU](https://bellard.org/tinyemu/), [tinygrad](https://github.com/geohot/tinygrad), and other “tiny tech” projects, we believe that core technology should be simple and small (in terms of LOC). Therefore, we will make sure that the core of TinyFive (without tests and examples) will always be below 1000 lines.
 
 Simplicity and size (in terms of number of instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200 pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
 the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf).
 
 <p align="center">
   <img src="https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg">
 </p>
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
 # TinyFive [Colab] [![Downloads](https://static.pepy.tech/badge/tinyfive)]
-(https://pepy.tech/project/tinyfive) [![Hits](https://hits.seeyoufarm.com/api/
-count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FOpenMachine-
-ai%2Ftinyfive&title_bg=%23555555&icon=&title=views+%28today+%2F+total%29&edge_flat=false)]
-(https://hits.seeyoufarm.com) TinyFive is a lightweight RISC-V emulator and
-assembler written entirely in Python: - It's useful for running neural networks
-on RISC-V: Simulate your RISC-V assembly code along with your neural network in
-Python (and without relying on RISC-V toolchains). Custom instructions can be
-easily added. - TinyFive is also useful for ML scientists who are using ML/RL
-for compiler optimization (see e.g. [CompilerGym](https://github.com/
-facebookresearch/CompilerGym/blob/development/README.md)). - If you want to
-learn how RISC-V works, TinyFive lets you play with instructions and assembly
-code. - Can be very fast if you only use the upper-case instructions defined in
-the [first ~200 lines of machine.py](machine.py#L1-L200). - [Fewer than 1000
-lines](machine.py) of code (w/o tests and examples) - Uses NumPy for math ##
-Contents - [Installation](#installation) - [Usage](#usage) - [Example 1:
-Multiply two numbers](#example-1-multiply-two-numbers) - [Example 2: Add two
-vectors](#example-2-add-two-vectors) - [Example 3: Multiply two matrices]
-(#example-3-multiply-two-matrices) - [Example 4: Neural network layers]
-(#example-4-neural-network-layers) - [Running in colab](#running-in-colab) -
-[Running without package](#running-without-package) - [Speed](#speed) - [Latest
-status](#latest-status) - [Comparison](#comparison) - [References](#references)
-- [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip install
-tinyfive ``` ## Usage TinyFive can be used in the following three ways: -
-**Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
+(https://pepy.tech/project/tinyfive)  TinyFive is a lightweight RISC-V emulator
+and assembler written entirely in Python: - Useful for running neural networks
+on RISC-V: Simulate your RISC-V assembly code along with a neural network in
+Keras or PyTorch (and without relying on RISC-V toolchains). - Custom
+instructions can be added for easy HW/SW codesign in Python (without C++ and
+compiler toolchains). - If you want to learn how RISC-V works, TinyFive lets
+you play with instructions and assembly code in [this colab](https://
+colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/
+colab.ipynb). - TinyFive might also be useful for ML scientists who are using
+ML/RL for compiler optimizations (see e.g. [CompilerGym](https://github.com/
+facebookresearch/CompilerGym/blob/development/README.md)) or to replace
+compiler toolchains by AI. - Can be very fast if you only use the upper-case
+instructions defined in the [first ~200 lines of machine.py](machine.py#L1-
+L200). - [Fewer than 1000 lines](machine.py) of code (w/o tests and examples) -
+Uses NumPy for math ## Contents - [Installation](#installation) - [Usage]
+(#usage) - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers) -
+[Example 2: Add two vectors](#example-2-add-two-vectors) - [Example 3: Multiply
+two matrices](#example-3-multiply-two-matrices) - [Example 4: Neural network
+layers](#example-4-neural-network-layers) - [Example 5: MobileNet](#example-5-
+mobilenet) - [Running in colab](#running-in-colab) - [Running without package]
+(#running-without-package) - [Contribute](#contribute) - [Latest status]
+(#latest-status) - [Speed](#speed) - [Comparison](#comparison) - [References]
+(#references) - [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip
+install tinyfive ``` ## Usage TinyFive can be used in the following three ways:
+- **Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
 examples 1.1, 1.2, 2.1, and 3.1 below. - **Option B:** Use `asm()` and `exe()`
 functions without branch instructions, see examples 1.3 and 2.2 below. -
 **Option C:** Use `asm()` and `exe()` functions with branch instructions, see
 example 2.3, 3.2, and 3.3 below. For the examples below, import and instantiate
 a RISC-V machine with at least 4KB of memory as follows: ```python from
 tinyfive.machine import machine m = machine(mem_size=4000) # instantiate RISC-
 V machine with 4KB of memory ``` ### Example 1: Multiply two numbers **Example
@@ -231,103 +232,115 @@
 (4*32, size=4*4).reshape(4, 4) # read result matrix ref = np.matmul(A, B) #
 golden reference print(np.array_equal(res, ref)) # should return 'True' #
 Output: True ``` The table below shows a speedup of 1.7 with the following
 caveats: - The bit-widths don't make sense for fixed point (in general,
 multiplying two 32-bit integers produces a 64-bit product; and adding 4 of
 these products requires up to 66 bits). - For runtime calculations, we assume
 that our RISC-V CPU can only perform one instruction per cycle (while many
-RISC-V cores can perform multiple instructions per cycle). - For 16x16 or
+RISC-V cores can perform multiple instructions per cycle). - We assume all 31
+registers can be used, which is unrealistic because we ignore register
+allocation conventions such as the procedure calling conventions specified
+[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). - For 16x16 or
 larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
 Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
 discovering-novel-algorithms-with-alphatensor) can reduce the total number of
 multiplications and additions if they are applied recursively. | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
 3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
-network layers Coming soon, see [file layer_examples.py](layer_examples.py) ##
-Running in colab [Colab] This is the quickest way to get started and should
-work on any machine. If you have a free Google Drive account, you can make a
-copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can
-edit the code. Alternatively, start a new colab in your Google Drive as
-follows: [Go here](https://drive.google.com/drive/my-drive) and click on `New`
--> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
-```python !pip install tinyfive from tinyfive.machine import machine import
-numpy as np m = machine(mem_size=4000) # instantiate RISC-V machine with 4KB of
-memory ``` ## Running without package If you don't want to use the TinyFive
-python package, then you can clone the latest repo and install numpy as
-follows: ```bash git clone https://github.com/OpenMachine-ai/tinyfive.git cd
-tinyfive pip install numpy ``` To run the examples, type: ```bash python3
-examples.py ``` To run the test suite, type: ```bash python3 tests.py ``` If
-you don't want to run above steps on your local machine, you can run it in a
-colab as follows: Start a new colab in your Google Drive by [going here](https:
-//drive.google.com/drive/my-drive) and clicking on `New` -> `More` -> `Google
-Colaboratory`. Then copy below lines into your colab: ```python !git clone
-https://github.com/OpenMachine-ai/tinyfive.git %cd tinyfive # run examples
-!python3 examples.py # run test suite !python3 tests.py ``` ## Speed - TinyFive
-is not optimized for speed (but for ease-of-use and [LOC](https://
-en.wikipedia.org/wiki/Source_lines_of_code)). - You might be able to use
-[Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see
-e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-
-riscv2016.pdf) for details). - If you only use the upper-case instructions such
-as `ADD()`, then TinyFive is very fast because there is no instruction
-decoding. And you should be able to accelerate it on a GPU or TPU. - If you use
-the lower-case instructions with `asm()` and `exe()`, then execution of these
-functions is slow as they involve look-up and string matching with O(n)
-complexity where "n" is the total number of instructions. The current
-implementations of `asm()` and `dec()` are optimized for ease-of-use and
-readability. A faster implementation would collapse multiple look-ups into one
-look-up, optimize the pattern-matching for the instruction decoding (bits -
-> instruction), and change the order of the instructions so that more
-frequently used instructions are at the top of the list. [Here is an older
-version](https://github.com/OpenMachine-ai/tinyfive/blob/
-2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster
-`dec()` function that collapses two look-ups (`bits -> instruction` and
-`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ## Latest
-status - TinyFive is still under construction, many things haven't been
-implemented and tested yet. - 37 of the 40 base instructions (RV32I), all
-instructions of the M-extension (RV32M) and the F-extension (RV32F) with the
-default rounding mode are already implemented, and many of them are tested.
-(The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not
-applicable here.) - Remaining work: improve testing, add perhaps more
-extensions. See TODOs in the code for more details. ## Comparison The table
-below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/
-Instruction_set_simulator) and emulator projects. | ISS | Author | Language |
-Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | ---------- |
---- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) | OpenMachine |
-Python | No | I, M, some F | < 1k | | [Pydgin](https://github.com/cornell-brg/
-pydgin) | Cornell University | Python, C | Last update 2016 | A, D, F, I, M | |
-| [Spike](https://github.com/riscv-software-src/riscv-isa-sim) | UC Berkeley |
-C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/) | [Fabrice Bellard]
-(https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [TinyEMU]
-(https://bellard.org/tinyemu/) | [Fabrice Bellard](https://en.wikipedia.org/
-wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim](https://github.com/
-riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All | | | [Whisper]
-(https://github.com/chipsalliance/SweRV-ISS) | Western Digital | C, C++ | Yes |
-Almost all | | | [Sail Model](https://github.com/riscv/sail-riscv) | Cambridge,
-Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https://github.com/PiMaker/
-rvc) | PiMaker | C | | | | | [mini-rv32ima](https://github.com/cnlohr/mini-
-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr | < 1k | ## References
-- Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/
-download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See [this RISC-V card]
-(https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief
-description of most instructions. See also the [RISC-V reference card](http://
-riscvbook.com/greencard-20181213.pdf). - Book "The RISC-V Reader: An Open
-Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this
-book defines all instructions. The Spanish version of this book is [available
-for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
-other free versions are [available here](http://riscvbook.com). - Pydgin
-[paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and
-[video](https://youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/
-research/briscv/simulator/simulator.html) for debug ## Tiny Tech promise
-Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://
-github.com/karpathy/micrograd), and other âtiny techâ projects, we believe
-that core technology should be simple and small (in terms of LOC). Therefore,
-we will make sure that the core of TinyFive (without tests and examples) will
-always be below 1000 lines. Simplicity and size (in terms of number of
-instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/
-Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as
-opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200
-pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
-the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-
-1.0.5.pdf).
+network layers Coming soon, see [file layer_examples.py](layer_examples.py) for
+now ### Example 5: MobileNet Coming soon-ish, see [file mobilenet_v1_0.25.py]
+(mobilenet_v1_0.25.py) for now ## Running in colab [Colab] This is the quickest
+way to get started and should work on any machine. If you have a free Google
+Drive account, you can make a copy of this colab via the menu `File` -> `Save a
+copy in Drive`. Now you can edit the code. Alternatively, start a new colab in
+your Google Drive as follows: [Go here](https://drive.google.com/drive/my-
+drive) and click on `New` -> `More` -> `Google Colaboratory`. Then copy below
+lines into your colab: ```python !pip install tinyfive from tinyfive.machine
+import machine import numpy as np m = machine(mem_size=4000) # instantiate
+RISC-V machine with 4KB of memory ``` ## Running without package If you don't
+want to use the TinyFive python package, then you can clone the latest repo and
+install numpy as follows: ```bash git clone https://github.com/OpenMachine-ai/
+tinyfive.git cd tinyfive pip install numpy ``` To run the examples, type:
+```bash python3 examples.py ``` To run the test suite, type: ```bash python3
+tests.py ``` If you don't want to run above steps on your local machine, you
+can run it in a colab as follows: Start a new colab in your Google Drive by
+[going here](https://drive.google.com/drive/my-drive) and clicking on `New` -
+> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
+```python !git clone https://github.com/OpenMachine-ai/tinyfive.git %cd
+tinyfive # run examples !python3 examples.py # run test suite !python3 tests.py
+``` ## Contribute If you like this project, give it a â­ and share it with
+friends! And if you are interested in helping make TinyFive better, I highly
+welcome you to do so. I thank you in advance for your interest. If you are
+unsure of what you could do to improve the project, you may have a look [here]
+(https://github.com/OpenMachine-ai/tinyfive/issues/5). ## Latest status -
+TinyFive is still under construction, many things haven't been implemented and
+tested yet. - 37 of the 40 base instructions (RV32I), all instructions of the
+M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode
+are already implemented, and many of them are tested. (The three missing RV32I
+instructions `fence`, `ebreak`, and `ecall` are not applicable here.) -
+Remaining work: improve testing, add more extensions. See TODOs in the code for
+more details. - Stay updated by following us on [Twitter](https://twitter.com/
+OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn]
+(https://www.linkedin.com/in/nilsgraef/). ## Speed - TinyFive is not optimized
+for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
+Source_lines_of_code)). - You might be able to use [Codon](https://github.com/
+exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https:
+//www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details). - If
+you only use the upper-case instructions such as `ADD()`, then TinyFive is very
+fast because there is no instruction decoding. And you should be able to
+accelerate it on a GPU or TPU. - If you use the lower-case instructions with
+`asm()` and `exe()`, then execution of these functions is slow as they involve
+look-up and string matching with O(n) complexity where "n" is the total number
+of instructions. The current implementations of `asm()` and `dec()` are
+optimized for ease-of-use and readability. A faster implementation would
+collapse multiple look-ups into one look-up, optimize the pattern-matching for
+the instruction decoding (bits -> instruction), and change the order of the
+instructions so that more frequently used instructions are at the top of the
+list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/
+blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a
+faster `dec()` function that collapses two look-ups (`bits -> instruction` and
+`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ##
+Comparison The table below compares TinyFive with other [ISS](https://
+en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects. | ISS |
+Author | Language | Mature? | Extensions | LOC | | --- | ------ | -------- | --
+----- | ---------- | --- | | [TinyFive](https://github.com/OpenMachine-ai/
+tinyfive) | OpenMachine | Python | No | I, M, some F | < 1k | | [Pydgin](https:
+//github.com/cornell-brg/pydgin) | Cornell University | Python, C | Last update
+2016 | A, D, F, I, M | | | [Spike](https://github.com/riscv-software-src/riscv-
+isa-sim) | UC Berkeley | C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/
+) | [Fabrice Bellard](https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes
+| All | | | [TinyEMU](https://bellard.org/tinyemu/) | [Fabrice Bellard](https:/
+/en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
+(https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
+| | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
+C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
+riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
+/github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
+github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
+| < 1k | ## References - [HuggingFive :raised_hand_with_fingers_splayed:]
+(https://github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https:
+//github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
+spec-20191213.pdf) - See [this RISC-V card](https://inst.eecs.berkeley.edu/
+~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions.
+See also the [RISC-V reference card](http://riscvbook.com/greencard-
+20181213.pdf). - Book [The RISC-V Reader: An Open Architecture Atlas](https://
+www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David
+Patterson and Andrew Waterman. Appendix A of this book defines all
+instructions. The Spanish version of this book is [available for free](http://
+riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf), other free versions
+are [available here](http://riscvbook.com). - Pydgin [paper](https://
+www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://
+youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/research/briscv/
+simulator/simulator.html) for debug ## Tiny Tech promise Similar to [TinyEMU]
+(https://bellard.org/tinyemu/), [tinygrad](https://github.com/geohot/tinygrad),
+and other âtiny techâ projects, we believe that core technology should be
+simple and small (in terms of LOC). Therefore, we will make sure that the core
+of TinyFive (without tests and examples) will always be below 1000 lines.
+Simplicity and size (in terms of number of instructions) is a key feature of
+[RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R"
+in RISC stands for "reduced" (as opposed to complex CISC). Specifically, the
+ISA manual of RISC-V has only ~200 pages while the ARM-32 manual is over 2000
+pages long according to Fig. 1.6 of the [RISC-V Reader](http://riscvbook.com/
+spanish/guia-practica-de-risc-v-1.0.5.pdf).
      [https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg]
```

### Comparing `tinyfive-0.0.14/pyproject.toml` & `tinyfive-0.0.15/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfive"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Open Machine", email="tinyfive@openmachine.ai" },
 ]
 description = "TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tinyfive-0.0.14/PKG-INFO` & `tinyfive-0.0.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyfive
-Version: 0.0.14
+Version: 0.0.15
 Summary: TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python
 Project-URL: Homepage, https://github.com/OpenMachine-ai/tinyfive
 Project-URL: Bug Tracker, https://github.com/OpenMachine-ai/tinyfive/issues
 Author-email: Open Machine <tinyfive@openmachine.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,35 +13,41 @@
 Requires-Dist: numpy>1.20.0
 Description-Content-Type: text/markdown
 
 # TinyFive
 
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20"> </a>
 [![Downloads](https://static.pepy.tech/badge/tinyfive)](https://pepy.tech/project/tinyfive)
+
+<!--- view counter is currently commented out
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FOpenMachine-ai%2Ftinyfive&title_bg=%23555555&icon=&title=views+%28today+%2F+total%29&edge_flat=false)](https://hits.seeyoufarm.com)
+ --->
 
 TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python:
-- It's useful for running neural networks on RISC-V: Simulate your RISC-V assembly code along with your neural network in Python (and without relying on RISC-V toolchains). Custom instructions can be easily added.
-- TinyFive is also useful for ML scientists who are using ML/RL for compiler optimization (see e.g. [CompilerGym](https://github.com/facebookresearch/CompilerGym/blob/development/README.md)).
-- If you want to learn how RISC-V works, TinyFive lets you play with instructions and assembly code.
+- Useful for running neural networks on RISC-V: Simulate your RISC-V assembly code along with a neural network in Keras or PyTorch (and without relying on RISC-V toolchains).
+- Custom instructions can be added for easy HW/SW codesign in Python (without C++ and compiler toolchains).
+- If you want to learn how RISC-V works, TinyFive lets you play with instructions and assembly code in [this colab](https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb).
+- TinyFive might also be useful for ML scientists who are using ML/RL for compiler optimizations (see e.g. [CompilerGym](https://github.com/facebookresearch/CompilerGym/blob/development/README.md)) or to replace compiler toolchains by AI.
 - Can be very fast if you only use the upper-case instructions defined in the [first ~200 lines of machine.py](machine.py#L1-L200).
 - [Fewer than 1000 lines](machine.py) of code (w/o tests and examples)
 - Uses NumPy for math
 
 ## Contents
 - [Installation](#installation)
 - [Usage](#usage)
   - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers)
   - [Example 2: Add two vectors](#example-2-add-two-vectors)
   - [Example 3: Multiply two matrices](#example-3-multiply-two-matrices)
   - [Example 4: Neural network layers](#example-4-neural-network-layers)
+  - [Example 5: MobileNet](#example-5-mobilenet)
 - [Running in colab](#running-in-colab)
 - [Running without package](#running-without-package)
-- [Speed](#speed)
+- [Contribute](#contribute)
 - [Latest status](#latest-status)
+- [Speed](#speed)
 - [Comparison](#comparison)
 - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise)
 
 ## Installation
 ```
 pip install tinyfive
@@ -388,23 +394,28 @@
 ref = np.matmul(A, B)            # golden reference
 print(np.array_equal(res, ref))  # should return 'True'
 # Output: True
 ```
 The table below shows a speedup of 1.7 with the following caveats:
 - The bit-widths don't make sense for fixed point (in general, multiplying two 32-bit integers produces a 64-bit product; and adding 4 of these products requires up to 66 bits).
 - For runtime calculations, we assume that our RISC-V CPU can only perform one instruction per cycle (while many RISC-V cores can perform multiple instructions per cycle).
+- We assume all 31 registers can be used, which is unrealistic because we ignore register allocation conventions such as the procedure
+calling conventions specified [here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc).
 - For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
 ### Example 4: Neural network layers
-Coming soon, see [file layer_examples.py](layer_examples.py)
+Coming soon, see [file layer_examples.py](layer_examples.py) for now
+
+### Example 5: MobileNet
+Coming soon-ish, see [file mobilenet_v1_0.25.py](mobilenet_v1_0.25.py) for now
 
 ## Running in colab
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20">
 </a>  This is the quickest way to get started and should work on any machine.
 
 If you have a free Google Drive account, you can make a copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
@@ -442,26 +453,30 @@
 
 # run examples
 !python3 examples.py
 
 # run test suite
 !python3 tests.py
 ```
+## Contribute
+If you like this project, give it a ⭐ and share it with friends!  And if you are interested in helping make TinyFive better,
+I highly welcome you to do so. I thank you in advance for your interest.  If you are unsure of what you could do to improve the project, you may have a look [here](https://github.com/OpenMachine-ai/tinyfive/issues/5).
+
+## Latest status
+- TinyFive is still under construction, many things haven't been implemented and tested yet.
+- 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
+- Remaining work: improve testing, add more extensions. See TODOs in the code for more details.
+- Stay updated by following us on [Twitter](https://twitter.com/OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn](https://www.linkedin.com/in/nilsgraef/).
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
 - You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
-## Latest status
-- TinyFive is still under construction, many things haven't been implemented and tested yet.
-- 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
-- Remaining work: improve testing, add perhaps more extensions. See TODOs in the code for more details.
-
 ## Comparison
 The table below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects.
 
 | ISS | Author | Language | Mature? | Extensions | LOC |
 | --- | ------ | -------- | ------- | ---------- | --- |
 | [TinyFive](https://github.com/OpenMachine-ai/tinyfive)             | OpenMachine          | Python    | No               | I, M, some F  | < 1k |
 | [Pydgin](https://github.com/cornell-brg/pydgin)                    | Cornell University   | Python, C | Last update 2016 | A, D, F, I, M | |
@@ -471,23 +486,24 @@
 | [riscvOVPsim](https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas              | C         | Yes              | All           | |
 | [Whisper](https://github.com/chipsalliance/SweRV-ISS)              | Western Digital      | C, C++    | Yes | Almost all                 | |
 | [Sail Model](https://github.com/riscv/sail-riscv)                  | Cambridge, Edinburgh | Sail, C   | Yes | All                        | |
 | [PiMaker/rvc](https://github.com/PiMaker/rvc)                      | PiMaker              | C         |     |                            | |
 | [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)             | Charles Lohr         | C         |     | A, I, M, Zifencei, Zicsr   | < 1k |
 
 ## References
+- [HuggingFive :raised_hand_with_fingers_splayed:](https://github.com/OpenMachine-ai/HuggingFive)
 - Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf)
 - See [this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions. See also the [RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf).
-- Book "The RISC-V Reader: An Open Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
+- Book [The RISC-V Reader: An Open Architecture Atlas](https://www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David Patterson and Andrew Waterman. Appendix A of this book defines all instructions. The Spanish version of this book is [available for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
 other free versions are [available here](http://riscvbook.com).
 - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk)
 - [Online simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for debug
 
 ## Tiny Tech promise
-Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://github.com/karpathy/micrograd), and other “tiny tech” projects, we believe that core technology should be simple and small (in terms of LOC). Therefore, we will make sure that the core of TinyFive (without tests and examples) will always be below 1000 lines.
+Similar to [TinyEMU](https://bellard.org/tinyemu/), [tinygrad](https://github.com/geohot/tinygrad), and other “tiny tech” projects, we believe that core technology should be simple and small (in terms of LOC). Therefore, we will make sure that the core of TinyFive (without tests and examples) will always be below 1000 lines.
 
 Simplicity and size (in terms of number of instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200 pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
 the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf).
 
 <p align="center">
   <img src="https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg">
 </p>
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: tinyfive Version: 0.0.14 Summary: TinyFive is a
+Metadata-Version: 2.1 Name: tinyfive Version: 0.0.15 Summary: TinyFive is a
 lightweight RISC-V emulator and assembler written entirely in Python Project-
 URL: Homepage, https://github.com/OpenMachine-ai/tinyfive Project-URL: Bug
 Tracker, https://github.com/OpenMachine-ai/tinyfive/issues Author-email: Open
 Machine
 openmachine.ai> License-File: LICENSE Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
 numpy>1.20.0 Description-Content-Type: text/markdown # TinyFive [Colab] [!
 [Downloads](https://static.pepy.tech/badge/tinyfive)](https://pepy.tech/
-project/tinyfive) [![Hits](https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2FOpenMachine-
-ai%2Ftinyfive&title_bg=%23555555&icon=&title=views+%28today+%2F+total%29&edge_flat=false)]
-(https://hits.seeyoufarm.com) TinyFive is a lightweight RISC-V emulator and
-assembler written entirely in Python: - It's useful for running neural networks
-on RISC-V: Simulate your RISC-V assembly code along with your neural network in
-Python (and without relying on RISC-V toolchains). Custom instructions can be
-easily added. - TinyFive is also useful for ML scientists who are using ML/RL
-for compiler optimization (see e.g. [CompilerGym](https://github.com/
-facebookresearch/CompilerGym/blob/development/README.md)). - If you want to
-learn how RISC-V works, TinyFive lets you play with instructions and assembly
-code. - Can be very fast if you only use the upper-case instructions defined in
-the [first ~200 lines of machine.py](machine.py#L1-L200). - [Fewer than 1000
-lines](machine.py) of code (w/o tests and examples) - Uses NumPy for math ##
-Contents - [Installation](#installation) - [Usage](#usage) - [Example 1:
-Multiply two numbers](#example-1-multiply-two-numbers) - [Example 2: Add two
-vectors](#example-2-add-two-vectors) - [Example 3: Multiply two matrices]
-(#example-3-multiply-two-matrices) - [Example 4: Neural network layers]
-(#example-4-neural-network-layers) - [Running in colab](#running-in-colab) -
-[Running without package](#running-without-package) - [Speed](#speed) - [Latest
-status](#latest-status) - [Comparison](#comparison) - [References](#references)
-- [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip install
-tinyfive ``` ## Usage TinyFive can be used in the following three ways: -
-**Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
+project/tinyfive)  TinyFive is a lightweight RISC-V emulator and assembler
+written entirely in Python: - Useful for running neural networks on RISC-V:
+Simulate your RISC-V assembly code along with a neural network in Keras or
+PyTorch (and without relying on RISC-V toolchains). - Custom instructions can
+be added for easy HW/SW codesign in Python (without C++ and compiler
+toolchains). - If you want to learn how RISC-V works, TinyFive lets you play
+with instructions and assembly code in [this colab](https://
+colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/
+colab.ipynb). - TinyFive might also be useful for ML scientists who are using
+ML/RL for compiler optimizations (see e.g. [CompilerGym](https://github.com/
+facebookresearch/CompilerGym/blob/development/README.md)) or to replace
+compiler toolchains by AI. - Can be very fast if you only use the upper-case
+instructions defined in the [first ~200 lines of machine.py](machine.py#L1-
+L200). - [Fewer than 1000 lines](machine.py) of code (w/o tests and examples) -
+Uses NumPy for math ## Contents - [Installation](#installation) - [Usage]
+(#usage) - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers) -
+[Example 2: Add two vectors](#example-2-add-two-vectors) - [Example 3: Multiply
+two matrices](#example-3-multiply-two-matrices) - [Example 4: Neural network
+layers](#example-4-neural-network-layers) - [Example 5: MobileNet](#example-5-
+mobilenet) - [Running in colab](#running-in-colab) - [Running without package]
+(#running-without-package) - [Contribute](#contribute) - [Latest status]
+(#latest-status) - [Speed](#speed) - [Comparison](#comparison) - [References]
+(#references) - [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip
+install tinyfive ``` ## Usage TinyFive can be used in the following three ways:
+- **Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
 examples 1.1, 1.2, 2.1, and 3.1 below. - **Option B:** Use `asm()` and `exe()`
 functions without branch instructions, see examples 1.3 and 2.2 below. -
 **Option C:** Use `asm()` and `exe()` functions with branch instructions, see
 example 2.3, 3.2, and 3.3 below. For the examples below, import and instantiate
 a RISC-V machine with at least 4KB of memory as follows: ```python from
 tinyfive.machine import machine m = machine(mem_size=4000) # instantiate RISC-
 V machine with 4KB of memory ``` ### Example 1: Multiply two numbers **Example
@@ -240,103 +241,115 @@
 (4*32, size=4*4).reshape(4, 4) # read result matrix ref = np.matmul(A, B) #
 golden reference print(np.array_equal(res, ref)) # should return 'True' #
 Output: True ``` The table below shows a speedup of 1.7 with the following
 caveats: - The bit-widths don't make sense for fixed point (in general,
 multiplying two 32-bit integers produces a 64-bit product; and adding 4 of
 these products requires up to 66 bits). - For runtime calculations, we assume
 that our RISC-V CPU can only perform one instruction per cycle (while many
-RISC-V cores can perform multiple instructions per cycle). - For 16x16 or
+RISC-V cores can perform multiple instructions per cycle). - We assume all 31
+registers can be used, which is unrealistic because we ignore register
+allocation conventions such as the procedure calling conventions specified
+[here](https://github.com/riscv-non-isa/riscv-elf-psabi-doc). - For 16x16 or
 larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
 Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
 discovering-novel-algorithms-with-alphatensor) can reduce the total number of
 multiplications and additions if they are applied recursively. | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
 3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
-network layers Coming soon, see [file layer_examples.py](layer_examples.py) ##
-Running in colab [Colab] This is the quickest way to get started and should
-work on any machine. If you have a free Google Drive account, you can make a
-copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can
-edit the code. Alternatively, start a new colab in your Google Drive as
-follows: [Go here](https://drive.google.com/drive/my-drive) and click on `New`
--> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
-```python !pip install tinyfive from tinyfive.machine import machine import
-numpy as np m = machine(mem_size=4000) # instantiate RISC-V machine with 4KB of
-memory ``` ## Running without package If you don't want to use the TinyFive
-python package, then you can clone the latest repo and install numpy as
-follows: ```bash git clone https://github.com/OpenMachine-ai/tinyfive.git cd
-tinyfive pip install numpy ``` To run the examples, type: ```bash python3
-examples.py ``` To run the test suite, type: ```bash python3 tests.py ``` If
-you don't want to run above steps on your local machine, you can run it in a
-colab as follows: Start a new colab in your Google Drive by [going here](https:
-//drive.google.com/drive/my-drive) and clicking on `New` -> `More` -> `Google
-Colaboratory`. Then copy below lines into your colab: ```python !git clone
-https://github.com/OpenMachine-ai/tinyfive.git %cd tinyfive # run examples
-!python3 examples.py # run test suite !python3 tests.py ``` ## Speed - TinyFive
-is not optimized for speed (but for ease-of-use and [LOC](https://
-en.wikipedia.org/wiki/Source_lines_of_code)). - You might be able to use
-[Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see
-e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-
-riscv2016.pdf) for details). - If you only use the upper-case instructions such
-as `ADD()`, then TinyFive is very fast because there is no instruction
-decoding. And you should be able to accelerate it on a GPU or TPU. - If you use
-the lower-case instructions with `asm()` and `exe()`, then execution of these
-functions is slow as they involve look-up and string matching with O(n)
-complexity where "n" is the total number of instructions. The current
-implementations of `asm()` and `dec()` are optimized for ease-of-use and
-readability. A faster implementation would collapse multiple look-ups into one
-look-up, optimize the pattern-matching for the instruction decoding (bits -
-> instruction), and change the order of the instructions so that more
-frequently used instructions are at the top of the list. [Here is an older
-version](https://github.com/OpenMachine-ai/tinyfive/blob/
-2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster
-`dec()` function that collapses two look-ups (`bits -> instruction` and
-`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ## Latest
-status - TinyFive is still under construction, many things haven't been
-implemented and tested yet. - 37 of the 40 base instructions (RV32I), all
-instructions of the M-extension (RV32M) and the F-extension (RV32F) with the
-default rounding mode are already implemented, and many of them are tested.
-(The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not
-applicable here.) - Remaining work: improve testing, add perhaps more
-extensions. See TODOs in the code for more details. ## Comparison The table
-below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/
-Instruction_set_simulator) and emulator projects. | ISS | Author | Language |
-Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | ---------- |
---- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) | OpenMachine |
-Python | No | I, M, some F | < 1k | | [Pydgin](https://github.com/cornell-brg/
-pydgin) | Cornell University | Python, C | Last update 2016 | A, D, F, I, M | |
-| [Spike](https://github.com/riscv-software-src/riscv-isa-sim) | UC Berkeley |
-C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/) | [Fabrice Bellard]
-(https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [TinyEMU]
-(https://bellard.org/tinyemu/) | [Fabrice Bellard](https://en.wikipedia.org/
-wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim](https://github.com/
-riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All | | | [Whisper]
-(https://github.com/chipsalliance/SweRV-ISS) | Western Digital | C, C++ | Yes |
-Almost all | | | [Sail Model](https://github.com/riscv/sail-riscv) | Cambridge,
-Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https://github.com/PiMaker/
-rvc) | PiMaker | C | | | | | [mini-rv32ima](https://github.com/cnlohr/mini-
-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr | < 1k | ## References
-- Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/
-download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See [this RISC-V card]
-(https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief
-description of most instructions. See also the [RISC-V reference card](http://
-riscvbook.com/greencard-20181213.pdf). - Book "The RISC-V Reader: An Open
-Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this
-book defines all instructions. The Spanish version of this book is [available
-for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
-other free versions are [available here](http://riscvbook.com). - Pydgin
-[paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and
-[video](https://youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/
-research/briscv/simulator/simulator.html) for debug ## Tiny Tech promise
-Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://
-github.com/karpathy/micrograd), and other âtiny techâ projects, we believe
-that core technology should be simple and small (in terms of LOC). Therefore,
-we will make sure that the core of TinyFive (without tests and examples) will
-always be below 1000 lines. Simplicity and size (in terms of number of
-instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/
-Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as
-opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200
-pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
-the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-
-1.0.5.pdf).
+network layers Coming soon, see [file layer_examples.py](layer_examples.py) for
+now ### Example 5: MobileNet Coming soon-ish, see [file mobilenet_v1_0.25.py]
+(mobilenet_v1_0.25.py) for now ## Running in colab [Colab] This is the quickest
+way to get started and should work on any machine. If you have a free Google
+Drive account, you can make a copy of this colab via the menu `File` -> `Save a
+copy in Drive`. Now you can edit the code. Alternatively, start a new colab in
+your Google Drive as follows: [Go here](https://drive.google.com/drive/my-
+drive) and click on `New` -> `More` -> `Google Colaboratory`. Then copy below
+lines into your colab: ```python !pip install tinyfive from tinyfive.machine
+import machine import numpy as np m = machine(mem_size=4000) # instantiate
+RISC-V machine with 4KB of memory ``` ## Running without package If you don't
+want to use the TinyFive python package, then you can clone the latest repo and
+install numpy as follows: ```bash git clone https://github.com/OpenMachine-ai/
+tinyfive.git cd tinyfive pip install numpy ``` To run the examples, type:
+```bash python3 examples.py ``` To run the test suite, type: ```bash python3
+tests.py ``` If you don't want to run above steps on your local machine, you
+can run it in a colab as follows: Start a new colab in your Google Drive by
+[going here](https://drive.google.com/drive/my-drive) and clicking on `New` -
+> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
+```python !git clone https://github.com/OpenMachine-ai/tinyfive.git %cd
+tinyfive # run examples !python3 examples.py # run test suite !python3 tests.py
+``` ## Contribute If you like this project, give it a â­ and share it with
+friends! And if you are interested in helping make TinyFive better, I highly
+welcome you to do so. I thank you in advance for your interest. If you are
+unsure of what you could do to improve the project, you may have a look [here]
+(https://github.com/OpenMachine-ai/tinyfive/issues/5). ## Latest status -
+TinyFive is still under construction, many things haven't been implemented and
+tested yet. - 37 of the 40 base instructions (RV32I), all instructions of the
+M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode
+are already implemented, and many of them are tested. (The three missing RV32I
+instructions `fence`, `ebreak`, and `ecall` are not applicable here.) -
+Remaining work: improve testing, add more extensions. See TODOs in the code for
+more details. - Stay updated by following us on [Twitter](https://twitter.com/
+OpenMachine_AI), [Post.news](https://post.news/@/openmachine), and [LinkedIn]
+(https://www.linkedin.com/in/nilsgraef/). ## Speed - TinyFive is not optimized
+for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
+Source_lines_of_code)). - You might be able to use [Codon](https://github.com/
+exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https:
+//www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details). - If
+you only use the upper-case instructions such as `ADD()`, then TinyFive is very
+fast because there is no instruction decoding. And you should be able to
+accelerate it on a GPU or TPU. - If you use the lower-case instructions with
+`asm()` and `exe()`, then execution of these functions is slow as they involve
+look-up and string matching with O(n) complexity where "n" is the total number
+of instructions. The current implementations of `asm()` and `dec()` are
+optimized for ease-of-use and readability. A faster implementation would
+collapse multiple look-ups into one look-up, optimize the pattern-matching for
+the instruction decoding (bits -> instruction), and change the order of the
+instructions so that more frequently used instructions are at the top of the
+list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/
+blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a
+faster `dec()` function that collapses two look-ups (`bits -> instruction` and
+`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ##
+Comparison The table below compares TinyFive with other [ISS](https://
+en.wikipedia.org/wiki/Instruction_set_simulator) and emulator projects. | ISS |
+Author | Language | Mature? | Extensions | LOC | | --- | ------ | -------- | --
+----- | ---------- | --- | | [TinyFive](https://github.com/OpenMachine-ai/
+tinyfive) | OpenMachine | Python | No | I, M, some F | < 1k | | [Pydgin](https:
+//github.com/cornell-brg/pydgin) | Cornell University | Python, C | Last update
+2016 | A, D, F, I, M | | | [Spike](https://github.com/riscv-software-src/riscv-
+isa-sim) | UC Berkeley | C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/
+) | [Fabrice Bellard](https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes
+| All | | | [TinyEMU](https://bellard.org/tinyemu/) | [Fabrice Bellard](https:/
+/en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
+(https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
+| | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
+C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
+riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
+/github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
+github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
+| < 1k | ## References - [HuggingFive :raised_hand_with_fingers_splayed:]
+(https://github.com/OpenMachine-ai/HuggingFive) - Official [RISC-V spec](https:
+//github.com/riscv/riscv-isa-manual/releases/download/Ratified-IMAFDQC/riscv-
+spec-20191213.pdf) - See [this RISC-V card](https://inst.eecs.berkeley.edu/
+~cs61c/fa18/img/riscvcard.pdf) for a brief description of most instructions.
+See also the [RISC-V reference card](http://riscvbook.com/greencard-
+20181213.pdf). - Book [The RISC-V Reader: An Open Architecture Atlas](https://
+www.abebooks.com/book-search/author/patterson-david-waterman-andrew/) by David
+Patterson and Andrew Waterman. Appendix A of this book defines all
+instructions. The Spanish version of this book is [available for free](http://
+riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf), other free versions
+are [available here](http://riscvbook.com). - Pydgin [paper](https://
+www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and [video](https://
+youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/research/briscv/
+simulator/simulator.html) for debug ## Tiny Tech promise Similar to [TinyEMU]
+(https://bellard.org/tinyemu/), [tinygrad](https://github.com/geohot/tinygrad),
+and other âtiny techâ projects, we believe that core technology should be
+simple and small (in terms of LOC). Therefore, we will make sure that the core
+of TinyFive (without tests and examples) will always be below 1000 lines.
+Simplicity and size (in terms of number of instructions) is a key feature of
+[RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R"
+in RISC stands for "reduced" (as opposed to complex CISC). Specifically, the
+ISA manual of RISC-V has only ~200 pages while the ARM-32 manual is over 2000
+pages long according to Fig. 1.6 of the [RISC-V Reader](http://riscvbook.com/
+spanish/guia-practica-de-risc-v-1.0.5.pdf).
      [https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg]
```

