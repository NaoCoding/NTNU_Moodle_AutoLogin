# NTNU_Moodle_AutoLogin (Chrome Extension)

### Requirement
```
下載插件包 > 打開 browser > 擴充功能 > 載入未封裝項目 > 選擇整個資料夾
```

### Source Code (若不下載套件包，可直接用tampermonkey等自動注入js的擴充功能)

```javascript
// ==UserScript==
// @name         NTNU Moodle3 AutoLogin
// @namespace    http://tampermonkey.net/
// @version      2024-03-23
// @description  NTNU Moodle3 AutoLogin
// @author       NaoCoding
// @match        https://moodle3.ntnu.edu.tw/
// @icon         https://www.google.com/s2/favicons?sz=64&domain=edu.tw
// @grant        none
// ==/UserScript==

(function() {
    var STUDENT_ID = "TYPE_YOUR_STUDENTID_HERE"
    var PASSWORD = "TYPE_YOUR_PASSWORD_HERE"
    document.querySelector("#username").value = STUDENT_ID
    document.querySelector("#password").value = PASSWORD
    document.querySelector("#boxForm > div > form > div.sign-up-btn > button").click()

})();
```
