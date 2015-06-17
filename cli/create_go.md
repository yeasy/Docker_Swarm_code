## create.go

create 方法，对应执行 create 命令。通过 token 来初始化一个 discovery，然后创建一个集群。

```go
func create(c *cli.Context) {
	if len(c.Args()) != 0 {
		log.Fatalf("the `create` command takes no arguments. See '%s create --help'.", c.App.Name)
	}
	discovery := &token.Discovery{}
	discovery.Initialize("", 0, 0)
	token, err := discovery.CreateCluster()
	if err != nil {
		log.Fatal(err)
	}
	fmt.Println(token)
}
```

