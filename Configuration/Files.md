# CAS Overlay Template 目錄說明

> 只列可能會用到的目錄和檔案

```
├── build
│    └── libs
│         └── cas.war
├── etc
│    └── cas
│         └── config
├── helm
│    └── cas-server
│         └── values.yam
├── src
│    └── main
│         ├── java/org/apereo/cas/config
│         │    └── CasOverlayOverrideConfiguration.java
│         └── resources
│              └── application.yml
├── build.gradle
├── gradle.properties
├── gradlew
└── gradlew.bat
```

* **build**
    * 專案建置後會產生的目錄
    * 可以在這個目錄下拿到 WAR 檔案
* **etc/cas/config**
    * ...
* **helm/cas-server**
    * CAS Server 的設定
        * 設定檔的目錄設定以 Linux 為主，如：`/etc/cas`
* **src**
    * 加入預設的設定，在專案建置後會一併的包進 WAR 檔
* **build.gradle**
    * 建置腳本
    * 加入相關的相依性和套件需要調整這裡
        * 例如：使用 LDAP Authentication 需要在這裡新增專案相依
* **gradle.properties**
    * Gradle 設定
        * 設定檔的目錄設定以 Linux 為主，如：`/etc/cas`
* **gradlew**
    * Linux Gradle 建置批次檔，執行建置時會執行這個檔案
* **gradlew.bat**
    * Windows Gradle 建置批次檔，執行建置時會執行這個檔案