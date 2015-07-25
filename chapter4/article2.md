# 流程类型管道


在Selling and Fulfillment Foundation系统中，每个基本文档都会经历一系列在系统中事先定义好的过程，这些过程叫做基本过程类型。每一种基本文档都会有一个基本过程类型与之对应。对于订单这个基本文件就定义了以下三种基本过程类型：Fulfillment,Negotiation,Delivery。用户可以通过为这些过程创建过程类型管道（process type pipeline）去配置这些过程的具体工作流程。一个过程类型管道（process type pipeline）包括了指导这个过程的一系列的处理操作和状态信息。同时针对具体的处理操作，用户可以为它配置具体的事件，行为和判断条件。

例如订单基础类型定义了基础流程类型：
* Fulfillment
* Negotiation
* Delivery

<b>订单履行基础流程类型</b>
<table class="table table-bordered table-striped table-condensed">
  <tr>
    <th width="300px">Derived Process Types</td>
    <th>Process Type Pipelines</td>
  </tr>
  <tr>
    <td>Order Fulfillment </td>
    <td> Sales Order Fulfillment</td>
  </tr>
  <tr>
    <td>Planned Order Execution  </td>
    <td>Planned Order Execution</td>
  </tr>
  <tr>
    <td>Template Order  </td>
    <td>None</td>
  </tr>
  <tr>
    <td>Reverse Logistics </td>
    <td> Reverse Logistics, Consumer Returns</td>
  </tr>
  <tr>
    <td>Purchase Order Execution </td>
    <td> Purchase Order Execution, Drop Ship Purchase Order Execution</td>
  </tr>
  <tr>
    <td>Transfer Order Execution </td>
    <td> Transfer Order Execution</td>
  </tr>
  <tr>
    <td>Quote Fulfillment </td>
    <td> Quote Fulfillment</td>
  </tr>
</table>

<b>订单谈判基础流程类型</b>

<table>
  <tr>
    <th width="300px">Derived Process Types</td>
    <th>Process Type Pipelines</td>
  </tr>
 <tr>
  <td>Master Order Fulfillment</td>
  <td>Master Order Fulfillment</td>
 </tr>
  <tr>
  <td>Order Negotiation</td>
  <td>Order Negotiation</td>
 </tr>
   <tr>
  <td>Planned Order Negotiation</td>
  <td>Planned Order Negotiation</td>
 </tr>
   <tr>
  <td>Purchase Order Negotiation</td>
  <td>Purchase Order Negotiation</td>
 </tr>
</table>



<b>接受基础流程类型</b>

<table>
  <tr>
    <th width="300px">Derived Process Types</td>
    <th>Process Type Pipelines</td>
  </tr>
 <tr>
  <td>Return Receipt</td>
  <td>Return Receipt</td>
 </tr>
  <tr>
  <td>Purchase Order Receipt</td>
  <td>Purchase Order Receipt</td>
 </tr>
   <tr>
  <td>Transfer Order Receipt</td>
  <td>Transfer Order Receipt</td>
 </tr>
   <tr>
  <td>Sales Order Receipt</td>
  <td>Sales Order Receipt</td>
 </tr>
</table>
流程类型管道包含一系列的事务和状态。一个管道包含很多文档的类型。在管道中你也可以包含事件、动作、条件。



在Selling and Fulfillment Foundation系统中还涉及到一个管道（pipeline）选择的功能，这主要通过在一个工作流中的特定时间点根据执行事先定义好的条件判断，得到结果并选择相应的管道(pipeline)流程。举例来说就是，当一个组织在处理销售订单时，提供两种不同的管道（pipeline）处理流程分别用于处理包含大量产品条目的订单和处理少量产品条目的订单。当系统收到一个订单信息时，会首先执行事先定义好的条件判断，得到判断结果，如果订单具有大量产品条目就执行相应的管道（pipeline）流程，如果不是执行另一个管道（pipeline)流程。这就使用户通过事先的配置提高订单流程的自动化程度


