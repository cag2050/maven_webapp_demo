# maven_webapp_demo
开发环境：
* IDE：Eclipse IDE for Java EE Developers
* Tomcat 9.0
* jdk 1.8

使用 maven 原型（archetype）为 maven-archetype-webapp 创建此项目，其实就是maven的web项目。 

需要自己安装jdk 1.8, tomcat 9.0
 
在 tomcat 部署并启动 tomcat 后，访问地址：http://localhost:8080/maven_webapp_demo/  

修改 jsp 文件内容后，会 Republish 到 tomcat，刷新浏览器即可看到修改结果。

其实在eclipse中配置server的时候，eclipse会把web项目自动发布到工作空间的：
.metadata\.plugins\org.eclipse.wst.server.core\
的这个目录中，具体你的项目被发布到这个目录的哪个位置要看你配置的server个数了。假如你的eclipse中只配置了一个server，那么你的项目就被发布到：
.metadata\.plugins\org.eclipse.wst.server.core\tmp0\wtpwebapps
你会看到，在这个目录下有你的项目被发布到这里来了。在eclipse中运行server的时候，其实执行的代码就是这个地方的。

参考链接：http://blog.csdn.net/clj198606061111/article/details/20221133

