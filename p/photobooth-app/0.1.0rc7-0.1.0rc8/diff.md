# Comparing `tmp/photobooth_app-0.1.0rc7.tar.gz` & `tmp/photobooth_app-0.1.0rc8.tar.gz`

## Comparing `photobooth_app-0.1.0rc7.tar` & `photobooth_app-0.1.0rc8.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/__main__.py
--rw-r--r--   0        0        0    19560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/appconfig.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/application.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/containers.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/config.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/debug.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/home.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/containers.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/gpioservice.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/shareservice.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/wledservice.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/index.html
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/272.0be6c807.css
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/706.5484da7d.css
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/835.ded66ce0.css
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-notext-black-transparent.png
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-black-transparent.png
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-white-transparent.png
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/247.74c0e45d.js
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/272.a73245eb.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/429.76096bfa.js
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/706.98593961.js
--rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/835.8e1bdcfb.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/931.55b1be58.js
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/954.7419ae78.js
--rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/app.979a8c9e.js
--rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/LICENSE.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/__main__.py
+-rw-r--r--   0        0        0    19399 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/config.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/debug.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/home.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/containers.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/gpioservice.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/shareservice.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    30982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/272.0be6c807.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/706.5484da7d.css
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/835.ded66ce0.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-notext-black-transparent.png
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-black-transparent.png
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-white-transparent.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/247.74c0e45d.js
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/272.a73245eb.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/429.76096bfa.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/706.98593961.js
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/835.8e1bdcfb.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/931.55b1be58.js
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/954.7419ae78.js
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/app.979a8c9e.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/LICENSE.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/README.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/pyproject.toml
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/PKG-INFO
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/__main__.py` & `photobooth_app-0.1.0rc8/photobooth/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
     # use to construct paths in app referring to assets
     logger.info(f"photobooth directory: {Path(__file__).parent.resolve()}")
     # use to construct paths to user data
     logger.info(f"working directory: {Path.cwd().resolve()}")
     # __version__ = importlib.metadata.version("photobooth-app")
     # logger.info(f"{__version__=}")
 
-    application_container.init_resources()
     application_container.wire(modules=[__name__], packages=[".routers"])
+    application_container.init_resources()
 
     # start main application
     server = _server()
 
     # serve, loops endless
     # this one is not executed in tests because it's not stoppable from within
     if run_server:
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/appconfig.py` & `photobooth_app-0.1.0rc8/photobooth/appconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any
 
 import jsonref
-from pydantic import BaseModel, ConfigDict, Extra, Field, PrivateAttr
+from pydantic import BaseModel, ConfigDict, Field, PrivateAttr
 from pydantic.fields import FieldInfo
 from pydantic_extra_types.color import Color
 from pydantic_settings import (
     BaseSettings,
     PydanticBaseSettingsSource,
     SettingsConfigDict,
 )
@@ -146,20 +146,20 @@
         description="IP/Hostname to bind the webserver to. 0.0.0.0 means bind to all IP adresses of host.",
     )
     webserver_port: int = Field(
         default=8000,
         description="Port to serve the photobooth website. Ensure the port is available.",
     )
 
