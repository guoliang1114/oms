# 密码策略
Selling and Fulfillment Foundation提供了设置密码的策略。密码策略就是一组规则。同时系统提供了默认的规则组，你可以针对业务修改。

密码策略总体上的定义:

* 密码强度: 它包含密码的长度(最短和最长)，特殊字符，密码复用。
* 口令生成: 系统会在某些情况下自动生成密码，例如，用户被创建，密码过期，失败登陆次数过多。
* 密码重置：通过邮件或者短信将用户密码重置。

#密码加密


Selling and Fulfillment Foundation的数据库会保护用户的密码，将用户的密码加密后在存储到数据库。

受保护的密码首先为每一个密码生成一个随机的字符串(salt)，通过加盐后的密码被hash存储到数据库中。系统为每一个密码存储了经过16位加盐的SHA-256哈希。

YCPValidateChangedPasswordUE以及YCPCheckPasswordsMatchUE这两个UE能够被实现并且提供定制化的哈希逻辑。


