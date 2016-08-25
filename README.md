用Node.js重写的通用页面框架，原框架采用ASP.NET MVC。:smile: 
既然是开源嘛，自然都是采用开源的东西，其中UI框架还是采用的BJUI(http://b-jui.com/)，后端采用ThinkJS，数据库采用PostgreSql
本框架通过配置模块的显示列、编辑列、查询列、按钮等，可以从数据库的表或者视图取数据，生成页面，通过Url: http://localhost/cmpage/emp (其中emp是模块名称) 可以访问该模块，实现了常用的分页列表、新增、编辑、查看、删除、条件查询等功能

运行步骤简述如下（具体参照 thinkjs.org）：
1、恢复数据库，直接用 pgAdmin 恢复数据库备份文件（cmpage.backup）
2、在/src/common/config/db.js 中配置数据库连接参数
3、运行：npm install --registry=https://registry.npm.taobao.org --verbose
4、运行：npm start

演示地址： http://139.129.48.131:8300/admin

![输入图片说明](http://git.oschina.net/uploads/images/2016/0407/171503_033281df_389947.png "模块列表")
![输入图片说明](http://git.oschina.net/uploads/images/2016/0407/171611_18aa7d89_389947.png "模块的显示列设置")
![输入图片说明](http://git.oschina.net/uploads/images/2016/0407/171717_a3be3142_389947.png "模块预览")