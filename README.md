# Netkeeper
基于Openwrt的Netkeeper相关代码

# 写在前面的
基于miao1007学长里面的pppoe拦截方法写的程序。

不太会这种网页编辑，写的东西排版不好看还请见谅。

感谢前面大佬的贡献。

想在研究生期间接盘做做这个事情，直到2020年。但是无奈本人关于网路的知识不足，写写程序还可以，关于协议什么的都不懂。

如果有大佬原意带带我入门，或者想一起做的，可以留言联系我。

# 起因
我实验室的人很多，如果都能动态的把账号登录到路由器里面，然后想退出的时候就退出，这样大家网速叠加，用起来就很爽。

# 用法

## 事前准备
1.先安装一个潘多拉固件。

2.把root目录下面的所有文件，全部扔进路由器/root/目录下。

3.用WinSCP运行

```sh
sh nk4conf.sh
```
## 软件用法
登录账号数量是你要一次性登陆的数量，如果你要登陆一个号码，就填1，你要同时登陆两个，就填2。
拿之前单号双拨的例子来说，这里就应该填2，因为这两个号码必须同时拨出去。
但是如果是你和你室友两个人的号码，就可以不用同时拨，你可以和室友分别在自己的电脑上拨号。但不要同时用。
填好了登录账号数量，点准备拦截，稍等一会儿，然后会弹出提示框，确定之后再打开你的netkeeper，登陆一个账号，
然后左下角会有状态显示。会有显示vwan*什么的，然后再登录下一个账号，最后一个账号登录完了之后，连接状态地方应该会刷新连接状态。
左下角那个地方出现Get Ready，就差不多了。然后，连接状态里面会更新连接状态，一般是vwan* connect或者vwan* down，前面一个表示连接成功，
后面一个表示没成功。*表示数字。其余的功能没什么好说的。

再讲一讲自助板块。自助板块适合比较了解的人用。在连接出现什么毛病或者明明有端口却显示端口不足或者等等等的毛病的时候用。
手动查询某个网口的状态就不说了，记得填对网口名字。手动关闭网口具有关闭网口和重置网口信息的功能。
