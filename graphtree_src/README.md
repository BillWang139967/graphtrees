# graphtree_遇见王斌

## 新增文件

***将以下文件拷贝 Zabbix web 目录***

> * ./biggraph.php
> * ./graphtree.left.php
> * ./graphtree.right.php
> * ./graphtrees.php
> * ./js/vendors/highlight.min.js

以下为左侧栏树状图 ztree js控件

> * ./js/vendors/jquery.ztree.core-3.5.js
> * ./styles/ztree/line_conn.gif
> * ./styles/ztree/loading.gif
> * ./styles/ztree/zTreeStandard.gif
> * ./styles/ztree/zTreeStandard.png
> * ./styles/ztree/zTreeStyle.css

## 需修改文件(三个文件)


> * ./include/menu.inc.php

功能:在菜单栏添加按钮

80行左右为charts.php

在80行后新增
```

                [
                    'url'       => 'graphtrees.php',
                    'label'     => _('Graphtrees'),
                    'sub_pages' => ['graphtree.left.php', 'graphtree.right.php', "biggraph.php"]
                ],
```

> * ./jsLoader.php

功能：在左侧栏添加按钮

在65行后新增
```
    'jquery.ztree.core-3.5.js'          => 'vendors/',
```

> * ./include/page_header.php

功能: 左侧栏点击主机主后，有下级菜单

在159行左右添加
```
    if(!empty($page['css']) && is_array($page['css'])){
		foreach($page['css'] as $v){
			$pageHeader->addCssFile('styles/' . $v);
		}
	}
```
