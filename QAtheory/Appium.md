Open Source project for iOS / Android / Windows desktop

_Support:_

- Java
- JS
- C#
- Python
- PHP

_Types of Mobile Application:_

- Native
- Web
- Hybrid
- Instant
- PWA

_Concept:_

1. Client/Server Architecture  
    Appium is a Web Server wich get http request - send to application - get the response - return to us
2. Session
3. Desired Capabilities

### Locator Strategy

|name|iOS|Android|
|---|---|---|
|Accessibility ID|acceddibility-id|content-desk|
|class name|attribute class||
|ID|name and label|resource-id|
|Name|-|-|
|XPath|-|-|
|Images|Base encoded images files||

### Tools

1. Android Studio
    
2. Appium
	 * desktop
	- console  
        _```run cmd and print npm install -g appium```
3. Node JS  
    _set checkbox for install special tools_
    
    ---
    
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
        

---

[^1]: ./Android/Sdk>emulator -list-avds
[^2]: ./Android/Sdk>adb devices