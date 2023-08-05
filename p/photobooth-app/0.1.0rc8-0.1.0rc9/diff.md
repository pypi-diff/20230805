# Comparing `tmp/photobooth_app-0.1.0rc8.tar.gz` & `tmp/photobooth_app-0.1.0rc9.tar.gz`

## Comparing `photobooth_app-0.1.0rc8.tar` & `photobooth_app-0.1.0rc9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/__main__.py
--rw-r--r--   0        0        0    19399 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/appconfig.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/application.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/containers.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/config.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/debug.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/home.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/containers.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/gpioservice.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/shareservice.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/wledservice.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0    30982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/index.html
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/272.0be6c807.css
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/706.5484da7d.css
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/835.ded66ce0.css
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-notext-black-transparent.png
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-black-transparent.png
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-white-transparent.png
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/247.74c0e45d.js
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/272.a73245eb.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/429.76096bfa.js
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/706.98593961.js
--rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/835.8e1bdcfb.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/931.55b1be58.js
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/954.7419ae78.js
--rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/app.979a8c9e.js
--rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/LICENSE.md
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/README.md
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/pyproject.toml
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc8/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/__main__.py
+-rw-r--r--   0        0        0    19399 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/config.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/debug.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/home.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/containers.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/gpioservice.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/shareservice.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    30982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/css/272.0be6c807.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/css/706.5484da7d.css
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/css/835.ded66ce0.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-notext-black-transparent.png
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-text-black-transparent.png
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-text-white-transparent.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/247.74c0e45d.js
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/272.a73245eb.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/429.76096bfa.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/706.98593961.js
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/835.8e1bdcfb.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/931.55b1be58.js
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/954.7419ae78.js
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/app.979a8c9e.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/LICENSE.md
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/README.md
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc9/PKG-INFO
```

### Comparing `photobooth_app-0.1.0rc8/photobooth/__main__.py` & `photobooth_app-0.1.0rc9/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/appconfig.py` & `photobooth_app-0.1.0rc9/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/application.py` & `photobooth_app-0.1.0rc9/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/containers.py` & `photobooth_app-0.1.0rc9/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc9/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/config.py` & `photobooth_app-0.1.0rc9/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/debug.py` & `photobooth_app-0.1.0rc9/photobooth/routers/debug.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/home.py` & `photobooth_app-0.1.0rc9/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc9/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc9/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc9/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc9/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/routers/system.py` & `photobooth_app-0.1.0rc9/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/baseservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/baseservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/containers.py` & `photobooth_app-0.1.0rc9/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/gpioservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/gpioservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/shareservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/shareservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         self._mediacollection_service: MediacollectionService = mediacollection_service
         self._initialized: bool = False
         self._worker_thread = StoppableThread(name="_shareservice_worker", target=self._worker_fun, daemon=True)
 
         # registered events
         # self._evtbus.on("publishSSE/initial", self._on_stats_interval_timer)
 
-        self._logger.info("initialized share service")
-
     def _initialize(self):
         self._initialized = False
 
         self._logger.info("checking shareservice api endpoint")
         try:
-            r = requests.get(self._config.common.shareservice_url, params={"action": "info"}, timeout=10)
+            r = requests.get(
+                self._config.common.shareservice_url, params={"action": "info"}, timeout=10, allow_redirects=False
+            )
         except Exception as exc:
             self._logger.warning(f"error checking shareservice api endpoint: {exc}")
         else:
             if r.status_code == 200:
                 try:
                     info = r.json()
                     self._logger.info(f"{info=}")
@@ -59,15 +59,15 @@
         self._initialize()
         if self._initialized:
             self._worker_thread.start()
 
             # short sleep until workerthread is started and likely to be connected to service or failed.
             time.sleep(1)
 
-            self._logger.debug(f"{self.__module__} started")
+            self._logger.debug(f"{self.__module__} initialized and started")
         else:
             self._logger.error("shareservice init was not successful. start service aborted.")
 
     def stop(self):
         """_summary_"""
         self._worker_thread.stop()
         if self._worker_thread.is_alive():
@@ -75,15 +75,17 @@
 
     def _worker_fun(self):
         # init
         self._logger.info("starting shareservice worker_thread")
 
         while not self._worker_thread.stopped():
             payload = {"action": "upload_queue"}
-            r = requests.get(self._config.common.shareservice_url, params=payload, stream=True, timeout=8)
+            r = requests.get(
+                self._config.common.shareservice_url, params=payload, stream=True, timeout=8, allow_redirects=False
+            )
             if r.encoding is None:
                 r.encoding = "utf-8"
 
             if r.status_code == 200:
                 self._logger.info("successfully connected to shareservice dl.php script")
             else:
                 self._logger.error("problem connecting to shareservice dl.php script!")
