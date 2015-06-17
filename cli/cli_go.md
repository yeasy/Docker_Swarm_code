## cli.go
实现了一个 Run 方法。

生成一个新的应用 app，然后传递执行的命令和参数，调用应用中的 Run 方法。

```go
if err := app.Run(os.Args); err != nil {
		log.Fatal(err)
	}
```

