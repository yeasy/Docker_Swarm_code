# Godeps
[godep](https://github.com/tools/godep) 是一套管理 Go 项目中依赖的工具，类似 Python 中通过 setup.py 或者 requirements.txt 来记录依赖信息。

它的使用十分简单。

保存当前项目使用的依赖信息：
```sh
$ godep save
```

基于保存的依赖库来构建项目

```sh
$ godep go install
```

或者

```
$ GOPATH=`godep path`:$GOPATH
$ go install
```
