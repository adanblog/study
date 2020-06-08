# 安装oracle11g数据库

##  一、oracle11g下载
点击[链接进入](https://www.oracle.com/database/technologies/oracle-database-software-downloads.html)进入选择相应的版本下载。oracle11g版本有两个文件,下载的时候需要登录，你可以注册一个或者百度一下oracle账号。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319593.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)

##  二、oracle安装
将下载好的两个文件win64_11gR2_database_1of2.zip、win64_11gR2_database_1of2.zip一起解压到当前文件夹中。
ps:解压后的路径最好不要出现中文和空格等不规则符号，否则之后可能会出现不可预知的错误！
在database文件夹中找到【setup.exe】双击安装
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319590.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)如果出现以下情况，可以直接点“是”继续安装
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319654.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)接下来进入安装步骤
### 第一步：配置安全更新
建议不填电子邮件、取消接受安全更新
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319722.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)
### 第二步：安装选项
选择默认的“创建和配置数据库”
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319703.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)
### 第三步：系统类，选择默认的“桌面类”
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319749.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)
### 第四步：典例安装，重要步骤
建议只需要将oracle及目录自行选择，目录路径不要有中文或者其他特殊字符。全局数据库名字默认就可以，口令自己设置（因为oracle本身有自己的密码原则，所以会有提示你的密码不符合规则，如果只是用于个人学习可以忽视不管，不必在意安全性），其他默认即可
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319931.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)点击下一步会提示口令不符合标准，点击“是”就行了。
### 第五步：先决条件检查
会坚持电脑是否符合软件安装要求。
### 第六步：概要
安装前相关选择配置信息，可以保存文件，但直接点击“完成”按钮就行。
### 第七步：安装产品
会自动安装产品，等待就行。
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020060615232022.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)数据库管理软件文件及DBMS文件安装完成后，会自动创建一个数据库实例默认前面的orcl数据库，还是等待就行
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020060615232046.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)实例数据库创建完成了，系统默认把所有账户都锁定，不可用（除了sys和system账户外），点击右边的口令管理，将常用的Scott用户解锁（点击√就行）输入自行设置密码，一般为123456
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319893.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319888.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)这里口令设置过于简单会提示你口令不能满足oracle复杂性策略，点击“是”继续就行。

### 第八步：安装完成了，关闭即可。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319923.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)
### 第九步：测试安装是否成功
以通过开始—>Oracle 11g—>应用开发程序—>Sql Developer 或 Sql Plus进行连接，打开后按照提示输入账户密码即可，或者通过命令行模式打开（快捷键win+r），输入用户名和密码!在这里插入图片描述]
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200606152319917.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)

> **关于阿丹博客**
>
> 以上内容，纯属一家之言，因个人能力有限，难免有疏漏和错误之处，如发现 bug 或者有更好的   >建议，欢迎留言批评指正，不吝感激。
> 下面阿丹的个人博客，记录所有学习和工作中的博文，欢迎大家前去逛逛。
>
> 个人博客：[http://www.adanblog.com/](http://www.adanblog.com/)
>
> GitHub：[https://github.com/adanblog/](https://github.com/adanblog/)
>
> ![](https://img-blog.csdnimg.cn/20200407220413142.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlbjkwMTIzMHpp,size_16,color_FFFFFF,t_70)