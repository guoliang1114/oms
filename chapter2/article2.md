###可扩展的用户界面

它允许你不改变任何功能就能修改呈现的信息。你可以为Application Console定制化主题和皮肤。

Application Console：Application Console是一个基于 Web 的图形用户界面，只适用于 Microsoft® Internet Explorer 浏览器，版本 8 或更高版本。它用于创建、跟踪并查看订单、物品库存，以及退货订单。

Applications Manager：Applications Manager是用于配置 Sterling Selling and Fulfillment Foundation 的图形用户界面。它提供对不同的供应链组件工具的访问。

可以使用Applications Manager来修改HTML代码来对JSP页面进行变动。此外，您也可以扩展打印文档的样式。

####可扩展的Application Consoles用户界面

Selling and Fulfillment Foundation外观框架允许你扩展标准的Application Consoles的界面。Application Consoles的UI界面是使用HTML嵌入到JSP页面。UI层通过SDF(Service Definition Framework,服务定义框架)来访问API。

Selling and Fulfillment Foundation的呈现框架提供开发者扩展UI的集中方式：
* 定制化Selling and Fulfillment Foundation的登录页面，它是用户看到的第一个页面，有以下几种方式：
  * 为登录页面设置本地化的语言。
  * 设置本地指定的登录页面。
  * 为公司定制皮肤，当用户登录时，可以看到公司的信息
  * 从外部的程序登录，你可以类似单点登录的方式登录OMS
* 添加公司logo，你可以将以下内容的logo修改为自己公司的logo:
  * 登录页面
  * 菜单栏
  * 关于对话框
*  定义主题：主题定义了外观，例如字体、颜色等等。
*  定制化视图：定制化以下屏幕的布局：
   *  查询视图
   *  列表视图
   *  详细视图
*  定制业务实体
*  添加查询，你可以添加查询，将输入框定制为选择框
*  添加图像和图表：可以将数据用图表的形式展现。
*  定义菜单的结构：当创建定制化屏幕的时候，你需要确保不论是菜单结构还是导航，用户都是否有权限访问。
*  定制Selling and Fulfillment Foundation的图像，你可以定制化任何在程序中出现的图片。主要包含以下几个内容：
   *  菜单栏
   *  菜单
   *  application Conosle
*  定制屏幕导航：你可以定制屏幕导航。
*  创建定制化事件控制器：你可以创建或者插入定制化客户端验证。
*  为定制化文档类型创建屏幕。
*  创建定制化事务，你可以创建自定义单据或者交付事务，配置管道来修改单据的状态。
*  XML绑定：开发者可以很容易的组装输入XML传送给API以及输出的XML。

### 应用程序管理器扩展

应用程序管理器界面是使用Swing开发的。UI扩展的主要目的是为了允许任何数据库的扩展能够集成到UI界面。

扩展内容：

* 添加按钮和标签
* 添加文本框和勾选框
* 隐藏非强制的组件
* 重新组装组件来展示
* 创建和修改用户主题

> PS.屏幕中包含树形结构是不能扩
