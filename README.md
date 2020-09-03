# sub_converter_convert
转换ssr/v2ray订阅链接转换的工具

### 背景
最初我们有了SS/SSR/V2RAY等爬墙工具，但手动添加节点不胜其烦

接着我们就有了机场和节点订阅，还有surge/quantmultx/surfboard/clash等得心应手的工具

但每个工具配置文件都不相同，手动修改不胜其烦

接着我们就有了订阅链接转换的工具

但每次更换机场都得重新转换，重新配置一下，不胜其烦

接着我就写了个小工具：

**订阅链接转换的转换工具**

可以让你的不同工具仅添加一次配置订阅，就能在你更换机场的时候

只在一个地方更新，你的所有设备自动就更新了！

在cloudflare worker上实现，免费！稳定！

使用cf worker的tutorial网上很多，不再赘述

### 使用
将程序导入worker，配置好你机场的订阅链接，访问worker的时候url后面带上参数，即可生成不同工具的配置

如生成clash的配置，访问
```
https://xxx.xxx.workers.dev/clash
```
即可！
