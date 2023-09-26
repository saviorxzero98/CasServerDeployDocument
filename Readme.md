# CAS WAR Overlay Template

> 文件以 CAS 6.6 版



## 1. 環境準備

* **OpenJDK 11**
    * [Microsoft Build of OpenJDK](https://www.microsoft.com/openjdk)
* **[Apache Tomcat](https://tomcat.apache.org)**
    * 可以換成其他 Servlet Containers，例如： Jetty、Glassfish、WildFly...
    * 這裡使用的是 Apache Tomcat 9.0



---

## 2. 下載 CAS Overlay Template

* 下載 https://github.com/apereo/cas-overlay-template
    * 這裡使用的是 6.6 版本，且切換到 6.6 的 Branch
*  或者執行 git clone

```shell
git clone https://github.com/apereo/cas-overlay-template.git
```



---

## 3. 修改 CAS Server 配置與相依元件

* [CAS Overlay Template 目錄說明](Configuration/Files.md)
* [CAS Server 配置](Configuration/Index.md)
* 如果相依元件有異動的話請重新建置 WAR 檔案，並重新佈署與執行 CAS Server
    * 如果只修改相關 Server 配置檔案 (例如： `application.yml`)，僅需要在調整後重新啟動 CAS Server 即可



---

## 4. 建置

* 執行以下指令建置專案
* **Windows**

```shell
gradlew.bat clean build
```

* **Linux**

```shell
gradlew clean build
```

* 建置完畢後會在產生 `build/libs`，同時目錄下會有 `cas.war` (WAR 檔案)



## 5. 佈署與執行

* 兩種佈署與執行方式：
    1. **[佈署到 Apache Tomcat](Deploy/Tomcat.md)**
    2. **[透過 Gradlew 直接執行](Deploy/Gradlew.md)**



---

## 6. CAS Client 的使用

* 透過 CAS Client 介接 CAS Server
    * 可參考 **[Github - GSS.Authentication.CAS](https://github.com/akunzai/GSS.Authentication.CAS)** 的範例



---

## 參考資料

* **[官方文件](https://apereo.github.io/cas/6.6.x/index.html)**
* **[CAS 6.2.x Deployment - WAR Overlays](https://fawnoos.com/2019/11/03/cas62-gettingstarted-overlay/)**
* **[Install CAS Server With DB Authentication](https://medium.com/swlh/install-cas-server-with-db-authentication-8ff52234f52)**
* **[kwei Blog - 建立 CAS server](https://sleepyman212.github.io/post/cas_build/)**
* **[CAS Community](https://groups.google.com/a/apereo.org/g/cas-user)**

