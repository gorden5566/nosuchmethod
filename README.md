# nosuchmethod

1. 切换到 `init` 分支，执行 `mvn clean install` 编译并将 `common`、`sdk` 的 `1.0-low-RELEASE` 版本安装到本地仓库

2. 切换到 `update` 分支，执行 `mvn clean install` ，然后找到 `client` 模块下的 `com.gorden5566.Test` 类，运行其 `main` 方法，不出意外的话你将看到如下报错

```java
Exception in thread "main" java.lang.NoSuchMethodError: com.gorden5566.ShapeUtil.show(Lcom/gorden5566/Shape;)V
	at com.gorden5566.ShowUtil.show(ShowUtil.java:9)
	at com.gorden5566.Test.main(Test.java:9)
```  
