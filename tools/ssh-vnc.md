# ssh登陆，建立vnc，连接vnc

1. 下载[putty.exe](https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe)

2. win7运行putty.exe

3. Host Name填入 `103.105.57.77` , Port默认`22`，Connection type选`SSH`

4. login as:  `risvv`, password: `ssh_password` 
输入密码之后按回车会提示登录成功。此处输入密码界面没有*号提示。

> login as: risvv
> risvv@103.105.57.77's password:
> Last login: Tue May 15 10:23:47 2018 from xxx.xxx.xxx.xxx


6. 启动vnc,输入以下命令

```shell
/home/risvv/startvnc
```

> New 'riscvv-svr:3 (risvv)' desktop is riscvv-svr:3

> Starting applications specified in /home/risvv/.vnc/xstartup
> Log file is /home/risvv/.vnc/riscvv-svr:3.log


如何需要修改分辨率和端口，可以使用下面命令：
```shell
vncserver -geometry 1280x1024 -depth 24 :8
```
其中`1280x1024`根据自己的显示器分辨率配置,`8`为对应的vnc端口号


7. 使用[vncviewer](https://www.realvnc.com/en/connect/download/viewer/)连接

> VNC Server: 103.105.57.77:3
> Encryption: Let VNC Server choose
> Passwd : vnc_password

－－－－－－－－－  
不忘出芯



