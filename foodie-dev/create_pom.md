# 聚合工程的搭建

- 顶级工程

  1. 聚合工程里可以分为顶级项目（顶级工程、父工程）与子工程，这两者的关系其实就是父子继承的关系，子工程在maven里称之为模块（module），模块之间是平级，是可以相互依靠的。
  2. 子模块可以使用顶级工程里所有的资源（依赖），子模块之间如果要使用资源，必须构建依赖（构建关系）
  3. 一个顶级工程是可以由多个不同的子工程共同组合而成

- 子工程

  1. 子工程创建完成后，需要返回父工程检查子工程是否导入成功

  2. 如果不指定打包方式，默认打包方式为 jar

  3. 依赖之间的资源引用  

     ```java
     mapper的依赖：
     	<artifactId>foodie-dev-mapper</artifactId>
     	<dependencies>
     		<!--
     			mapper -> pojo -> common
     			mapper通过pojo是可以使用common中相应的方法的
     		-->
     		<dependency>
     			<groupId>com.imooc</groupId>
     			<artifactId>foodie-dev-pojo</artifactId>
     			<version>1.0-SNAPSHOT</version>
     		</dependency>
     	</dependencies>
     	
     pojo的依赖：
     	<dependencies>
     		<dependency>
     			<groupId>com.imooc</groupId>
     			<artifactId>foodie-dev-common</artifactId>
     			<version>1.0-SNAPSHOT</version>
     		</dependency>
     	</dependencies>
     ```

  4. 子模块之间的依赖需要 install 成功之后才会真正生效
  
  5. 运行前，代码更改或依赖更改，需要 install 

