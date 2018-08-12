# app-wecht

微信开发服务端

需要部署到具有公网 IP 的服务器。

```shell
pm2 start app.js -i 0 --name "wechat"
```

## 测试号管理

接口配置信息：

- URL  ：http://外网IP/wx 
- Token：随便填写

请填写接口配置信息，此信息需要你有自己的服务器资源，填写的URL需要正确响应微信发送的Token验证。

如果提示`配置失败`，接口返回信息：`token check fail`。原因是所填的 URL 不能正确返回加密后的字符串，请检查服务端的路由和 token 是否同接口配置信息一致。
