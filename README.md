# generic
## 项目简介
本项目为通用项目，目前主要提供 Maven 的通用 POM 文件，简化项目的构建流程。

## 模块说明
本项目主要包含了以下模块：
- generic-dependencies：通用的 Maven Bom 模块
- generic-parent：通用的 Maven Parent 模块

## 版本说明
本项目的版本号和 Spring Boot 的 RELEASE 版本号保持一致（由 reversion 属性决定）

## 升级说明
1. 修改 <revision> 的版本号为对应 Spring Boot 的 RELEASE 版本号
2. 上传私服和更新代码：
    ```
    mvn clean package deploy -Dmaven.test.skip=true
    git add *
    git commit -m "feature(all): update version"
    git push
    ```