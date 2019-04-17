原文：https://my.oschina.net/yangjianzhou/blog/1836031
官方：https://github.com/mybatis/generator


由于博主贡献给官方的代码，截至2019年4月17日还没有发布新版本。如果有急需修改Example目录而且不想手工修改重复打包的懒人朋友可以下载这个临时用用。如果有新版本发布还是用官方的好（官方大于1.3.7的版本一定就包含了此功能）。

```
注：楼主提交的代码在官方版本中是给javaModelGenerator节点添加<property name="exampleTargetPackage" value="example"/>属性实现分离的。


<javaModelGenerator targetPackage="model" targetProject="src/main/java">
	<property name="enableSubPackages" value="true"/>
	<property name="trimStrings" value="true"/>
	<property name="exampleTargetPackage" value="example"/>
</javaModelGenerator>
```