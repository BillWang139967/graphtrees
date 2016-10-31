# graphtrees_遇见王斌


* [相关项目](#相关项目)
* [将 graphtrees 添加到现有zabbix项目](#将-graphtrees-添加到现有zabbix项目)
* [编写 zabbix 插件教程](#编写-zabbix-插件教程)
* [graphtrees 功能](#graphtrees-功能)
* [version](#version)

## 相关项目

> * [zabbix_3.0.4一键安装](https://github.com/BillWang139967/zabbix_install) 安装自带graphtrees
> * [zabbix常用模板](https://github.com/BillWang139967/zabbix_templates)
> * [zabbix终端管理工具](https://github.com/BillWang139967/zabbix_manager)

## 将 graphtrees 添加到现有zabbix项目

[添加到现有zabbix项目方法](./graphtree_src/README.md)

## 编写 zabbix 插件教程

[编写 zabbix 插件](./doc/plugin.md)

## graphtrees 功能

> * 一、集中展示所有分组设备
> * 二、集中展示一个分组图像
> * 三、集中展示一个设备图像
> * 四、展示设备下的Application
> * 五、展示每个Application下的图像
> * 六、展示每个Application下的日志
> * 七、对原生无图的监控项进行绘图

[设置显示图像的列数](doc/dispaly.md)

```
注意问题:
    在组和主机级别，默认只显示系统配置的graph
    点击application后，会显示3种数据：
    1. 系统默认有graph的；
    2. 系统默认无graph的；
    3. 日志类的
```
## version

1.0.1 更新:对原生无图的监控项进行绘图时，只显示enabled item

> * [原作者说明](doc/doc.md)
