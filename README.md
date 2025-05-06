## 代理加速的网页参考项目： https://github.com/MegaSuite/ghproxy-page
## Cloudflare 代理的项目： https://github.com/hunshcn/gh-proxy
## cf worker版本部署

首页：https://workers.cloudflare.com

注册，登陆，`Start building`，取一个子域名，`Create a Worker`。

复制 [Worker.js](https://raw.githubusercontent.com/yootor/Gh-Proxy-Pages/refs/heads/main/Worker.js)  到左侧代码框，`Save and deploy`。如果正常，右侧应显示首页。

#此版本修复了Github识别Zh-cn的请求头拒绝访问。

`ASSET_URL`是静态资源的url（实际上就是现在显示出来的那个输入框单页面）

`PREFIX`是前缀，默认（根路径情况为"/"），如果自定义路由为example.com/gh/*，请将PREFIX改为 '/gh/'，注意，少一个杠都会错！
