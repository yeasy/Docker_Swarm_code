# 整体结构

源代码主要分为 7 个目录和若干文件：
contrib，devstack，doc，etc，magnum，specs 和 tools。
除了这 7 个目录外，还包括一些说明文档、安装需求说明文件等。

## contrib
主要包括一个 templates 目录，给出了实现一个 Bay Template 的例子。

## devstack
包括将 Magnum 集成到 devstack 中的若干工具和文档。

## doc
包括使用 Sphinx 生成文档的相关源码。

## etc
跟服务和配置相关的文件，基本上该目录中内容在安装时会被复制到系统的/etc/ 目录下。

## magnum
项目核心的代码实现都在这个目录下。
可以通过下面的命令来统计主要实现的核心代码量。
```
find magnum  -name "*.py" | xargs cat | wc -l
```
目前版本，约为 46k 行。

## specs
项目提出时候的提案文档。

## tools
一些相关的代码格式化检测、环境安装的脚本。

## 其它文档
* README.rst：介绍了项目的情况和连接。
* TESTING.rst：介绍如何进行开发后的测试。官方配置的 jenkins 当 gerrit 上有代码提交 review 的时候会触发 tox 测试。实际上，OpenStack 中的项目使用 [tox](http://tox.readthedocs.org/en/latest/) 来管理测试的虚拟环境，使用 [testr](https://wiki.openstack.org/wiki/Testr) 来管理运行测试案例的顺序。
* Dockerfile：生成一个 Docker 镜像，默认里面运行 Mangum-api 服务。
