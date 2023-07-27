# Comparing `tmp/TensorFlow1-1.1.0.tar.gz` & `tmp/TensorFlow1-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlow1-1.1.0.tar", last modified: Tue Jul 25 14:54:24 2023, max compression
+gzip compressed data, was "TensorFlow1-2.2.1.tar", last modified: Thu Jul 27 18:56:19 2023, max compression
```

## Comparing `TensorFlow1-1.1.0.tar` & `TensorFlow1-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.943781 TensorFlow1-1.1.0/
--rw-rw-rw-   0        0        0      193 2023-07-25 14:54:24.943781 TensorFlow1-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.923442 TensorFlow1-1.1.0/TensorFlow1/
--rw-rw-rw-   0        0        0    17833 2023-07-25 14:37:39.000000 TensorFlow1-1.1.0/TensorFlow1/TensorFlow.py
--rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-1.1.0/TensorFlow1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.942777 TensorFlow1-1.1.0/TensorFlow1.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-1.1.0/license.txt
--rw-rw-rw-   0        0        0      158 2023-07-25 14:54:24.952251 TensorFlow1-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-07-25 14:53:56.000000 TensorFlow1-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.536582 TensorFlow1-2.2.1/
+-rw-rw-rw-   0        0        0      193 2023-07-27 18:56:19.536582 TensorFlow1-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.520265 TensorFlow1-2.2.1/TensorFlow1/
+-rw-rw-rw-   0        0        0    19024 2023-07-27 18:48:05.000000 TensorFlow1-2.2.1/TensorFlow1/TensorFlow.py
+-rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-2.2.1/TensorFlow1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.534187 TensorFlow1-2.2.1/TensorFlow1.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-2.2.1/license.txt
+-rw-rw-rw-   0        0        0      158 2023-07-27 18:56:19.541341 TensorFlow1-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-07-27 18:52:50.000000 TensorFlow1-2.2.1/setup.py
```

### Comparing `TensorFlow1-1.1.0/TensorFlow1/TensorFlow.py` & `TensorFlow1-2.2.1/TensorFlow1/TensorFlow.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,444 +41,446 @@
                     print('Root Mean Square Error:', rootMeanSqErr)''')
     def m2(self):
         print('''
         import pandas as pd
         import numpy as np
         import matplotlib.pyplot as plt
         a=pd.read_csv('seattle-weather.csv')
+        a
         a=a.drop(['date'],axis=1)
+        a
         from sklearn.preprocessing import LabelEncoder
         a['weather'].value_counts()
         l=LabelEncoder()
-        a['w']=l.fit_transform(a['weather'])       
+        a['w']=l.fit_transform(a['weather'])
         a=a.drop(['weather'],axis=1)
+        a
         from sklearn.model_selection import train_test_split
-        a.columns        
-        x=a[['precipitation','temp_max','temp_min','wind']]
+        a.columns
+        x=a[['precipitation', 'temp_max', 'temp_min', 'wind']]
         y=a['w']
-        x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.1,random_stafrom sklearn.linear_model import LinearRegression
+        x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.1,random_state=10)
+        from sklearn.linear_model import LinearRegression
         m=LinearRegression()
-        m.fit(x_train,y_train)       
+        m.fit(x_train,y_train)
         m.predict([[8.6,4.4,1.7,1.3]])
         y_predict=m.predict(x_test).round(0)
         y_test=y_test.round(0)
         from sklearn.metrics import f1_score
-        f1_score(y_test,y_predict,average='micro')
+        f1_score(y_test,y_predict,average='micro')                                                                                             
         i=np.array(range(50))
         plt.scatter(i,y_predict[0:50])
         plt.scatter(i,y_test[0:50])
         ''')
     def m3(self):
         print('''
                 import csv
