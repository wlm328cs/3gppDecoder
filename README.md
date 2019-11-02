3gppDecoder
=====

## 概述

使用RED语言实现的3GPP解码器。
 - 支持2G、3G、4G、5G等等等相关通信协议。
 - 理论上，通过修改配置文件，可以解码wireshark未来支持的所有协议。
 - 支持各种乱七八糟的码流输入：
 - - 连续的码流1a2b3c432345
 - - 空格隔开的码流 1a 2b 3c 43 23 45
 - - 逗号隔开的码流 1a,2b,3c,43,23,45
 - - 以0x开头的码流 0x1a 0x2b 0x3c 0x43 0x23 0x45
 - - 以上所有的混合 0x1a,2b ,3c 4323,0x45
 
## 预览

<div align=center>
  <img src='https://github.com/konglinglong/3gppDecoder/blob/master/%E7%95%8C%E9%9D%A2.png' alt='preview' />
</div>

## 使用
#### 1. 从GitHub的releases页面下载[3gppDecoder-Release-XXX.zip](https://github.com/konglinglong/3gppDecoder/releases)
#### 2. 解压到一个文件夹，打开3gppDecoder.cfg配置文件：
 - 修改wireshark路径（注意：路径只支持"/"，不支持"\\"）
 - 修改notepad++路径（注意：路径只支持"/"，不支持"\\"）
 - 增加配置文件里面没有但你需要用到的协议（前提是你的wireshark版本支持）
