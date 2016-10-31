### 原作者说明

##zabbix版本要求 3.0.x

###安装
```
cd 您的Zabbix-WEB目录
wget https://raw.githubusercontent.com/OneOaaS/graphtrees/master/graphtree3-0-1.patch
yum install -y patch
patch  -Np0 <graphtree3-0-1.patch

或者下载web下的所有文件替换您的Zabbbix-WEB目录下的所有文件，修改配置即可
```
#官方RPM包安装的如下
```
mkdir  /tmp/zbx
mv  /usr/share/zabbix /usr/share/zabbix-old
wget http://sourceforge.net/projects/zabbix/files/ZABBIX%20Latest%20Stable/3.0.1/zabbix-3.0.1.tar.gz
tar xf zabbix-3.0.1.tar.gz
cd zabbix-3.0.1/frontends/php
wget https://raw.githubusercontent.com/OneOaaS/graphtrees/master/graphtree3-0-1.patch
yum install -y patch
patch  -Np0 <graphtree3-0-1.patch
cp -r /tmp/zbx/zabbix-3.0.1/frontends/php /usr/share/zabbix
cp /usr/share/zabbix-old/conf/zabbix.conf.php /usr/share/zabbix/conf/
如果是3.0.2/3.0.3 使用同样方法即可
```

#实现效果
http://t.cn/RqAeAxT
