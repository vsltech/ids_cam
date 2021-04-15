####README################################
###IDS_CAM UEYE UI-3880CP-M-GL Rev.2######
###Developed BY Vishal Aditya#############
###Embedded Systems Engineer##############
###Innovatios Technology##################
###vishal@innovatiostech.com##############

Follow below instructions in sequence on your RaspbianOS
(Keep 32/64-bit for all package/sdk flavours respectively)
---------------------------------------------------------
1.Install Python3.7 32/64-bit
2.Install IDS Peak SDK: https://en.ids-imaging.com/files/downloads/ids-peak/readme/ids-peak-linux-readme-1.2.1_EN.html
	2.1 sudo apt-get install libqt5core5a libqt5gui5 libqt5widgets5 libqt5quick5 qml-module-qtquick-window2 qml-module-qtquick2 qtbase5-dev qtdeclarative5-dev qml-module-qtquick-dialogs qml-module-qtquick-controls qml-module-qtquick-layouts libusb-1.0-0
	
	2.2 sudo dpkg -i ids-peak-linux-armhf-1.2.1.0.deb
	    sudo apt -f install
		
3.Install IDS API Bindings for Python3
	3.1 cd /usr/local/share/ids/bindings/python/wheel/debian_10_buster
	3.2 sudo pip3 install ids_peak-1.2.0.5-cp38-cp38-win32.whl
	3.3 sudo pip3 install ids_peak_ipl-1.2.0.5-cp38-cp38-win32.whl
	
4.Install IDS Dependencies(Qt5, PySide2) for Python3
	sudo apt-get update
	sudo apt-get install qt5-default pyqt5-dev pyqt5-dev-tools
	
	sudo apt-get install python3-pyside2.qt3dcore python3-pyside2.qt3dinput python3-pyside2.qt3dlogic python3-pyside2.qt3drender python3-pyside2.qtcharts python3-pyside2.qtconcurrent python3-pyside2.qtcore python3-pyside2.qtgui python3-pyside2.qthelp python3-pyside2.qtlocation python3-pyside2.qtmultimedia python3-pyside2.qtmultimediawidgets python3-pyside2.qtnetwork python3-pyside2.qtopengl python3-pyside2.qtpositioning python3-pyside2.qtprintsupport python3-pyside2.qtqml python3-pyside2.qtquick python3-pyside2.qtquickwidgets python3-pyside2.qtscript python3-pyside2.qtscripttools python3-pyside2.qtsensors python3-pyside2.qtsql python3-pyside2.qtsvg python3-pyside2.qttest python3-pyside2.qttexttospeech python3-pyside2.qtuitools python3-pyside2.qtwebchannel python3-pyside2.qtwebsockets python3-pyside2.qtwidgets python3-pyside2.qtx11extras python3-pyside2.qtxml python3-pyside2.qtxmlpatterns python3-pyside2uic
			
5.Test Cam Live Stream on Python Code
	cd ids/master
	python main.py
	