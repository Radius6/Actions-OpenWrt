237大佬immortalwrt24.10 内核6.6

git clone https://github.com/padavanonly/immortalwrt-mt798x-6.6.git

默认feeds.conf已经失效故使用官网的

Github Ac­tions 教程https://p3terx.com/archives/build-openwrt-with-github-actions.html
 
pass编译根据官方文档直接写入feeds.conf  在这里增加JDCloud-AX6000-Baili-immortalwrt.yml GOLONG版本否则编译不过


FAQ  ：HAProxy 运行passwall显示不运行

找到原因了，默认被隐藏了这个菜单，确切的说，安了haproxy也会没有，真正的原因是，得用浏览器恢复隐藏菜单
http://IP管理地址/cgi-bin/luci/admin/services/passwall/show 比如我就进这个就可以看到负载均衡菜单了
我是在FAQ里看到的........
关于DNS问题：

部分浏览器可能有内置的DNS，请务必关闭。如：chrome。 设置 - 安全和隐私设置 - 使用安全 DNS 关闭。
有时候重启后，上不了，尤其是GFW模式。这时请先关闭所有浏览器（重要），Windows客户端请ipconfig /flushdns。手机端请关闭WIFI，切一下飞行模式再切回来。
客户端DNS和默认网关必须指向本路由器。
如果你自行配置了错误的DNS流程，后果自负！
可以使用负载均衡实现故障切换功能。
恢复默认配置方法，地址栏输入例：http://IP管理地址/cgi-bin/luci/admin/services/passwall/reset_config
隐藏菜单方法，地址栏输入例：http://IP管理地址/cgi-bin/luci/admin/services/passwall/hide
当你隐藏后想再次显示，地址栏输入例：http://IP管理地址/cgi-bin/luci/admin/services/passwall/show
