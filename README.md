# Gost Tunnel使用指南
***
## 感谢: 
1. 感谢 @ginuerzh 大佬开发的 [gost](https://github.com/ginuerzh/gost) 隧道程序 ，功能强大使用简单，想要详细了解的朋友可以查看[官方文档](https://docs.ginuerzh.xyz/gost/)
2. 感谢 @风萧萧兮易水寒 大佬的[原始脚本](https://www.fiisi.com/?p=125)
3. 感谢 @ STSDUST 提供的EasyGost脚本（已删库），此脚本是基于其进行修改增强
4. 感谢 @ KANIKIG 提供的Multi-EasyGost脚本，此脚本是基于其进行修改
***
## 简介

> 项目地址及帮助文档:  
> https://github.com/XTBANNY/Gost-Tunnel
***
## 脚本

* 启动脚本  
  `wget --no-check-certificate -O gost.sh https://raw.githubusercontent.com/XTBANNY/Gost-Tunnel/master/gost.sh && chmod +x gost.sh && ./gost.sh`  
* 再次运行本脚本只需要输入`./gost.sh`回车即可  

> 注：由于 gost v2.11.2 功能稳定，此脚本将一直采用该版本，后续不再跟随官方更新

## 功能

### 原脚本功能

- 实现了systemd及gost配置文件对gost进行管理
- 在不借助其他工具(如screen)的情况下实现多条转发规则同时生效
- 机器reboot后转发不失效
- 支持传输类型：
  - tcp+udp不加密转发
  -  relay+tls加密

### 此脚本新增功能

- 增加了传输类型选择功能
- 新支持传输类型
  - relay+ws
  - relay+wss
- 落地机一键创建ss/socks5/http代理 (gost内置)
- 支持多传输类型的多落地简单型均衡负载
- 简单创建或删除gost定时重启任务
- 脚本自动检查更新
- 转发CDN自选节点ip
- 支持自定义tls证书，落地可一键申请证书，中转可开启证书校验

## 功能展示

![iShot2020-12-14下午05.42.23.png](https://github.com/XTBANNY/Gost-Tunnel/blob/main/.idea/1.png?raw=true)

![iShot2020-12-14下午05.42.39.png](https://i.loli.net/2020/12/14/vzpGlWmPtCrneOY.png)

![2](https://i.loli.net/2020/10/16/fBHgwStVQxc821z.png)

![3](https://i.loli.net/2020/10/16/xgZ6eVAwSzDUFjO.png)

![4](https://i.loli.net/2020/10/16/lt6uAzI5X7yYWhr.png)

![iShot2020-12-14下午05.43.46.png](https://i.loli.net/2020/12/14/YjiFTMCKs8lANbI.png)

![iShot2020-12-14下午05.43.11.png](https://i.loli.net/2020/12/14/VIcQSsoUaqpzx5T.png)
