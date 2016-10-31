# zabbix 创建plugin

## zabbix RPC

> * zabbix 3.0.x

zabbix 的 RPC 接口是传递：

假如zabbix web目录位置在/data/web/zabbix,定义zabbix目录

ZABBIX_PATH=/data/web/zabbix

```
./api_jsonrpc.php
./include/classes/api/API.php
```
## Zabbix web 布局

zabbix web 页面布局非常简单。主要分为三部分：

include/page_header.php
new CWidget
include/page_footer.php
