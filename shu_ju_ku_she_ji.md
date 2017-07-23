# 数据库设计
###后台信息表
admin_message 存储前端用户操作产生的信息（在后台展示，例如：用户上传了车辆）
###运营文章表
article 存储文章信息及推荐车辆id（如：超值体验、新车专区、新鲜车型等）
###附件信息表
attachment_file_info 存储系统中上传的附件信息
###银行卡信息表
bank_card 存储用户绑定的银行卡信息
###浏览记录表
browse_log 存储用户浏览车辆的记录
###验证码表
captcha 存储验证码
###车辆表
car 存储车辆信息及车辆状态等
###车型表
car_model 存储车型信息
###我的收藏表
collection 存储用户收藏的车辆信息
###首页banner表
homepage_banner 存储首页轮播图信息及是否上架状态
###后台用户表
manager 存储后台用户的账号、密码、权限等信息
###推送信息总表
message_base 存储推送信息
###推送信息子表
message_child 存储后台发送给用户的推送信息及用户是否已读信息
###订单表
orders 存储用户的订单信息及订单状态信息
###充值记录表
recharge_record 存储用户的充值记录
###罚单信息表
ticket 存储用户的罚单信息及罚单处理状态
###用户表
users 存储用户信息及各种认证状态
###提现记录表
withdrawals_record 存储用户提现记录及状态信息