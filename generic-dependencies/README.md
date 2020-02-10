# generic-dependencies
## 模块简介
本模块提供通用的 Maven Bom 文件，目的在于提供良好的依赖管理，减少不必要的依赖冲突。
该 Bom 文件主要源于以下两个 Bom 文件 
- `spring-boot-dependencies`
- `spring-cloud-dependencies`
这两个 Bom 文件提供和管理了大量的开源软件版本号，方便了我们引入依赖，也减少了依赖冲突的发生。

## 版本说明
本模块的版本号和 Spring Boot 的 RELEASE 版本号保持一致。

## 使用说明
和大多数 Bom 一样，引入以下下依赖即可：
```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>com.idukelu.generic</groupId>
            <artifactId>generic-dependencies</artifactId>
            <version>${reversion}</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```
