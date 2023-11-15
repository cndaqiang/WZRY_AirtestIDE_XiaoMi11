# 王者熟练度工具使用方法

## 后续更新
https://github.com/cndaqiang/AirTest_MobileAuto_WZRY

## 安装初始化

1. 打开网页 https://airtest.netease.com/ 下载安装
2. 打开软件 软件最上面有一个 Options 点击 出现 `Language` 选择 `简体中文`
3. 打开软件 软件最上面有一个 `文件` 点击 `打开脚本`

## 连接手机(无线ADB调试)
IP
```
# --------------------- 自定义信息 --------------------->
设备类型 = "Android"  # 设备类型？(Android/Windows/iOS)
设备IP地址 = "192.168.12.164"  # 设备IP地址:端口号 默认: (IOS: IP地址:8100 Android: IP地址:5555)
```
端口
```
    设备信息 = {
        "链接": format("{}:///{}:{}".format(设备类型, 设备IP地址, 5555)),
        "王者应用ID": "com.tencent.tmgp.sgame"
    }
    if 设备类型 == "iOS":
        设备信息 = {
            "链接": format("{}:///{}:{}".format(设备类型, 设备IP地址, 8100)),
            "王者应用ID": "com.tencent.smoba"
        }
```

注有些手机连接不上,找找原因

## airtest修改和运行
1. 显示手机画面
2. 使用`touch`,截取手机画面上的图片(代码格式)
3. 是用截取的图片替换原有代码中的图片

例如修改英雄和线路


## 终端运行
通过观察airtest的运行日志发现可以
```
"/Applications/AirtestIDE.app/Contents/MacOS/AirtestIDE" pyrunner "/Users/cndaqiang/Desktop/WZRY_AirtestIDE-main/XiaoMI11.py" 

```
