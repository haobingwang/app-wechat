# app-wecht

微信开发服务端

需要部署到具有公网 IP 的服务器。

## 测试号管理

接口配置信息：

- URL  ：http://外网IP/wx 
- Token：随便填写

如果提示`配置失败`，接口返回信息：`token check fail`。原因是所填的 URL 不能正确返回加密后的字符串。

```shell
pm2 start app.js -i 0 --name "wechat"
```
