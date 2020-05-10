# foundation-dependency

Java 基础依赖（工具类、数据库、Spring） 统一管理版本

项目中引入
```xml

	<parent>
		<groupId>com.github.sixinyiyu</groupId>
		<artifactId>spring-dependency</artifactId>
		<version>0.0.1-SNAPSHOT</version>
		<relativePath>../</relativePath>
	</parent>
	
	<dependencyManagement>
		<dependencies>
			<dependency>
				<groupId>com.github.sixinyiyu</groupId>
				<artifactId>data-dependency</artifactId>
				<version>0.0.1-SNAPSHOT</version>
				<type>pom</type>
				<scope>import</scope>
			</dependency>
		</dependencies>
	</dependencyManagement>
	
```


在   dependencies中申明 dependencyManagement 定义的依赖即可