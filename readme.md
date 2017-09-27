##  项目使用说明

 > 本项目用于将单独的aar文件上传到maven仓库。本工程默认是上传到本地nexus空间。默认地址为：[http://127.0.0.1:8081/nexus/content/groups/public/](http://127.0.0.1:8081/nexus/content/groups/public/) 有需要的可以用此工程将aar发布到maven仓库中。SNAPSHOT文件不支持手动上传可以用此工具 上传哦！by : Dagger

*  支持 aar 文件上传
*  支持 aar snapshot版本上传

## 项目配置需求

* java 8 环境、gradle环境 最好配置gradle 环境变量 方便运行您的项目！配置环境变量我就不多说了。
   最好使用AndroidStudio 打开此项目

* 本地有maven仓库服务器 或者 有私服 maven服务器
* 电脑为mac 或者windows 本作者刚好用了 mac  ^_^
* 需要在gradle.properties里配置 上传的用户名和密码及url。我已配好。

## 运行说明
 * 可以在控制台运行 gradle copyAar
 此任务 是copy aar目录下的aar到build/libs下

 * 发布 aar可以使用
 ``` java
 gradle publish
 ```


或者
```
./gradlew publish
```

## 上传成功截图如下：
![项目运行结果如下](http://owx00rmbo.bkt.clouddn.com/publis_success.png)

![到maven 私服查看如下： ](http://owx00rmbo.bkt.clouddn.com/up_nexus.png)
