# 透過 Gradlew 直接執行

## 1. 安裝和執行步驟


### Step.1 建立根目錄 (限 Windows)

* 由於多個設定有關路徑的設定會使用到 `/etc/cas` (以 Linux 目錄為主)
    * 可以手動修改目錄
* 如果不想手動修改目錄，一勞永逸的方式就是在專案所在的磁碟根目錄下新增 `etc/cas`
    * 例如：`C://etc/cas` 或 `D://etc/cas`



### Step.2 建立 Keystore

* 執行以下指令產生 keystore
* **Windows**

```shell
gradlew.bat createKeystore
```

* **Linux**

```shell
gradlew createKeystore
```

* keystore 會自動產生到上一個步驟的目錄下
    * 例如：`C://etc/cas` 或 `D://etc/cas`



### Step.3 執行 CAS Server

* 執行以下指令啟動 CAS Server
* **Windows**

```shell
gradlew.bat run
```

* **Linux**

```shell
gradlew run
```

* 執行成功後開啟瀏覽器連到 https://localhost:8443/cas
    * 可以看到 CAS 的登入頁面
        * 預設登入帳號
            * 帳號：`casuser`
            * 密碼：`Mellon`



---

# 2. 設定反向代理

### IIS

TODO...

### Nginx

TODO...



---

## 3. 設定開機自動啟動

### Windows 

TODO...

### Linux (Ubuntu)

TODO...