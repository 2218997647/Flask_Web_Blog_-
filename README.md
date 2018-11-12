主要根据flask+redis+mysql实现，采用前后端分离的方式实现，使用csrf防护机制。前端接触较少，前端代码修改于网络案例。

主要功能

1. 主页：
    1.1 随机展示文章，点击可跳转至文章详情页面。
    1.2 提供登陆/注册入口，登陆后显示用户名，点击可跳转至个人中心。

2. 注册：
    2.1 用户账号默认为手机号。
    2.2 图片验证码正确后才能发送短信验证码（待实现）。
    2.3 短信验证码每60秒可发送一次（待实现）。
    2.4 每个条件出错时有相应错误提示。
    2.5 注册的密码加密存储。

3. 登陆：
    3.1 用手机号与密码登陆。
    3.2 错误时有相应提示。
    
4. 管理中心：
    4.1 显示手机号、用户名。
    4.2 提供修改个人信息的入口。
    4.3 提供我的文章入口。
    4.4 实名认证的入口（待实现）。
    4.7 提供退出的入口。
    
5. 我的文章页面：
    5.1 显示已经发布的文章信息。
    5.2 点击文章可以进入详情页面 。  
    5.3 提供发表新文章入口，文章配图（需要调用第三方云，待实现）。

6. 文章详情页：
    5.1 显示作者，文章类别，内容。
    5.2 文章配图（需要调用第三方云，待实现）。

7. 发布新文章：
    7.1 标题，内容，类别，图片（需要调用第三方云接口，待实现）。

8. 个人信息修改：
    8.1 个人头像（需要调用第三方云接口，待实现）。
    8.2 可以修改用户名。
 
9. 实名认证（待实现）、评论功能（待实现）。

10. 退出：
    10.1 提供退出功能。
    
    
参考来源：
   1. [美] Miguel Grinbe Flask Web开发：基于Python的Web应用开发实战 
   2. http://flask.pocoo.org/
   3. 尚学堂
   4. http://www.redis.net.cn/tutorial/3501.html
   5. 使用SQLAlchemy - 廖雪峰的官方网站
   6. 刘鑫 简易的基于SSH的问答系统 
   7. 刘鑫 基于安卓的仿网易新闻客户端
   8. 刘鑫 对抗神经网络验证码的生成
