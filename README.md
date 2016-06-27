# hibernate介绍
## hibernate是什么
## 步骤
1. 导入包
```
        <!-- 添加Hibernate依赖 -->
		<dependency>
			<groupId>org.hibernate</groupId>
			<artifactId>hibernate-core</artifactId>
			<version>3.6.10.Final</version>
		</dependency>
		<!-- 添加javassist -->
		<dependency>
			<groupId>javassist</groupId>
			<artifactId>javassist</artifactId>
			<version>3.12.0.GA</version>
		</dependency>
```
导入本地的oracle　JDBC包
`F:\data\wwwtest\test-hibernate>mvn install:install-file -Dfile=E:/app/tom/product/11.1.0/db_1/jdbc/lib/ojdbc6.jar -DgroupId=com.oracle -DartifactId=ojdbc6 -Dversion=11.1.0 -Dpackaging=jar`
pom文件中增加　
```
<!-- 添加oracle jdbc driver -->  
    <dependency>    
        <groupId>com.oracle</groupId>    
        <artifactId>ojdbc6</artifactId>    
        <version>11.1.0</version>
    </dependency>
```
2. 配置数据源
主要有 数据库库驱动，地址，用户名，密码，方言

