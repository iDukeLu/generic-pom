# generic-parent
## 项目简介
本模块提供通用的 Maven Parent 文件，目的在于减少每次构建项目时重复的配置工作。该 Maven Parent 主要提供了：
- 通用的属性配置：UTF8 的编码格式，1.8 的 Java 版本
- 常用的仓库配置：阿里云仓库、jcenter 仓库、google 仓库、central 仓库
- 常用的开源软件版本号管理：由 `generic-dependencies` 提供依赖管理

## 版本说明
本项目的版本号和 Spring Boot 的 RELEASE 版本号保持一致

## 使用说明
作为父依赖引入即可：
```xml
<parent>
    <groupId>com.idukelu.generic</groupId>
    <artifactId>generic-parent</artifactId>
    <version>2.2.2.RELEASE</version>
    <relativePath/>
</parent>
```
