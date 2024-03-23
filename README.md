# NTNU_Moodle_AutoLogin (Chrome Extension)

### 使用方法
```
下載插件包 > 將content.js 中的學號與密碼改為自己的帳密
> 打開 browser > 擴充功能 > 載入未封裝項目 > 選擇整個資料夾
```

### Source Code (若不下載套件包，可直接用tampermonkey等自動注入js的擴充功能)

```javascript

(function() {
    var STUDENT_ID = "TYPE_YOUR_STUDENTID_HERE"
    var PASSWORD = "TYPE_YOUR_PASSWORD_HERE"
    document.querySelector("#username").value = STUDENT_ID
    document.querySelector("#password").value = PASSWORD
    document.querySelector("#boxForm > div > form > div.sign-up-btn > button").click()

})();
```

```
不定期注意網頁是否更改架構，會第一時間修改並上傳
```
