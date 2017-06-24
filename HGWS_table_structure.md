
# HGWS表结构

## 顾客模组

tb_order 订单表

列名|类型|含义|约束
-|-|-|-
orderno|number(20)|订单号|pk
genetime|date|订单生成时间|
accid|varchar2(30)|账号|fk
orderstat|char(1)|状态(1正常、2申请取消、3取消中、0已取消)|
paid|char(1)|是否已支付|

cs_account 账号表

列名|类型|含义|约束
-|-|-|-
accid|varchar2(30)|账号|pk
accpwd|varchar2(30)|密码|

tb_address 收货地址表

列名|类型|含义|约束
-|-|-|-
accid|varchar2(30)|账号|pk
name|varchar2(20)|收货人|
address|varchar2(100)|收货地址|
mobile|varchar2(11)|手机号码|


## 店铺模组

bu_account 商家账号表

列名|类型|含义|约束
-|-|-|-
accid|varchar2(30)|账号|pk
accpwd|varchar2(30)|密码
