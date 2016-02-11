
# cordova-plugin-app-update
App updater for Cordova/PhoneGap

# Preview
![enter image description here](https://raw.githubusercontent.com/vaenow/cordova-plugin-app-update/master/res/img/Screenshot_2015-10-31-13-42-13.jpg)

# 

![enter image description here](https://raw.githubusercontent.com/vaenow/cordova-plugin-app-update/master/res/img/Screenshot_2015-10-31-13-42-19.jpg)

# Install

### Latest published version on npm (with Cordova CLI >= 5.0.0)
`cordova plugin add cordova-plugin-app-update`

or this fork that provide internationalization for english and french  

`cordova plugin add https://github.com/EmmanuelSimo/cordova-plugin-app-update.git`

# Usage
 - Simple:
```js
var updateUrl = "http://192.168.0.1/version.xml";
window.AppUpdate.checkAppUpdate(onSuccess, onFail, updateUrl);
```
 - Verbose
```js
var appUpdate = cordova.require('cordova-plugin-app-update.AppUpdate');
var updateUrl = "http://192.168.0.1/version.xml";
appUpdate.checkAppUpdate(onSuccess, onFail, updateUrl);
```




versionName | versionCode
------- | ----------------
0.0.1  | 12
0.3.4  | 3042  
3.2.4   | 302042
12.234.221  | 1436212

### server version.xml file
 
```xml
<update>
    <version>302042</version>
    <name>name</name>
    <url>http://192.168.0.1/android.apk</url>
</update>
```


# Platforms
Android only

# License
MIT

# :snowflake: :beers:
Pull request is welcomed, I'll be very pleasure if you can help me to improve this cordova-plugin. 
