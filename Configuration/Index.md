# CAS Server 配置與相依性修改

## 架構圖

![](https://apereo.github.io/cas/6.6.x/images/cas_architecture.png)



---

## 配置設定

1. **Authentication** － CAS Server 帳號驗證來源的設定
    * [Static User Authentication](1.Authentication/1.1.StaticUser.md) －固定使用者帳號和密碼
    * [LDAP Authentication](1.Authentication/1.2.LDAP.md) －介接 OpenLDAP 的帳號驗證來源
    * Database Authentication － 介接資料庫的帳號驗證來源
    * [REST Authentication](1.Authentication/1.4.REST.md) －介接來自 REST API 的帳號驗證來源
2. **[Service Management](2.ServiceManagement/Index.md)** －CAS Client 的服務設定
    * **Registered Services Metadata**
        * [請參考官方文件](https://apereo.github.io/cas/6.6.x/services/Service-Management.html#registered-services)
    * **Storages**
        * [JSON 檔案](2.ServiceManagement/2.1.JsonServiceRegistry.md)
        * JPA (關聯式資料庫)
        * Redis
    * **Others**
        * [Service HTTP Security Headers](2.ServiceManagement/2.2.1.ServiceHTTPSecurityHeaders.md)
3. **Protocol** － CAS Server 與 Client 之間的協議
    * [CAS Protocol](3.Protocol/3.1.CAS.md)
    * [REST Protocol](3.Protocol/3.2.REST.md)
    * [OAuth2 Protocol](3.Protocol/3.3.OAuth2.md)
    * [OpenID Connect Protpcol](3.Protocol/3.4.OpenIdConnect.md)
        * [JWKS Storage](https://apereo.github.io/cas/6.6.x/authentication/OIDC-Authentication-JWKS-Storage.html)
    * [SAML Protocol](3.Protocol/3.3.SMAL.md)
4. **Ticketing** － Ticket 設定
    * Storages
        * Default Ticket Registry
        * JPA Ticket Registry
        * Redis Ticket Registry





