-                a=[]
-                print("\n The given training dataset")
-                with open('Enjoysports.csv','r')as csvfile:
-                    reader = csv.reader(csvfile)
-                    for row in reader:
-                        a.append(row)
-                        print(row)
-                num_attributes = len(a[0])-1
-                print("\n The intial value of hypothesis:")
-                S=['0']*num_attributes
-                G=['?']*num_attributes
-                print("\n The most specific hypothesis SO:[0,0,0,0,0,0]")
-                print("\n The most general hypothesis GO : [?,?,?,?,?,?]")
-                for j in range(0,num_attributes):
-                S[j]=a[0][j];
-                print("\n Candidate Elimation algorithm Hpothesis Version space computation
-                temp=[]
-                for i in range(0,len(a)):
-                    if a[i][num_attributes]=='yes':
-                        for j in range(0,num_attributes):
-                            if a[i][j]!=S[j]:
-                                S[j]='?'
-                            for j in range(0,num_attributes):
-                                for k in range(1,len(temp)):
-                                    if temp[k][j]!='?'and temp[k][j]!=S[j]:
-                                        del temp[k]
-                        print("------------------------------------------------------------")
-                        print("For training Example No:{0} the hypothesis is S{0}".format(i+1),S)
-                        if(len(temp)==0):
-                            print("For training Example No:{0} the hypothesis is G{0}".format(i+1),G)
-                        else:
-                            print("For Positive training Example No:{0} the hypothesis is G{0}".format(i+1),temp)
-                    if a[i][num_attributes]=='no':
-                        for j in range(0,num_attributes):
-                            if S[j]!=a[i][j] and S[j]!='?':
-                                G[j]=S[j]
-                                temp.append(G)
-                                G=['?']*num_attributes
-                        print("------------------------------------------------------------
-                        print("For training Example No:{0} the hypothesis is S{0}".format(i+1),S)
-                        print("For Positive training Example No:{0} the hypothesis is G{0}".format(i+1),temp)
+a=[]
+print("/n The Given Training Data Set")
+with open('p2.csv') as csvFile:
+    reader = csv.reader(csvFile)
+    for row in reader:
+        a.append(row)
+        print(row)
+num_attributes = len(a[0])-1
+print("\n The initial value of hypothesis: ") 
+S=['0']*num_attributes
+G=['?']*num_attributes 
+print("\n The most specific hypothesis S0 : [0,0,0,0,0,0]")
+print("\n The most general hypothesis G0 : [?,?,?,?,?,?]")
+for j in range(0,num_attributes): 
+          S[j]=a[0][j];
+print("\n Candidate Elimination algorithm Hypotheses Version Space Computation\n")
+temp=[]
+for i in range(0,len(a)):
+    if a[i][num_attributes]=='Yes':
+        for j in range(0,num_attributes):
+            if a[i][j]!=S[j]:
+                S[j]='?'
+        for j in range(0,num_attributes): 
+            for k in range(1, len(temp)):
+                if temp[k][j]!='?' and temp[k][j]!=S[j]: 
+                    del temp[k]
+
+        print("------------------------------------------------------------------------------------------------------------------------")
+        print( "For Training Example No :{0} the hypothesis is S{0} ".format(i+1),S) 
+        if (len(temp)==0): 
+            print(" For Training Example No : {0} the hypothesis is G{0} ".format(i+1),G)
+        else:
+            print( "For Positive Training Example No : {0} the hypothesis is G{0}".format(i+1), temp) 
+    if a[i][num_attributes]=="No":
+        for j in range(0,num_attributes):
+            if S[j]!= a[i][j] and S[j]!= '?':
+                G[j]=S[j]
+                temp.append(G)
+                G=['?'] * num_attributes
+        print("------------------------------------------------------------------------------------------------------------------------")
+        print("For Training Example No :{0} the hypothesis is S{0} ".format(i+1),S)
+        print(" For Training Example No :{0} the hypothesis is G{0}".format(i+1),temp)    
                     ''')
     def m4(self):
         print('''
 import math
 import csv
 
 def load_csv(filename):
-    lines = csv.reader(open(filename, "r"))
+    lines=csv.reader(open(filename,"r"))
     dataset = list(lines)
     headers = dataset.pop(0)
-    return dataset, headers
+    return dataset,headers
 
 class Node:
-    def __init__(self, attribute):
-        self.attribute = attribute
-        self.children = []
-        self.answer = ""
-
-def subtables(data, col, delete):
-    dic = {}
-    coldata = [row[col] for row in data]
-    attr = list(set(coldata))
-    counts = [0] * len(attr)
-    r = len(data)
-    c = len(data[0])
+    def __init__ (self,attribute):
+        self.attribute=attribute
+        self.children=[]
+        self.answer=""
 
-    for x in range(len(attr)):
-        for y in range(r):
-            if data[y][col] == attr[x]:
-                counts[x] += 1
 
+def subtables(data,col,delete):  #col is basically a column header
+    dic={}
+    coldata=[row[col] for row in data]
+    
+    attr=list(set(coldata))  #set returns only unique values in coldata
+    counts=[0]*len(attr)     #create empty list for every unique value
+    r=len(data)     #no of rows
+    c=len(data[0])  #no of columns in each row
+    for x in range(len(attr)):   #no of unique values in the "col" column 
+        for y in range(r):
+            if data[y][col]==attr[x]:
+                counts[x]+=1    
     for x in range(len(attr)):
-        dic[attr[x]] = [[0 for i in range(c)] for j in range(counts[x])]
-
-    pos = 0
-    for y in range(r):
-        if data[y][col] == attr[x]:
-            if delete:
-                del data[y][col]
-            dic[attr[x]][pos] = data[y]
-            pos += 1
-
-    return attr, dic
+        dic[attr[x]]=[[0 for i in range(c)] for j in range(counts[x])] #initialing the dictionary items
+        pos=0
+        for y in range(r):
+            if data[y][col]==attr[x]:
+                if delete:
+                    del data[y][col]   #removing tat particular column (upper in the tree/parent)
+                dic[attr[x]][pos]=data[y] #all rows for each unique value
+                pos+=1
+    return attr,dic   #attr is a list, dic is a set
 
 def entropy(S):
-    attr = list(set(S))
-    if len(attr) == 1:
-        return 0
-
-    counts = [0, 0]
+    attr=list(set(S))  #S will basically have last column data(not necessarily of all rows)
+    if len(attr)==1:
+        return 0    #if there is either only yes/ only no =>entrop is 0
+    counts=[0,0]
     for i in range(2):
-        counts[i] = sum([1 for x in S if attr[i] == x]) / (len(S) * 1.0)
-
-    sums = 0
+        counts[i]=sum([1 for x in S if attr[i]==x])/(len(S)*1.0) #find no of yes and no of no
+    sums=0
     for cnt in counts:
-        sums += -1 * cnt * math.log(cnt, 2)
-
+        sums+=-1*cnt*math.log(cnt,2)  #base 2(second parameter)
     return sums
 
-def compute_gain(data, col):
-    attr, dic = subtables(data, col, delete=False)
-    total_size = len(data)
-    entropies = [0] * len(attr)
-    ratio = [0] * len(attr)
-    total_entropy = entropy([row[-1] for row in data])
-
+def compute_gain(data,col): #col  is column-header
+    attr,dic = subtables(data,col,delete=False) #here no deletion, we just calculate gain
+    total_size=len(data)  # |S| value in formula
+    entropies=[0]*len(attr) #entropies of each value
+    ratio=[0]*len(attr)   # to maintain |Sv|/|S| values
+    total_entropy=entropy([row[-1] for row in data])
+    
     for x in range(len(attr)):
-        ratio[x] = len(dic[attr[x]]) / (total_size * 1.0)
-        entropies[x] = entropy([row[-1] for row in dic[attr[x]]])
-        total_entropy -= ratio[x] * entropies[x]
+        ratio[x]=len(dic[attr[x]])/(total_size*1.0) #len of dic=> |Sv| value
+        entropies[x]=entropy([row[-1] for row in dic[attr[x]]])
 
+        total_entropy-=ratio[x]*entropies[x] #acc to formula
     return total_entropy
 
-def build_tree(data, features):
-    lastcol = [row[-1] for row in data]
-    if len(set(lastcol)) == 1:
-        node = Node("")
-        node.answer = lastcol[0]
+def build_tree(data,features):
+    lastcol=[row[-1] for row in data]
+    if(len(set(lastcol)))==1:  #if last column contains either only "yes" or only "no"
+        node=Node("")          #we are not building the tree further(so no attribute)
+        node.answer=lastcol[0] #it'll be either yes/no
         return node
-
-    n = len(data[0]) - 1  # -1 because we don't need the last column values
-    gains = [0] * n  # gain is initialized to be 0 for all attributes
-
-    for col in range(n):
-        gains[col] = compute_gain(data, col)  # compute gain of each attribute
-
-    split = gains.index(max(gains))  # split will have the index of an attribute
-    node = Node(features[split])  # features list will have attributes
-    nofea = features[:split] + features[split+1:]
-    attr, dic = subtables(data, split, delete=True)  # attr will have possible values, dic will have all rows for each value
-
-    for x in range(len(attr)):
-        child = build_tree(dic[attr[x]], nofea)  # for each value of the attribute
-        node.children.append((attr[x], child))  # again build the tree (but for a smaller dataset)
-
+    n=len(data[0])-1   #-1 boz we dont need the last column values
+    gains=[0]*n        # gain is initialized to be 0 for all attributes
+    for col in range(n):   
+        gains[col]=compute_gain(data,col)  #compute gain of each attribute
+    
+    split=gains.index(max(gains))          # split will have the index of attribute with "highest gain"
+    node=Node(features[split])             # features list will have attribute headings(col names)
+                                           # so now we create a subtree (node) with that particular attribute
+    fea = features[:split]+features[split+1:] 
+    attr,dic=subtables(data,split,delete=True)  #attr will have possible values for tat particular attribute
+                                                #dic will have all rows for all those attributes(key: values)
+    for x in range(len(attr)):                  
+        child=build_tree(dic[attr[x]],fea)     #for each value of the attribute
+        node.children.append((attr[x],child))  #again build the tree (but fea exclude the one already taken)
     return node
 
-def print_tree(node, level):
-    if node.answer != "":
-        print(" " * level, node.answer)
+def print_tree(node,level):
+    if node.answer!="":              #if its a leaf node
+        print(" "*level,node.answer) #just print "level" no of spaces, followed by answer (yes/no)
         return
+    print(" "*level,node.attribute)  #attribute in the node
+    for value,n in node.children:
+        print(" "*(level+1),value)
+        print_tree(n,level+2)        # recursive call to the next node (child)
 
-    print(" " * level, node.attribute)
-    for value, n in node.children:
-        print(" " * (level + 1), value)
-        print_tree(n, level + 2)  # recursive call to the next node (child)
-
-def classify(node, x_test, features):  # features: column headers
-    if node.answer != "":
+def classify(node,x_test,features): #features: column headers
+    if node.answer!="":      #this will be true only for leaf nodes(answer: yes/no)
         print(node.answer)
         return
-
-    pos = features.index(node.attribute)  # node.attribute will have the column header for that node
-
-    for value, n in node.children:  # for every value of that attribute
-        if x_test[pos] == value:  # for that particular value, go along the tree
-            classify(n, x_test, features)  # go deeper in the tree
-
-dataset, features = load_csv("traintennis.csv")
-node1 = build_tree(dataset, features)
-print("The decision tree for the dataset using ID3 algorithm is:")
-print_tree(node1, 0)
-
-testdata, features = load_csv("testtennis.csv")
-for xtest in testdata:  # xtest is each row in testdata
-    print("The test instance:", xtest)
-    print("The label for the test instance:", end=" ")
-    classify(node1, xtest, features)
-
-        
+    pos=features.index(node.attribute) #node.attribute will have the col header
+    for value, n in node.children:   #for every value of that attribute
+        if x_test[pos]==value:       # for that particular value go along that value
+            classify(n,x_test,features) #go deeper in the tree
+
+
+dataset,features=load_csv("traintennis.csv")
+#lastcol=[row[-1] for row in dataset]
+node1=build_tree(dataset,features)
+print("The decision tree for the dataset using ID3 algorithm is")
+print_tree(node1,0)
+
+testdata,features=load_csv("testtennis.csv")
+for xtest in testdata:   #xtest is each row in testdata
+    print("The test instance:",xtest)
+    print("The label for test instance:",end=" ")
+    classify(node1,xtest,features)
         
         ''')
     def m5(self):
         print('''
 import numpy as np
-
 X = np.array(([2, 9], [1, 5], [3, 6]), dtype=float)
 y = np.array(([92], [86], [89]), dtype=float)
+X = X/np.amax(X,axis=0) # maximum of X array longitudinally
+y = y/100
 
-X = X / np.amax(X, axis=0)  # maximum of X array longitudinally
-y = y / 100
+#Sigmoid Function
+def sigmoid (x):
+    return 1/(1 + np.exp(-x))
 
-# Sigmoid Function
-def sigmoid(x):
-    return 1 / (1 + np.exp(-x))
-
-# Derivative of Sigmoid Function
+#Derivative of Sigmoid Function
 def derivatives_sigmoid(x):
     return x * (1 - x)
 
-# Variable initialization
-epoch = 5000  # Setting training iterations
-lr = 0.1  # Setting learning rate
-inputlayer_neurons = 2  # number of features in the data set
-hiddenlayer_neurons = 3  # number of hidden layer neurons
-output_neurons = 1  # number of neurons at the output layer
-
-# Weight and bias initialization
-wh = np.random.uniform(size=(inputlayer_neurons, hiddenlayer_neurons))
-bh = np.random.uniform(size=(1, hiddenlayer_neurons))
-wout = np.random.uniform(size=(hiddenlayer_neurons, output_neurons))
-bout = np.random.uniform(size=(1, output_neurons))
+#Variable initialization
+epoch=5000 	#Setting training iterations
+lr=0.1 		#Setting learning rate
+inputlayer_neurons = 2 		#number of features in data set
+hiddenlayer_neurons = 3 	#number of hidden layers neurons
+output_neurons = 1 		#number of neurons at output layer
+
+#weight and bias initialization
+wh=np.random.uniform(size=(inputlayer_neurons,hiddenlayer_neurons))  #2,3
+bh=np.random.uniform(size=(1,hiddenlayer_neurons))                   #1,3
+wout=np.random.uniform(size=(hiddenlayer_neurons,output_neurons))    #3,1
+bout=np.random.uniform(size=(1,output_neurons))                      #1,1
 
 for i in range(epoch):
-    # Forward Propagation
-    hinp = np.dot(X, wh) + bh
-    hlayer_act = sigmoid(hinp)  # HIDDEN LAYER ACTIVATION FUNCTION
-    outinp = np.dot(hlayer_act, wout) + bout
+#Forward Propogation 
+    hinp=np.dot(X,wh)+ bh
+    hlayer_act = sigmoid(hinp)      #HIDDEN LAYER ACTIVATION FUNCTION
+    outinp=np.dot(hlayer_act,wout)+ bout
     output = sigmoid(outinp)
 
-    outgrad = derivatives_sigmoid(output)
+    outgrad = derivatives_sigmoid(output) 
     hiddengrad = derivatives_sigmoid(hlayer_act)
+    
+    EO = y-output                   #ERROR AT OUTPUT LAYER
+    d_output = EO* outgrad
 
-    EO = y - output  # ERROR AT OUTPUT LAYER
-    d_output = EO * outgrad
-    EH = d_output.dot(wout.T)  # ERROR AT HIDDEN LAYER (TRANSPOSE => CO
-
+    EH = d_output.dot(wout.T)       #ERROR AT HIDDEN LAYER (TRANSPOSE => COZ REVERSE(BACK))
     d_hiddenlayer = EH * hiddengrad
-    wout += hlayer_act.T.dot(d_output) * lr
-    wh += X.T.dot(d_hiddenlayer) * lr
 
-print("Input: \n" + str(X))
+    wout += hlayer_act.T.dot(d_output) *lr      #REMEMBER WOUT IS 3*1 MATRIX
+    wh += X.T.dot(d_hiddenlayer) *lr
+
+print("Input: \n" + str(X)) 
 print("Actual Output: \n" + str(y))
-print("Predicted Output: \n", output)
+print("Predicted Output: \n" ,output)
  
         
         
         ''')
     def m6(self):
         print('''
 import csv
 import random
 import math
 
 def loadcsv(filename):
-    dataset = list(csv.reader(open(filename, "r")))
+    dataset = list(csv.reader(open(filename,"r")))
     for i in range(len(dataset)):
         dataset[i] = [float(x) for x in dataset[i]]
     return dataset
 
 def splitDataset(dataset, splitRatio):
     trainSize = int(len(dataset) * splitRatio)
-    trainSet, testSet = dataset[:trainSize], dataset[trainSize:]
+    trainSet = []
+    trainSet,testSet = dataset[:trainSize],dataset[trainSize:]
     return [trainSet, testSet]
 
 def mean(numbers):
-    return sum(numbers) / len(numbers)
+    return sum(numbers)/(len(numbers))
 
 def stdev(numbers):
     avg = mean(numbers)
     v = 0
     for x in numbers:
-        v += (x - avg) ** 2
-    return math.sqrt(v / (len(numbers) - 1))
+        v += (x-avg)**2
+    return math.sqrt(v/(len(numbers)-1))
 
 def summarizeByClass(dataset):
     separated = {}
     for i in range(len(dataset)):
         vector = dataset[i]
-        if vector[-1] not in separated:
+        if (vector[-1] not in separated):
             separated[vector[-1]] = []
         separated[vector[-1]].append(vector)
-
     summaries = {}
     for classValue, instances in separated.items():
-        summaries[classValue] = [(mean(attribute), stdev(attribute)) for attribute in zip(*instances)]
+        summaries[classValue] = [(mean(attribute), stdev(attribute)) for attribute in zip(*instances)][:-1]
     return summaries
 
 def calculateProbability(x, mean, stdev):
-    exponent = math.exp((-(x - mean) ** 2) / (2 * (stdev ** 2)))
-    return (1 / (math.sqrt(2 * math.pi) * stdev)) * exponent
+    exponent = math.exp((-(x-mean)**2)/(2*(stdev**2)))
+    return (1 / math.sqrt(2*math.pi*(stdev**2))) * exponent
 
 def predict(summaries, inputVector):
     probabilities = {}
     for classValue, classSummaries in summaries.items():
         probabilities[classValue] = 1
         for i in range(len(classSummaries)):
             mean, stdev = classSummaries[i]
             x = inputVector[i]
             probabilities[classValue] *= calculateProbability(x, mean, stdev)
-
     bestLabel, bestProb = None, -1
     for classValue, probability in probabilities.items():
         if bestLabel is None or probability > bestProb:
             bestProb = probability
             bestLabel = classValue
-
     return bestLabel
 
 def getPredictions(summaries, testSet):
     predictions = []
     for i in range(len(testSet)):
         result = predict(summaries, testSet[i])
         predictions.append(result)
     return predictions
 
 def getAccuracy(testSet, predictions):
     correct = 0
     for i in range(len(testSet)):
         if testSet[i][-1] == predictions[i]:
             correct += 1
-    return (correct / len(testSet)) * 100.0
+    return (correct/(len(testSet))) * 100.0
 
-filename = '/home/nmit/Downloads/diabetes.csv'
+filename = 'diabetes2.csv'
 splitRatio = 0.9
 dataset = loadcsv(filename)
 actual = []
 trainingSet, testSet = splitDataset(dataset, splitRatio)
 for i in range(len(testSet)):
-    vector = testSet[i]
-    actual.append(vector[-1])
-
+	vector = testSet[i]
+	actual.append(vector[-1])
 print('Split {0} rows into train={1} and test={2} rows'.format(len(dataset), len(trainingSet), len(testSet)))
-summaries = summarizeByClass(trainingSet)  # will have (mean, sd) for all attributes
+summaries = summarizeByClass(trainingSet) #will have (mean,sd) for all attributes.(for class 1 & 0 separately)
 predictions = getPredictions(summaries, testSet)
-
-print('\nActual values:\n', actual)
-print("Predictions:\n", predictions)
+print('\nActual values:\n',actual)
+print("\nPredictions:\n",predictions)
 accuracy = getAccuracy(testSet, predictions)
-print("Accuracy:", accuracy)
-
-        
+print("Accuracy",accuracy)
         
         ''')
 
     def m7(self):
         print('''
         
+#import the dataset and library files
 from sklearn.datasets import load_iris
 from sklearn.neighbors import KNeighborsClassifier
 import numpy as np
 from sklearn.model_selection import train_test_split
 
-iris_dataset = load_iris()
+iris_dataset=load_iris()
 
-# Display the iris dataset
-print("\nIRIS FEATURES TARGET NAMES:")
+#display the iris dataset
+print("\n IRIS FEATURES \ TARGET NAMES: \n ", iris_dataset.target_names)
 for i in range(len(iris_dataset.target_names)):
-    print("[{0}]:[{1}]".format(i, iris_dataset.target_names[i]))
+    print("\n[{0}]:[{1}]".format(i,iris_dataset.target_names[i]))
 
-print("\nIRIS DATA:\n", iris_dataset["data"])
+print("\n IRIS DATA :\n",iris_dataset["data"])
 
-# Split the data into training and testing data
+#split the data into training and testing data
 X_train, X_test, y_train, y_test = train_test_split(iris_dataset["data"], iris_dataset["target"], random_state=0)
 
-print("\nX TRAIN:\n", X_train)
-print("\nX TEST:\n", X_test)
-print("\nY TRAIN:\n", y_train)
-print("\nY TEST:\n", y_test)
+print("\n Target :\n",iris_dataset["target"])
+#print("\n")
+#print(len(iris_dataset["target"]))
+print("\n X TRAIN \n", X_train)
+print("\n X TEST \n", X_test)
+print("\n Y TRAIN \n", y_train)
+print("\n Y TEST \n", y_test)
 
-# Train and fit the model
+#train and fit the model
 kn = KNeighborsClassifier(n_neighbors=5)
 kn.fit(X_train, y_train)
 
-# Predicting from the model
+#predicting from model
 x_new = np.array([[5, 2.9, 1, 0.2]])
-print("\nX NEW:\n", x_new)
-
+print("\n XNEW \n",x_new)
 prediction = kn.predict(x_new)
-print("\nPredicted target value: {}\n".format(prediction))
-print("\nPredicted feature name: {}\n".format(iris_dataset["target_names"][prediction]))
+print("\n Predicted target value: {}\n".format(prediction))
+print("\n Predicted feature name: {}\n".format(iris_dataset["target_names"][prediction]))
 
-for i in range(len(X_test)):
-    x = X_test[i]
-    x_new = np.array([x])
-    prediction = kn.predict(x_new)  # Predict method returns the label
-    print("Actual: {0}, Predicted: {1}".format(iris_dataset["target_names"][y_test[i]], iris_dataset["target_names"][prediction]))
-
-print("\nTEST SCORE (ACCURACY): {:.2f}\n".format(kn.score(X_test, y_test)))
+i=1
+x= X_test[i]
+x_new = np.array([x])
+print("\n XNEW \n",x_new)
 
-        
+for i in range(len(X_test)):
+  x = X_test[i]
+  x_new = np.array([x])
+  prediction = kn.predict(x_new)     #predict method returns label 
+  print("\n Actual : {0} {1}, Predicted :{2}{3}".format(y_test[i],iris_dataset["target_names"][y_test[i]],prediction,iris_dataset["target_names"][ prediction]))
+print("\n TEST SCORE[ACCURACY]: {:.2f}\n".format(kn.score(X_test, y_test)))
         ''')
     def m8(self):
         print('''
         import matplotlib.pyplot as plt
         from sklearn import datasets
         from sklearn.cluster import KMeans
         from sklearn.mixture import GaussianMixture
-        import sklearn.mixture as sm
+        import sklearn.metrics as sm
         import pandas as pd
         import numpy as np
+
         iris = datasets.load_iris()
-        x = pd.DataFrame(iris.data)
-        x.columns ={'sepal_length','sepal_width','Petal_length','Petal_width'}
-        y = pd.DataFrame(iris.target)
-        y.columns =['Target']
-        print(x)
-        print(y)
-        colormap = np.array(['red','line','black'])
+
+        X = pd.DataFrame(iris.data)
+        X.columns = ['Sepal_Length','Sepal_Width','Petal_Length', 'Petal_Width']
+        Y = pd.DataFrame(iris.target)
+        Y.columns = ['Targets']
+
+        print(X)
+        print(Y)
+        colormap = np.array(['red', 'lime', 'black'])
+
         plt.subplot(1,2,1)
-        plt.scatter(x.petal_length,x.petal_width,c=colormap[y.targets],s=40)
-        plt.title("Real clustering")
-        model1=KMeans(n_clusters=3)
-        model1.fit(x)
+        plt.scatter(X.Petal_Length, X.Petal_Width, c=colormap[Y.Targets],s=40)
+        plt.title('Real Clustering')
+
+        model1 = KMeans(n_clusters=3)
+        model1.fit(X)
+                    
         plt.subplot(1,2,2)
-        plt.scatter(x.petal_legth,x.petal_width,c=colormap[model1.labels_],s=40)
-        plt.title(' K mean clustering ')
+        plt.scatter(X.Petal_Length, X.Petal_Width,c=colormap[model1.labels_],s=40)
+        plt.title('K Mean Clustering')
         plt.show()
-        model2=GaussianMixture(n_components=3)
-        model2.fit(x)
+
+        model2 = GaussianMixture(n_components=3)
+        model2.fit(X)
+
         plt.subplot(1,2,1)
-        plt.scatter(x.petal_length,x.petal_width,c=colormap[model2.predict(x)],s=40)
-        plt.title('EM clustering')
+        plt.scatter(X.Petal_Length, X.Petal_Width, c=colormap[model2.predict(X)],s=40) 
+        plt.title('EM Clustering')
         plt.show()
-        print("Actual Target is : \n " , iris.target)
-        print("K means: \n ",model1.labels_)
-        print(" EM : \n ",model2.predict(x))
-        print("Accuracy of KMeans is " ,sm.accuracy_score(y,model1.label_))
-        print("Accuracy of EM is ",sm.accuracy_score(y,model2.predict(x)))
+
+        print("Actual Target is:\n", iris.target)
+        print("K Means:\n",model1.labels_)
+        print("EM:\n",model2.predict(X))
+        print("Accuracy of KMeans is ",sm.accuracy_score(Y,model1.labels_))
+        print("Accuracy of EM is ",sm.accuracy_score(Y, model2.predict(X)))
         ''')
```

