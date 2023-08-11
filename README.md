### 项目部署大致步骤 
```
1、安装MySQL数据库
docker run -d --name mysql57 -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql:5.7
2、导入SQL文件
db/*.sql
3、修改MySQL数据库连接信息
src/main/resources/application.yml
4、安装软件环境
yum install java-1.8.0-openjdk maven -y
5、代码编译
mvn clean package
6、安装Tomcat
7、将构建出的war包拷贝到Tomcat网站根目录
cp target/web-demo-0.1.0.war tomcat/webapps/ROOT.war
8、启动Tomcat
```
