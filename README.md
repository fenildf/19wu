# 19wu

19wu - 卖活动票的小屋

这是一个基于 Rails3 的开源电子商务项目，主要是为了方便会议活动（e.g.RubyConfChina）网上卖票，项目上线后将完全免费。

之前做 ShopQi 时，项目功能太多，后期不少朋友想要贡献代码非常困难，新手学习门槛也高。
对于这个项目我决定推迟 2 周，将在 **2012年12月24日** 正式开始，并持续利用业余时间进行完善，欢迎关注或加入。

## 项目特色

* 完全免费
* 支持即时到帐网上支付
* 代卖公司票（提供发票）

## 基本需求

* `主办方`发起活动，卖票，发放电子票
* `参与者`可以在线购票，退票
* 个人票、公司票的库存可以联合计算，总数在 n 以内
* 支持调价规则，如11月1日起 118 元，或者第200张开始 118 元
* 支持手机、平板、网站访问

## 扩展需求

* 参与者关注`主办方`（下次RubyConfChina办活动你将得到邮件通知）

## 技术选型

* 数据库支持 PostgreSQL 和 MySQL
* 后台任务使用 delayed_job，而不使用 resque，避免对 redis 的依赖
* 前端基于 Spine.js


## License

[GNU  Affero GPL 3](http://www.gnu.org/licenses/agpl-3.0.html)