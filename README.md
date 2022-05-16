# 轻量化的智能家居（HomeKit_List）

## 介绍

`工作原理`： 将不支持HomeKit的智能家居设备伪造成苹果支持的智能家居设备

## 技术栈

`nodejs`，其中对米家小程序做了反编译，逆向出了米家加密方式，以及Api构造。

### 准备

`服务器`：树莓派或者NSA等(需要本地部署)

`中枢控制` HomePod MiNi 或 HomePod 或 iPad(用于远程服务)



## 食用方法

```
启动方式：
npm install
npm run server
```


``` js
米家设备调用方法：
import { login,httpEncrypt } from '../MiHome_SDK/main';
//米家APP账号，密码
const token = login('你的手机号','密码')
//返回token
console.log(token);
```