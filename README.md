Docker Swarm 源码分析
============
[Swarm](https://github.com/docker/swarm) 是 Docker 官方推出的 Docker 容器集群管理项目。通过它，你可以在多个机器构建的集群上使用 Docker 容器，而无需关心具体被分配到哪台机器上。

本书将剖析 Swarm 组件的代码。

最新版本在线阅读：[GitBook](https://www.gitbook.io/book/yeasy/Docker_Swarm_code)。

本书源码在 Github 上维护，欢迎参与：[https://github.com/yeasy/Docker_Swarm_code](https://github.com/yeasy/Docker_Swarm_code)。

感谢所有的 [贡献者](https://github.com/yeasy/Docker_Swarm_code/graphs/contributors)。

## 更新历史:
* V0.1: 2015-06-17
	* 完成基本结构。


## 参加步骤
* 在 GitHub 上 `fork` 到自己的仓库，如 `user/Docker_Swarm_code`，然后 `clone` 到本地，并设置用户信息。
```
$ git clone git@github.com:user/Docker_Swarm_code.git
$ cd Docker_Swarm_code
$ git config user.name "User"
$ git config user.email user@email.com
```

* 修改代码后提交，并推送到自己的仓库。
```
$ #do some change on the content
$ git commit -am "Fix issue #1: change helo to hello"
$ git push
```

* 在 GitHub 网站上提交 pull request。
* 定期使用项目仓库内容更新自己仓库内容。
```
$ git remote add upstream https://github.com/yeasy/Docker_Swarm_code
$ git fetch upstream
$ git checkout master
$ git rebase upstream/master
$ git push -f origin master
```
