# WHID 平替版
WHID injector made by ESP8266 and ProMicro
origianl:https://github.com/whid-injector/WHID


## 原材料
ESP8266-12f
ProMicro
5v转3.3v稳压板
特利迦密钥玩具
usb转ttl
![b0eb7211ac8f3c8f27ed352ebc70654](https://github.com/user-attachments/assets/bef13d4d-dd05-4751-8faf-0633d724859a)

## 制作过程
### 将esp8266-12f与usb转ttl连接，注意gpio0接gnd，进入fasttboot模式
使用NodeMCU-PyFlasher工具将原链接中source文件夹下espcode中的.bin文件烧录进esp8266
### 将promicro连接电脑
使用arduino ide将开发板选择为arduino lenoardo，将source文件夹下arduino_32u4_code文件夹下的.ino文件使用arduino ide刷入pro micro开发板
### 接线
将pro micro的vcc接入5v转3.3v稳压板的input引脚，gnd接gnd引脚，txd和rxd分别与esp8266的rxd,txd相连
将esp8266的 vcc ， en ，gpio0 接入3.3v稳压板output引脚，gnd，gpio15接入gnd
![92bd69006596ad3e549079fec67d683](https://github.com/user-attachments/assets/16f991ff-4805-46f1-b926-be17d5e79b52)

## 使用
连接受害设备，在控制设备上连接esp8266的热点信号，进入192.168.1.1使用
![ae7762e129c0929593ab45b5b20ad30](https://github.com/user-attachments/assets/2e382fc4-32c1-4403-b24c-5018aeed5fcf)


