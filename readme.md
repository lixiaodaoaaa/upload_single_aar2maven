##  项目使用说明

 > 本项目用于将单独的aar文件上传到maven仓库。本工程默认是上传到本地nexus空间。默认地址为：[http://127.0.0.1:8081/nexus/content/groups/public/](http://127.0.0.1:8081/nexus/content/groups/public/) 有需要的可以用此工程将aar发布到maven仓库中。SNAPSHOT文件不支持手动上传可以用此工具 上传哦！
 需要将上传的文件copy到aar目录下，更改相应的build.gradle文件即可。

*  支持 aar 文件上传
*  支持 aar snapshot版本上传

## 项目分支说明：
|  分支名称      |  说明       | 备注  |
| ------------- |:-------------:| -----:|
| master        | 主要分支 | 目前项目在master分支 |
| develop    | 开发分支 |   feat分支的东西 过来merge |
| feat/uplaodtest | feat 分支 成功后 移动到develop分支      |   已上传成功 |



## 项目配置需求

* java 8 环境、gradle环境 最好配置gradle 环境变量 方便运行您的项目！配置环境变量我就不多说了。
   最好使用AndroidStudio 打开此项目

* 本地有maven仓库服务器 或者 有私服 maven服务器
* 电脑为mac 或者windows 本作者刚好用了 mac  ^_^
* 需要在gradle.properties里配置 上传的用户名和密码及url。我已配好。

* 用AndroidStudio打开此项目然后将需要上传的aar copy到aar目录下。

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
***
![到maven私服查看如下](http://owx00rmbo.bkt.clouddn.com/up_nexus.png)

## 任何问题 请通过如下方式联系我：
 * http://www.weibo.com/lixiaodaoaaa
 * lixiaodaoaaa@126.com
