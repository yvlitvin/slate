--- 

title: AuthorizationService Api 

language_tabs: 
   - shell 
 


toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 

includes: 
   - errors 

search: true 

--- 

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "https://auth-dev.wirexapp.com/sso/Ping"
  -H "Authorization: yourAPIKey"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('yourAPIKey');
```

# Introduction 

**Version:** v1 


# /Ping
```shell
# With shell, you can just pass the correct header with each request
curl "https://auth-dev.wirexapp.com/sso/Ping" -H "accept: application/json"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('yourAPIKey');
```


**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |


# /CONNECT/TOKEN
```shell
# With shell, you can just pass the correct header with each request
curl -X POST "https://auth-dev.wirexapp.com/sso/connect/token?ClientId=ClientId&ClientSecret=ClientSecret&GrantType=GrantType&UserName=UserName&Password=Password&DeviceId=DeviceId&Scope=Scope&TwoFactorCode=TwoFactorCode&SystemType=SystemType&CompanyId=CompanyId&Code=Code&RedirectUri=RedirectUri" -H "accept: application/json"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('yourAPIKey');
```

## ***POST*** 

### HTTP Request 
`***POST*** /connect/token` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| ClientId | query |  | No | string |
| ClientSecret | query |  | No | string |
| GrantType | query |  | No | string |
| UserName | query |  | No | string |
| Password | query |  | No | string |
| DeviceId | query |  | No | string |
| Scope | query |  | No | string |
| TwoFactorCode | query |  | No | string |
| SystemType | query |  | No | string |
| CompanyId | query |  | No | string |
| Code | query |  | No | string |
| RedirectUri | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /CONNECT/REVOCATION
## ***POST*** 

### HTTP Request 
`***POST*** /connect/revocation` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Token | query |  | No | string |
| TokenTypeHint | query |  | No | string |
| ClientId | query |  | No | string |
| ClientSecret | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /EXTERNALLOGIN
## ***GET*** 

### HTTP Request 
`***GET*** /ExternalLogin` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| DeviceId | query |  | Yes | string |
| DeviceName | query |  | Yes | string |
| ClientId | query |  | Yes | string |
| Provider | query |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /EXTERNALLOGINCALLBACK
## ***GET*** 

### HTTP Request 
`***GET*** /ExternalLoginCallback` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /API/TWOFACTOR/REGISTRATION/QR
## ***GET*** 

### HTTP Request 
`***GET*** /api/twofactor/registration/qr` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /API/TWOFACTOR/REGISTRATION/CODE
## ***GET*** 

### HTTP Request 
`***GET*** /api/twofactor/registration/code` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
