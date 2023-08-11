### 使用步骤
```
1、安装MySQL数据库
docker run -d --name mysql57 -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql:5.7
2、修改MySQL数据库连接信息
src/main/resources/application.yml
3、安装软件环境
yum install java-1.8.0-openjdk maven -y
4、代码编译
mvn clean package
5、安装Tomcat
6、将构建出的war包拷贝到Tomcat网站根目录
cp target/*.war tomcat/webapps/ROOT.war
7、启动Tomcat
```
