# Maven 仓库镜像加速配置

使用阿里云镜像源进行配置，Maven settings.xml 文件参考如下

```markup
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
          xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                      http://maven.apache.org/xsd/settings-1.0.0.xsd">
    <localRepository/>
    <interactiveMode/>
    <usePluginRegistry/>
    <offline/>
    <pluginGroups/>
    <servers/>
    <mirrors>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>Aliyun public repository</name>
            <url>https://maven.aliyun.com/repository/public</url>
        </mirror>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>Aliyun Google repository</name>
            <url>https://maven.aliyun.com/repository/google</url>
        </mirror>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>Aliyun Apache respository</name>
            <url>https://maven.aliyun.com/repository/apache-snapshots</url>
        </mirror>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>Aliyun Spring respository</name>
            <url>https://maven.aliyun.com/repository/spring</url>
        </mirror>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>Aliyun Spring plugin respository</name>
            <url>https://maven.aliyun.com/repository/spring-plugin</url>
        </mirror>
    </mirrors>
    <proxies/>
    <profiles/>
    <activeProfiles/>
</settings>
```

