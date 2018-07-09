# LLP-AuthPay-dotnet

欢迎来到连连认证收款的c#仓库， 本仓库包含c#接入认证收款网页版的示例代码及必要的说明。

其中， ```Web```目录下为认证收款PC端页面的示例工程；```H5```目录下为认证收款移动端页面的示例工程。

## 主要内容

[前置要求](#前置要求)

[认证收款测试商户号信息](#认证收款测试商户号信息)

[使用说明](#使用说明)

[文档说明](#文档说明)

## 前置要求

暂无

## 认证收款测试商户号信息

测试商户号: 201408071000001543

PKCS8格式私钥(供```c#```使用): 

```text
MIICdwIBADANBgkqhkiG9w0BAQEFAASCAmEwggJdAgEAAoGBAOilN4tR7HpNYvSBra/DzebemoAiGtGeaxa+qebx/O2YAdUFPI+xTKTX2ETyqSzGfbxXpmSax7tXOdoa3uyaFnhKRGRvLdq1kTSTu7q5s6gTryxVH2m62Py8Pw0sKcuuV0CxtxkrxUzGQN+QSxf+TyNAv5rYi/ayvsDgWdB3cRqbAgMBAAECgYEAj02d/jqTcO6UQspSY484GLsL7luTq4Vqr5L4cyKiSvQ0RLQ6DsUG0g+Gz0muPb9ymf5fp17UIyjioN+ma5WquncHGm6ElIuRv2jYbGOnl9q2cMyNsAZCiSWfR++op+6UZbzpoNDiYzeKbNUz6L1fJjzCt52w/RbkDncJd2mVDRkCQQD/Uz3QnrWfCeWmBbsAZVoM57n01k7hyLWmDMYoKh8vnzKjrWScDkaQ6qGTbPVL3x0EBoxgb/smnT6/A5XyB9bvAkEA6UKhP1KLi/ImaLFUgLvEvmbUrpzY2I1+jgdsoj9Bm4a8K+KROsnNAIvRsKNgJPWd64uuQntUFPKkcyfBV1MXFQJBAJGs3Mf6xYVIEE75VgiTyx0x2VdoLvmDmqBzCVxBLCnvmuToOU8QlhJ4zFdhA1OWqOdzFQSw34rYjMRPN24wKuECQEqpYhVzpWkA9BxUjli6QUo0feT6HUqLV7O8WqBAIQ7X/IkLdzLa/vwqxM6GLLMHzylixz9OXGZsGAkn83GxDdUCQA9+pQOitY0WranUHeZFKWAHZszSjtbe6wDAdiKdXCfig0/rOdxAODCbQrQs7PYy1ed8DuVQlHPwRGtokVGHATU=
```

其公钥已上传至商户站。有关您真实商户号的公私钥配置， 请参考[连连开放平台 - 公私钥配置](https://open.lianlianpay-inc.com/docs/development/signature-key-generation)。

> 测试商户号是连连正式环境的商户号， 需要使用真实信息进行测试， 测试时建议将订单金额设置到```0.01```元(CNY)。使用测试商户号时， 建议使用独特的用户唯一标识```user_id```及独特的商户订单号```no_order```以免与其他商户的测试信息冲突。

## 使用说明

使用前需添加引用```Newtonsoft.Json.dll```。

配置文件```PartnerConfig.cs```中包含RSA密钥/MD5密钥、异步通知及结束返回URL、商户编号、签名方式、业务类型等信息， 您可以根据需要做相应更改。

引用添加完成后， 根据实际情况完成工程部署， 部署成功后浏览器中输入http://ip:port/可以进入demo演示页面。

## 文档说明

有关认证收款的详细介绍及请求参数说明， 请参考[连连开放平台 - 认证收款](https://open.lianlianpay-inc.com/docs/receive-money/express/overview)。