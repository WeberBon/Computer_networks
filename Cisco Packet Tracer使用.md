# Cisco Packet Tracer使用

## 下载|Download

[链接](https://pan.baidu.com/s/1YG10xepo6CUqQNTENqrbgA )
提取码：`pwei`

> 下载安装完成后，可以注册思科账户登录也可使用Guest身份使用

## 使用方法|Using

**打开后的主界面**

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122305834-314975424.png)



- 工作区：主界面的空白区域。在工作区中可以创建网络拓扑、配置设备和观察模拟过程。大家可以像操作真实设备一样打开设备的控制台对设备进行配置和管理。
- 设备库：设备库在模拟器的左下角。设备库两排图表中最重要的就是路由器、交换机、链接和终端设备。

---

**构建一个简单的网络|Build a Network**

模拟器中构建网络是非常简单的，只要将图标拖到工作区，并按照设备要求选择合适的链路连接设备即可。

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122321134-1165658243.png)



在设备连接过程中大家只要用鼠标选择链路，单击需要连接的设备，模拟器就会显示可用的端口。

==如果链路工作正常，模拟图中就会显示闪烁的绿色小点。==如果链路出现错误就会出现红色闪烁的小点。

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122330944-1556782452.png)



---

**配置PC和服务器**

PC主机和服务器的配置类似，所以这里只介绍PC主机的网络配置。

PC主机的IP地址配置和网关配置不在同一个窗口，这和真实的计算机还是有区别。

单机PC主机图标，然后选择Config选项后进入IP地址配置界面。

其中IP地址的配置在INTERFACE选项中，在如下图所示的“FastEthernet0”端口中设置IP地址和子网掩码。动态主机配置也在此界面进行选择，点击DHCP前面的单选按钮即可完成这个配置。

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122340806-844656017.png)



![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122349796-216086764.png)



网关和域名服务器的设置在Global/Settings界面，如下图所示：

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122400287-1236737168.png)



在PC主机Desktop选项中点击Command Prompt可以启动命令行窗口。在这个窗口中可以使用网络调试命令对所构建的网络进行调试。

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122412520-878143701.png)



服务器和PC主机的区别在于服务器可以启动Web、FTP、Firewall等简单的服务。这些应用服务在服务器的Service选项中启动。下图是配置FTP的界面。在这个界面中可以看到FTP服务有一个默认的用户Cisco.这个用户登录FTP服务的口令也是Cisco。

![](https://img2020.cnblogs.com/blog/1969825/202004/1969825-20200430122422475-672404091.png)



---

**配置交换机和路由器**

单击交换机或者路由器就会出现他们的配置窗口。其中CLI选项卡包含了设备的控制台，控制台提供命令行模式的配置管理界面，这个界面与真实的设备的配置界面是类似的。

**保存一次配置**

如果要保存自己构建的网络，可以在菜单中选怎File->SaveAs进行网络配置的保存。模拟器会询问你想要保存的文件的位置。在你制定的文件名后模拟器会将你所有的配置保存成扩展名为.pkt的文件。在实验过程中可以使用这种方法保存模拟的现场，在需要的时候继续进行练习。
