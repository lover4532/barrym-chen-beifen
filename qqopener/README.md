# **qq url跳转**<br>



该脚本理论上该脚本兼Quan、Surge，Loon使用一份即可<br>



## 配置<br>

##### quanx

```


[rewrie_local]

^http:\/\/c\.pc\.qq\.com\/middlem\.html url script-request-header https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js

^htps:\/\/qr\.alipay\.com\/[a-zA-Z0-9]{22} url script-request-header https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js

```
##### surge
```
[Script]

qqopener.js = type=http-request,pattern=^http:\/\/c\.pc\.qq\.com\/middlem\.html,script-path=https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js
qqaplipay.js= type=http-request,pattern=^https:\/\/qr\.alipay\.com\/[a-zA-Z0-9]{22},script-path= https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js

```
##### Loon
```
[Script]

http-request http-request,pattern=^http:\/\/c\.pc\.qq\.com\/middlem\.html script-path=https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js, requires-header=true

http-request http-request,pattern=^https:\/\/qr\.alipay\.com\/[a-zA-Z0-9]{22} script-path= https://raw.githubusercontent.com/barrym-chen/Script/master/qqopener/qqopener.js, requires-header=true

```

## 脚本说明<br>

1、无需配置MITM<br>

2、只对于不能正常在qq中打开的url生效<br>

3、默认跳转到safari中打开链接


## 感谢
@江湖中人


```

## 脚本说明<br>

1、无需配置MITM<br>

2、只对于不能正常在qq中打开的url生效<br>

3、默认跳转到safari中打开链接


## 感谢
@江湖中人