1. Android Studio
1. Appium
	* desktop
	* console
	_run cmd and print **npm install -g appium**_
2. Node JS
	_set checkbox for install special tools _
	
	***
	### Important
	1. Make sure that environments variables are written:
		ANDROID_HOME - ./Android/Sdk
		Path: %ANDROID_HOME%\emulator;%ANDROID_HOME%\platform-tools;%ANDROID_HOME%\tools;%ANDROID_HOME%\tools\bin
	2. Make sure that Appium Capabilities fill:
		platformName Android
		platformVersion 8.0.0
		deviceName: Pixel_2_API_26[^1]
		udid emulator-5554[^2]
	3. You should may fill the path to ./Android/Sdk into Appium Configure main window 
		
		[^1]: ./Android/Sdk>emulator -list-avds
		[^2]: ./Android/Sdk>adb devices