@@ -128,26 +130,33 @@
                             self._logger.debug(f"{filepath_to_upload=}")
 
                             request_upload_file = {"upload_file": open(filepath_to_upload, "rb")}
 
                         ## send request
                         start_time = time.time()
 
-                        r = requests.post(
-                            self._config.common.shareservice_url,
-                            files=request_upload_file,
-                            data={
-                                "action": "upload",
-                                "apikey": self._config.common.shareservice_apikey,
-                                "id": decoded_line["file_identifier"],
-                            },
-                        )
+                        try:
+                            r = requests.post(
+                                self._config.common.shareservice_url,
+                                files=request_upload_file,
+                                data={
+                                    "action": "upload",
+                                    "apikey": self._config.common.shareservice_apikey,
+                                    "id": decoded_line["file_identifier"],
+                                },
+                                timeout=9,
+                                allow_redirects=False,
+                            )
+                        except Exception as exc:
+                            self._logger.warning(f"upload failed, err: {exc}")
+                            # try again?
 
-                        self._logger.debug(f"response from dl.php script: {r.text}")
-                        self._logger.debug(f"-- request took: {round((time.time() - start_time), 2)}s")
+                        else:
+                            self._logger.debug(f"response from dl.php script: {r.text}")
+                            self._logger.debug(f"-- request took: {round((time.time() - start_time), 2)}s")
                     elif decoded_line.get("ping", None):
                         pass
                     else:
                         self._logger.error(f"invalid queue line, ignore: {line}")
 
                 # if a keepalive message is issued, we can check here also regularly for exit condition set
                 if self._worker_thread.stopped():
```

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc9/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc9/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/simulated.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,23 @@
 def img_aquisition(
     shm_buffer_name,
     _condition_img_buffer_ready: Condition,
     _img_buffer_lock: Lock,
     _event_proc_shutdown: Event,
 ):
     """function started in separate process to deliver images"""
+
+    ## Create a logger. INFO: this logger is in separate process and just logs to console.
+    # Could be replaced in future by a more sophisticated solution
+    logger = logging.getLogger()
+    fmt = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s) proc%(process)d"
+    logging.basicConfig(level=logging.DEBUG, format=fmt)
+
+    logger.info("img_aquisition process started")
+
     target_fps = 15
     last_time = time.time_ns()
     shm = shared_memory.SharedMemory(shm_buffer_name)
 
     path_live_img = Path(__file__).parent.joinpath("assets", "backend_simulated", "simulated_background.jpg").resolve()
     path_font = Path(__file__).parent.joinpath("assets", "backend_simulated", "fonts", "Roboto-Bold.ttf").resolve()
 
@@ -219,7 +228,9 @@
                 raise RuntimeError("shared memory too small!")
 
             compile_buffer(shm, jpeg_bytes)
 
         with _condition_img_buffer_ready:
             # wait to be notified
             _condition_img_buffer_ready.notify_all()
+
+    logger.info("img_aquisition process finished")
```

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc9/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc9/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc9/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc9/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc9/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc9/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc9/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc9/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc9/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc9/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc9/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc9/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-notext-black-transparent.png` & `photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-notext-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-black-transparent.png` & `photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-text-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/icons/logo-text-white-transparent.png` & `photobooth_app-0.1.0rc9/photobooth/web_spa/icons/logo-text-white-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/247.74c0e45d.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/247.74c0e45d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/272.a73245eb.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/272.a73245eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/429.76096bfa.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/429.76096bfa.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/706.98593961.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/706.98593961.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/835.8e1bdcfb.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/835.8e1bdcfb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/931.55b1be58.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/931.55b1be58.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/954.7419ae78.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/954.7419ae78.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/app.979a8c9e.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/app.979a8c9e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc9/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/LICENSE.md` & `photobooth_app-0.1.0rc9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/README.md` & `photobooth_app-0.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc8/pyproject.toml` & `photobooth_app-0.1.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "photobooth-app"
 requires-python = ">=3.9,<3.12"
-version = "0.1.0rc8"
+version = "0.1.0rc9"
 description = "Photobooth app written in Python supporting DSLR, picamera2 and webcameras"
 authors = [{ name = "Michael G", email = "me@mgrl.de" }]
 maintainers = [{ name = "Michael G", email = "me@mgrl.de" }]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `photobooth_app-0.1.0rc8/PKG-INFO` & `photobooth_app-0.1.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: Photobooth app written in Python supporting DSLR, picamera2 and webcameras
 Project-URL: homepage, https://github.com/mgrl/photobooth-app
 Project-URL: repository, https://github.com/mgrl/photobooth-app
 Project-URL: documentation, https://mgrl.github.io/photobooth-docs
 Author-email: Michael G <me@mgrl.de>
 Maintainer-email: Michael G <me@mgrl.de>
 License-Expression: MIT
```

