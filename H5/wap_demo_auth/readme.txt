
        ╭───────────────────────╮
          连连银通代码示例结构说明           
        ╰───────────────────────╯ 
　                                                                  
　       接口名称：wap支付
         开发语言：ASP.NET(c#)
         版    权：连连银通电子支付有限公司
    ─────────────────────────────────


本代码只是为了方便商户测试而提供的样例代码，商户可以根据自己网站的需要，按照技术文档编写,并非一定要使用该代码。

 ─────────────────────────────────
    
※注意事项※：

本代码示例（demo）采用C#编写，
请添加引用：Newtonsoft.Json.dll
并修改配置文件PartnerConfig.cs , 修改其中的RSA密钥/MD5密钥、异步通知及结束返回URL、商户编号、签名方式、业务类型等信息
部署成功后浏览器中输入http://ip:port/可以进入demo演示页面。
───────
 代码文件结构
 ─────────────────────────────────

配置文件：
PartnerConfig.cs

wap支付入口文件
Default.aspx  
paySubmit.aspx

异步通知页面：
notify_url.aspx,notify_url.aspx.cs
支付结束后返回页面：
urlReturn.aspx,urlReturn.aspx.cs

工具类：
Md5Algorithm.cs
RSA.cs
SignTypeEnum.cs
YinTongUtil.cs

其他：
css文件夹
image文件夹

 ─────────────────────────────────

出现问题，求助方法
──────────

如果在集成连连支付接口时，有疑问或出现问题，可在连连支付开放平台上查找答案。
http://open.lianlianpay.com/open/
或者联系我们的技术支持 tel:0571-56072616 


