# 基本文档类型与文档类型

Selling and Fulfillment Foundation使用基本文档类型和文档类型来制定信息。
以下为OMS自带的基本文档类型:

* 订单
* 装货
* 一般
* 盘点
* 装箱
* 出库提货
* 工作单
* 商机

文档类型是来自于基础文档类型的特定业务文档。例如SO，PO都是起源于订单。

以下为定义的文档类型：

* 计划订单
* 销售订单
* 采购订单
* 退换货订单
* 模板订单
* 调拨单
* 主订单(允许用户指定一系列订单以及将这些订单装运到客户并向客户收费的时间间隔)
* 装货
* 一般
* 盘点
* 装箱
* 出库提货
* 工作单
* 报价


每种文件类型都必须建立业务规则，如支付规则和修改规则。
订单的具体相关文件（即1.Planned Order 2.Sales Order 3.Purchase Order 4.Return 5.Template Order 6.Transfer Order 7.Master Order）都是继承自一个基本文件Order。