-    shareservice_enable: bool = Field(
+    shareservice_enabled: bool = Field(
         default=False,
         description="Enable share service. To enable URL needs to be configured and dl.php script setup properly.",
     )
     shareservice_url: str = Field(
-        default="https://dl.qbooth.net/dl.php",
+        default="https://explain-shareservice.photobooth-app.de/dl.php",
         description="URL of php script that is used to serve files and share via QR code.",
     )
     shareservice_apikey: str = Field(
         default="changedefault!",
         description="Key to secure the download php script. Set the key in dl.php script to same value. Only if correct key is provided the shareservice works properly.",
     )
     shareservice_share_original: bool = Field(
@@ -397,15 +397,15 @@
 
     model_config = ConfigDict(title="Personalize the User Interface")
 
     FRONTPAGE_TEXT: str = Field(
         default='<div class="fixed-center text-h2 text-weight-bold text-center text-white" style="text-shadow: 4px 4px 4px #666;">Hey!<br>Let\'s take some pictures <br>📷💕</div>',
         description="Text/HTML displayed on frontpage.",
     )
-    GALLERY_ENABLE: bool = Field(
+    GALLERY_ENABLED: bool = Field(
         default=True,
         description="Enable gallery for user.",
     )
     GALLERY_EMPTY_MSG: str = Field(
         default="So boring here...🤷‍♂️<br>Let's take some pictures 📷💕",
         description="Message displayed if gallery is empty.",
     )
@@ -421,18 +421,14 @@
         default=30,
         description="Timeout in seconds a new item popup closes automatically.",
     )
     SHOW_ADMIN_LINK_ON_FRONTPAGE: bool = Field(
         default=True,
         description="Show link to admin center, usually only during setup.",
     )
-    EXT_DOWNLOAD_URL: str = Field(
-        default="http://dl.qbooth.net/{filename}",
-        description="URL encoded by QR code to download images from onlineservice. {filename} is replaced by actual filename",
-    )
     gallery_show_filter: bool = Field(
         default=True,
         description="",
     )
     gallery_filter_userselectable: list[EnumPilgramFilter] = Field(
         title="Pic1 Filter Userselectable",
         default=[EnumPilgramFilter.original, EnumPilgramFilter.clarendon, EnumPilgramFilter.moon],
@@ -521,18 +517,18 @@
     misc: GroupMisc = GroupMisc()
 
     # TODO[pydantic]: We couldn't refactor this class, please create the `model_config` manually.
     # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
     model_config = SettingsConfigDict(
         env_file_encoding="utf-8",
         # first in following list is least important; last .env file overwrites the other.
-        env_file=[".env.installer", ".env.dev", ".env.prod"],
+        env_file=[".env.installer", ".env.dev", ".env.test", ".env.prod"],
         env_nested_delimiter="__",
         case_sensitive=True,
-        extra=Extra.ignore,
+        extra="ignore",
     )
 
     @classmethod
     def settings_customise_sources(
         cls,
         settings_cls: type[BaseSettings],
         init_settings: PydanticBaseSettingsSource,
@@ -540,14 +536,15 @@
         dotenv_settings: PydanticBaseSettingsSource,
         file_secret_settings: PydanticBaseSettingsSource,
     ) -> tuple[PydanticBaseSettingsSource, ...]:
         """customize sources"""
         return (
             init_settings,
             JsonConfigSettingsSource(settings_cls),
+            dotenv_settings,
             env_settings,
             file_secret_settings,
         )
 
     def get_schema(self, schema_type: str = "default"):
         """Get schema to build UI. Schema is polished to the needs of UI"""
         if schema_type == "dereferenced":
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/application.py` & `photobooth_app-0.1.0rc8/photobooth/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,30 +27,34 @@
 FASTAPI_DECRIPTION = """
 Photobooth App 🚀
 
 The photobooth app is written in Python and coming along with a modern Vue frontend.
 
 Following api is provided by the app.
 
-## Work in progress, API may change any time.
+## API may change any time.
 
 """
 
 
 def _create_basic_folders():
     os.makedirs("data", exist_ok=True)
     os.makedirs("log", exist_ok=True)
     os.makedirs("config", exist_ok=True)
 
 
 def _create_app() -> FastAPI:
     application_container = ApplicationContainer()
     logger = logging.getLogger(f"{__name__}")
 
-    _create_basic_folders()
+    try:
+        _create_basic_folders()
+    except Exception as exc:
+        logger.critical(f"cannot create data folders, error: {exc}")
+        raise RuntimeError(f"cannot create data folders, error: {exc}") from exc
 
     _app = FastAPI(
         title="Photobooth App API",
         description=FASTAPI_DECRIPTION,
         version="0.0.1",
         contact={
             "name": "mgrl",
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/containers.py` & `photobooth_app-0.1.0rc8/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc8/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/config.py` & `photobooth_app-0.1.0rc8/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/debug.py` & `photobooth_app-0.1.0rc8/photobooth/routers/debug.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/home.py` & `photobooth_app-0.1.0rc8/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc8/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc8/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc8/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc8/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/routers/system.py` & `photobooth_app-0.1.0rc8/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/baseservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/baseservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/containers.py` & `photobooth_app-0.1.0rc8/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/gpioservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/gpioservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/loggingservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,67 +69,63 @@
         """Setup logger
 
         Args:
             evtbus (EventEmitter): _description_
         """
         super().__init__(evtbus=evtbus, config=config)
 
-        self.debug_level = config.common.DEBUG_LEVEL.value
-
         ## formatter ##
         fmt = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
         log_formatter = logging.Formatter(fmt=fmt)
 
-        logging.basicConfig(level=logging.DEBUG, format=fmt, force=True)
+        ## basic configuration
+        # latest basicConfig adds a streamHandler output to console if not automatically called
+        # earlier by some .warn .info or other
+        # force=False because otherwise the pytest console logger stream handler gets deleted
+        logging.basicConfig(level=logging.DEBUG, format=fmt, force=False)
+        logging.debug("loggingservice __init__ basicConfig set")
+        logging.debug("loggingservice __init__ started")
 
-        ## logger ##
+        self.debug_level = config.common.DEBUG_LEVEL.value
 
+        ## logger
         # default logger (root = None or "")
         # root logger also to be the template for all other loggers,
         # that are created in the app at a later time during run
         root_logger = logging.getLogger(name=None)
-        # Remove all handlers associated with the root logger object.
-        for handler in logging.root.handlers[:]:
-            logging.root.removeHandler(handler)
 
         # set level based on users config
         root_logger.setLevel(self.debug_level)
 
-        ## handler ##
-
-        # create console handler
-        self.console_handler = logging.StreamHandler()
-        self.console_handler.setFormatter(log_formatter)
-
+        ## handler
         # create rotatingFileHandler
         self.rotatingfile_handler = RotatingFileHandler(
             filename="./log/qbooth.log", maxBytes=1024**2, backupCount=10, delay=True, encoding="utf-8"
         )
         self.rotatingfile_handler.setFormatter(log_formatter)
 
         # create rotatingFileHandler
         self.eventstream_handler = EventstreamLogHandler(evtbus=evtbus)
         self.eventstream_handler.setFormatter(log_formatter)
 
         ## wire logger and handler ##
-
-        root_logger.addHandler(self.console_handler)
         root_logger.addHandler(self.rotatingfile_handler)
         root_logger.addHandler(self.eventstream_handler)
 
-        # loggers_defined = [logging.getLogger(name)
-        #                   for name in logging.root.manager.loggerDict]
-        # print(loggers_defined)
-
+        ## mute other loggers
         self.other_loggers()
 
+        ## add the exepthooks
         sys.excepthook = self._handle_sys_exception
         threading.excepthook = self._handle_threading_exception
         # no solution to handle exceptions in sep processes yet...
 
+        logging.debug("loggingservice __init__ finished")
+        logging.debug(f"registered handlers: {logging.root.handlers}")
+
     def other_loggers(self):
         """mute some logger by rasing their log level"""
 
         for name in [
             "picamera2.picamera2",
             "sse_starlette.sse",
             "PIL.PngImagePlugin",
@@ -159,15 +155,14 @@
         ]:
             lgr = logging.getLogger(name=name)
             lgr.setLevel(self.debug_level)
             lgr.propagate = False
             lgr.handlers = [
                 self.rotatingfile_handler,
                 self.eventstream_handler,
-                self.console_handler,
             ]
 
     @staticmethod
     def _handle_sys_exception(exc_type, exc_value, exc_traceback):
         if issubclass(exc_type, KeyboardInterrupt):
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
             return
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/mediacollectionservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,20 @@
         """count number of items in db
 
         Returns:
             int: Number of items in db
         """
         return len(self._db)
 
-    def db_get_images(self) -> dict:
+    def db_get_images(self) -> list:
         """Get dict of mediaitems. Most recent item is at index 0.
 
 
         Returns:
-            dict: _description_
+            list: _description_
         """
         return [item.asdict() for item in self._db]
 
     def db_get_image_by_id(self, item_id):
         """_summary_
 
         Args:
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/processingservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,52 +80,58 @@
 
         # register to send initial data SSE
         self._evtbus.on("publishSSE/initial", self._sse_initial_processinfo)
 
     # general on_ events
     def before_transition(self, event, state):
         """_summary_"""
-        logger.info(f"Before '{event}', on the '{state.id}' state.")
+        pass
+        # logger.info(f"Before '{event}', on the '{state.id}' state.")
 
     def on_transition(self, event, state):
         """_summary_"""
-        logger.info(f"On '{event}', on the '{state.id}' state.")
+        pass
+        # logger.info(f"On '{event}', on the '{state.id}' state.")
 
     def on_exit_state(self, event, state):
         """_summary_"""
-        logger.info(f"Exiting '{state.id}' state from '{event}' event.")
+        pass
+        # logger.info(f"Exiting '{state.id}' state from '{event}' event.")
 
     def on_enter_state(self, event, state):
         """_summary_"""
-        logger.info(f"Entering '{state.id}' state from '{event}' event.")
-        logger.info(f"current state '{self.current_state.id}' ")
+        # logger.info(f"Entering '{state.id}' state from '{event}' event.")
+        logger.info(f"on_enter_state '{self.current_state.id=}' ")
 
         # always send current state on enter so UI can react (display texts, wait message on postproc, ...)
         self._sse_processinfo(
             __class__.Stateinfo(
                 state=self.current_state.id,
                 countdown=self.timer_countdown,
             )
         )
 
     def after_transition(self, event, state):
         """_summary_"""
-        logger.info(f"After '{event}', on the '{state.id}' state.")
+        pass
+        # logger.info(f"After '{event}', on the '{state.id}' state.")
 
     ## specific on_ transition actions:
 
     def on_thrill(self):
         """_summary_"""
+        logger.info("on_thrill")
         self._evtbus.emit("statemachine/on_thrill")
 
     def on_shoot(self):
         """_summary_"""
 
     def on_enter_postprocess_still(self):
         # create JPGs and add to db
+        logger.info("on_enter_postprocess_still")
 
         # TODO: collage: separate postprocessing step 2 mount collage and create a new original.
 
         # create mediaitem for further processing
         mediaitem = MediaItem(os.path.basename(self._filepath_originalimage_processing))
 
         # always create unprocessed versions for later usage
@@ -150,19 +156,21 @@
             sse_data=json.dumps(mediaitem.asdict()),
         )
 
     ## specific on_state actions:
 
     def on_enter_idle(self):
         """_summary_"""
+        logger.info("on_enter_idle")
         # always remove old reference
         self._filepath_originalimage_processing = None
 
     def on_enter_counting(self):
         """_summary_"""
+        logger.info("on_enter_counting")
         self.timer_countdown = (
             self._config.common.PROCESS_COUNTDOWN_TIMER + self._config.common.PROCESS_COUNTDOWN_OFFSET
         )
         logger.info(f"loaded timer_countdown='{self.timer_countdown}'")
         logger.info("starting timer")
 
         while self.timer_countdown > 0:
@@ -175,18 +183,20 @@
             time.sleep(0.1)
             self.timer_countdown -= 0.1
 
             if self.timer_countdown <= self._config.common.PROCESS_COUNTDOWN_OFFSET and self.counting.is_active:
                 return
 
     def on_exit_counting(self):
+        logger.info("on_exit_counting")
         self.timer_countdown = 0
 
     def on_enter_capture_still(self):
         """_summary_"""
+        logger.info("on_enter_capture_still")
         self._evtbus.emit("statemachine/on_enter_capture_still")
 
         filepath_neworiginalfile = get_new_filename(type=MediaItemTypes.IMAGE)
         logger.debug(f"capture to {filepath_neworiginalfile=}")
 
         start_time_capture = time.time()
 
@@ -220,14 +230,15 @@
             logger.critical(f"finally failed after {MAX_ATTEMPTS} attempts to capture image!")
             raise RuntimeError(f"finally failed after {MAX_ATTEMPTS} attempts to capture image!")
 
         logger.info(f"-- process time: {round((time.time() - start_time_capture), 2)}s to capture still")
 
     def on_exit_capture_still(self):
         """_summary_"""
+        logger.info("on_exit_capture_still")
         self._evtbus.emit("statemachine/on_exit_capture_still")
 
     ### some external functions
 
     def evt_chose_1pic_get(self):
         logger.info("evt_chose_1pic_get called to take picture")
         if not self.idle.is_active:
@@ -240,15 +251,14 @@
             self.postprocess()
             self.finalize()
         except Exception as exc:
             logger.critical(f"something went wrong :( {exc}")
             self._reset()
             raise RuntimeError(f"something went wrong :( {exc}") from exc
 
-
     ### some custom helper
 
     def _sse_initial_processinfo(self):
         """_summary_"""
         self._sse_processinfo(__class__.Stateinfo(state=self.current_state.id))
 
     def _sse_processinfo(self, sse_data: Stateinfo):
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/shareservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/shareservice.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,111 +30,133 @@
 
         self._logger.info("initialized share service")
 
     def _initialize(self):
         self._initialized = False
 
         self._logger.info("checking shareservice api endpoint")
-        r = requests.get(self._config.common.shareservice_url, params={"action": "info"})
-        if r.status_code == 200:
-            try:
-                info = r.json()
-                self._logger.info(f"{info=}")
-            except requests.exceptions.JSONDecodeError as exc:
-                self._logger.error(f"api endpoint error: {exc}")
-
-            self._initialized = True
-            self._logger.info("api endpoint found, URL valid")
+        try:
+            r = requests.get(self._config.common.shareservice_url, params={"action": "info"}, timeout=10)
+        except Exception as exc:
+            self._logger.warning(f"error checking shareservice api endpoint: {exc}")
         else:
-            self._logger.error("api endpoint check failed")
+            if r.status_code == 200:
+                try:
+                    info = r.json()
+                    self._logger.info(f"{info=}")
+                except requests.exceptions.JSONDecodeError as exc:
+                    self._logger.error(f"api endpoint error: {exc}")
+
+                self._initialized = True
+                self._logger.info("api endpoint found, URL valid")
+            else:
+                self._logger.error("api endpoint check failed")
 
     def start(self):
         """_summary_"""
-        if not self._config.common.shareservice_enable:
+        if not self._config.common.shareservice_enabled:
             self._logger.info("shareservice disabled, start aborted.")
             return
         self._initialize()
         if self._initialized:
             self._worker_thread.start()
+
+            # short sleep until workerthread is started and likely to be connected to service or failed.
+            time.sleep(1)
+
+            self._logger.debug(f"{self.__module__} started")
         else:
             self._logger.error("shareservice init was not successful. start service aborted.")
 
     def stop(self):
         """_summary_"""
         self._worker_thread.stop()
         if self._worker_thread.is_alive():
             self._worker_thread.join()
 
     def _worker_fun(self):
         # init
-        # nothing here yet
+        self._logger.info("starting shareservice worker_thread")
 
         while not self._worker_thread.stopped():
             payload = {"action": "upload_queue"}
-            r = requests.get(self._config.common.shareservice_url, params=payload, stream=True, timeout=60)
+            r = requests.get(self._config.common.shareservice_url, params=payload, stream=True, timeout=8)
             if r.encoding is None:
                 r.encoding = "utf-8"
 
-            iterator = r.iter_lines(decode_unicode=True)
+            if r.status_code == 200:
+                self._logger.info("successfully connected to shareservice dl.php script")
+            else:
+                self._logger.error("problem connecting to shareservice dl.php script!")
+
+            iterator = r.iter_lines(chunk_size=24, decode_unicode=True)
 
             while not self._worker_thread.stopped():
                 try:
                     line = next(iterator)
+                except StopIteration:
+                    self._logger.debug("dl.php script finished after some time. stopiteration issued-reconnect")
+                    break
                 except Exception as exc:
-                    print(exc)
                     self._logger.warning(f"encountered shareservice connection issue. retrying. error: {exc}")
                     break
 
                 # filter out keep-alive new lines
                 if line:
-                    job = json.loads(line)
+                    decoded_line = json.loads(line)
 
-                    if job.get("file_identifier", None) and job.get("status", None):
+                    if decoded_line.get("file_identifier", None) and decoded_line.get("status", None):
                         # valid job check whether pending and upload
-                        self._logger.info(f"got share upload job, {job}")
+                        self._logger.info(f"got share upload job, {decoded_line}")
 
                         # set the file to be uploaded
+                        request_upload_file = {}
                         try:
                             mediaitem_to_upload = self._mediacollection_service.db_get_image_by_id(
-                                job["file_identifier"]
+                                decoded_line["file_identifier"]
                             )
+                            self._logger.info(f"found mediaitem to upload: {mediaitem_to_upload}")
                         except FileNotFoundError as exc:
                             self._logger.error(f"mediaitem not found, wrong id? {exc}")
                             self._logger.info("sending upload request to dl.php anyway to signal failure")
-                            request_upload_file = {}
                         else:
-                            self._logger.info(f"found mediaitem to upload: {mediaitem_to_upload}")
+                            self._logger.info(f"mediaitem to upload: {mediaitem_to_upload}")
                             if self._config.common.shareservice_share_original:
                                 filepath_to_upload = mediaitem_to_upload.path_original
                             else:
                                 filepath_to_upload = mediaitem_to_upload.path_full
+
                             self._logger.debug(f"{filepath_to_upload=}")
 
                             request_upload_file = {"upload_file": open(filepath_to_upload, "rb")}
-                        finally:
-                            start_time = time.time()
-
-                            r = requests.post(
-                                self._config.common.shareservice_url,
-                                files=request_upload_file,
-                                params={
-                                    "action": "upload",
-                                    "apikey": self._config.common.shareservice_apikey,
-                                    "id": job["file_identifier"],
-                                },
-                            )
 
-                            self._logger.debug(f"response from php server: {r.text}")
-                            self._logger.debug(f"-- request took: {round((time.time() - start_time), 2)}s")
+                        ## send request
+                        start_time = time.time()
 
+                        r = requests.post(
+                            self._config.common.shareservice_url,
+                            files=request_upload_file,
+                            data={
+                                "action": "upload",
+                                "apikey": self._config.common.shareservice_apikey,
+                                "id": decoded_line["file_identifier"],
+                            },
+                        )
+
+                        self._logger.debug(f"response from dl.php script: {r.text}")
+                        self._logger.debug(f"-- request took: {round((time.time() - start_time), 2)}s")
+                    elif decoded_line.get("ping", None):
+                        pass
                     else:
                         self._logger.error(f"invalid queue line, ignore: {line}")
-                else:
-                    # if a keepalive message is issued, we can check here also regularly for exit condition set
-                    if self._worker_thread.stopped():
-                        self._logger.debug("stop workerthread requested")
-                        break
+
+                # if a keepalive message is issued, we can check here also regularly for exit condition set
+                if self._worker_thread.stopped():
+                    self._logger.debug("stop workerthread requested")
+                    break
 
             self._logger.info("request timed out, error occured or shutdown requested")
             if not self._worker_thread.stopped():
-                self._logger.info("restarting loop after 5 seconds")
-                time.sleep(5)
+                self._logger.info("restarting loop wait 1 second")
+                time.sleep(1)
+
+        self._logger.info("leaving shareservice workerthread")
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc8/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/simulated.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Simulated backend for testing.
 """
+import glob
 import logging
+import random
 import time
 from datetime import datetime
 from io import BytesIO
 from multiprocessing import Condition, Event, Lock, Process, shared_memory
 from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
@@ -95,21 +97,22 @@
 
         logger.debug(f"{self.__module__} stopped")
 
     def wait_for_hq_image(self):
         """for other threads to receive a hq JPEG image"""
         self._evtbus.emit("frameserver/onCapture")
 
-        # get img off the producing queue
-        with self._condition_img_buffer_ready:
-            if not self._condition_img_buffer_ready.wait(timeout=4):
-                raise TimeoutError("timeout receiving frames")
+        hq_images = glob.glob(
+            f'{Path(__file__).parent.joinpath("assets", "backend_simulated", "hq_img").resolve()}/*.jpg'
+        )
+        current_hq_image_index = random.randint(0, len(hq_images) - 1)
 
-            with self._img_buffer_lock:
-                img = decompile_buffer(self._img_buffer_shm)
+        # get img off the producing queue
+        logger.info(f"provide {hq_images[current_hq_image_index]} as hq_image")
+        img = open(hq_images[current_hq_image_index], "rb").read()
 
         # virtual delay for camera to create picture
         time.sleep(0.1)
 
         self._evtbus.emit("frameserver/onCaptureFinished")
 
         # return to previewmode
@@ -195,24 +198,28 @@
             (25, 130),
             datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f"),
             fill=text_fill,
             font=font_large,
         )
         img_draw.text((25, 160), f"framerate: {fps}", fill=text_fill, font=font_small)
         img_draw.text(
-            (25, 340),
+            (25, 400),
             "you see this, so installation was successful :)",
             fill=text_fill,
             font=font_small,
         )
 
         # create jpeg
         jpeg_buffer = BytesIO()
         img.save(jpeg_buffer, format="jpeg", quality=90)
 
         # put jpeg on queue until full. If full this function blocks until queue empty
         with _img_buffer_lock:
-            compile_buffer(shm, jpeg_buffer.getvalue())
+            jpeg_bytes = jpeg_buffer.getvalue()
+            if len(jpeg_bytes) >= SHARED_MEMORY_BUFFER_BYTES:
+                raise RuntimeError("shared memory too small!")
+
+            compile_buffer(shm, jpeg_bytes)
 
         with _condition_img_buffer_ready:
             # wait to be notified
             _condition_img_buffer_ready.notify_all()
```

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc8/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc8/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc8/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc8/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc8/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc8/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc8/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-notext-black-transparent.png` & `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-notext-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-black-transparent.png` & `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-white-transparent.png` & `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-white-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/247.74c0e45d.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/247.74c0e45d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/272.a73245eb.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/272.a73245eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/429.76096bfa.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/429.76096bfa.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/706.98593961.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/706.98593961.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/835.8e1bdcfb.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/835.8e1bdcfb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/931.55b1be58.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/931.55b1be58.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/954.7419ae78.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/954.7419ae78.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/app.979a8c9e.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/app.979a8c9e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc8/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/LICENSE.md` & `photobooth_app-0.1.0rc8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc7/README.md` & `photobooth_app-0.1.0rc8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Written in Python 🐍, coming along with a modern Vue frontend.
 
 ![python versions supported 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/photobooth-app)
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
-[![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
+[![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/main/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
 **[Installation](https://mgrl.github.io/photobooth-docs/installation/)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)** - **[PyPI package](https://pypi.org/project/photobooth-app/)** - **[3d printed box](https://mgrl.github.io/photobooth-docs/photobox3dprint/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
```

### Comparing `photobooth_app-0.1.0rc7/PKG-INFO` & `photobooth_app-0.1.0rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0rc7
-Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
+Version: 0.1.0rc8
+Summary: Photobooth app written in Python supporting DSLR, picamera2 and webcameras
 Project-URL: homepage, https://github.com/mgrl/photobooth-app
 Project-URL: repository, https://github.com/mgrl/photobooth-app
 Project-URL: documentation, https://mgrl.github.io/photobooth-docs
 Author-email: Michael G <me@mgrl.de>
 Maintainer-email: Michael G <me@mgrl.de>
+License-Expression: MIT
 License-File: LICENSE.md
 Keywords: camera,dslr,filter,gphoto2,photobooth,picamera2,python,raspberry-pi
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.9
 Requires-Dist: dependency-injector~=4.41.0
 Requires-Dist: fastapi<0.101.0,>=0.100.0
-Requires-Dist: gphoto2<=2.3.4; platform_system == 'Linux'
+Requires-Dist: gphoto2~=2.3.6; platform_system == 'Linux'
 Requires-Dist: gpiozero~=1.6.2
 Requires-Dist: jsonref~=1.1.0
 Requires-Dist: opencv-python<4.9,>=4.7
 Requires-Dist: piexif~=1.1.3
 Requires-Dist: pilgram2~=2.0.2
 Requires-Dist: pillow<10.1,>=9.5
 Requires-Dist: psutil~=5.9.5
@@ -35,27 +36,27 @@
 Requires-Dist: pymitter~=0.4.0
 Requires-Dist: pyserial~=3.5
 Requires-Dist: python-dotenv~=1.0.0
 Requires-Dist: python-statemachine<2.2,>=2.0
 Requires-Dist: pyturbojpeg~=1.7.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: sse-starlette~=1.6.1
-Requires-Dist: uvicorn~=0.22.0
+Requires-Dist: uvicorn<0.24,>=0.22
 Requires-Dist: v4l2py~=0.6.2; platform_system == 'Linux'
 Description-Content-Type: text/markdown
 
 # ![photobooth-app logo](https://raw.githubusercontent.com/mgrl/photobooth-app/main/assets/logo/logo-text-black-transparent.png)
 
 Written in Python 🐍, coming along with a modern Vue frontend.
 
 ![python versions supported 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/photobooth-app)
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
-[![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
+[![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/main/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
 **[Installation](https://mgrl.github.io/photobooth-docs/installation/)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)** - **[PyPI package](https://pypi.org/project/photobooth-app/)** - **[3d printed box](https://mgrl.github.io/photobooth-docs/photobox3dprint/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
```

