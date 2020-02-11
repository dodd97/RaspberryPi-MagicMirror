# RaspberryPi-MagicMirror
    ```
    上手型项目
    ```

## 环境配置
### 树莓派系统安装
1. 官网下载系统镜像解压,通过balenaEtcher烧写到内存卡上.
2. 直接在内存卡中创建无后缀文件`ssh`以开启树莓派的ssh服务.
3. 修改config.txt,树莓派系统中路径为/boot/config.txt
    ```
    hdmi_force_hotplug=1    //开启树莓派HDMI输出热拔插
    config_hdmi_boost=4     ///开启树莓派HDMI输出信号增强
    ```
4. 
    
    
    
    在/usr/share/fonts/truetype/下建立文件夹myfonts，然后拷贝上述字体到改文件夹下。
             sudo mkdir /usr/share/fonts/truetype/myfonts
             cp *.ttf  /usr/share/fonts/truetype/myfonts/
        3. 更改myfonts和该目录下面的权限，可以都设成777
             sudo chmod -c 777 /usr/share/fonts/truetype/myfonts
             sudo chmode -c 777 /usr/share/fonts/truetype/myfonts/*
        4. 最后就是注册新添加字体了，执行如下命令：
             sudo mkfontscale
             sudo mkfontdir
             sudo fc-cache -fv

sudo apt-get remove --purge idle3 java-common libreoffice* minecraft-pi scratch nuscratch penguinspuzzle python-minecraftpi python3-minecraftpi smartsim sonic-pi wolfram-engine
sudo apt-get autoremove
sudo apt-get update
sudo apt-get upgrade
sudo rpi-update
 
 /etc/wpa_supplicant/wpa_supplicant.conf
 ```
 ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
 update_config=1
 country=CN
 
 network={
         ssid="CMCC-Yuan"
         psk="ywg10086584120"
         key_mgmt=WPA-PSK
         priority=5
 }
 ```
