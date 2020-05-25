### beego

官网：beego.me

beego的hello很简单

```go
import "github.com/astaxie/beego"
func main()  {
	beego.Run()
}
```



### bee

```go
go get 	github.com/beego/bee
```

安装完成后，检验

* GOPATH下面的 bin目录下看到bee的二进制可执行文件，
* 也可以在GOPATH中的src/github.com/beego/bee/中看到bee的源代码

执行bee命令，现实帮助文档

<img src="/Users/dxm/Library/Application Support/typora-user-images/image-20200428071946910.png" alt="image-20200428071946910" style="zoom:50%;" />

bee生成beego的应用程序

```go
bee new hellobeebeego
```

如果遇到了下面的错

<img src="/Users/dxm/Library/Application Support/typora-user-images/image-20200428072350743.png" alt="image-20200428072350743" style="zoom:50%;" />

我们就是去设置一下GOPATH

<img src="/Users/dxm/Library/Application Support/typora-user-images/image-20200428073553693.png" alt="image-20200428073553693" style="zoom:50%;" />



mac中添加环境变量和linux中添加环境变量相仿，可以在当前用户下设置环境变量，也可以设置全局的环境变量

```bash
# 查看go的安装情况
go env

# 编辑当前用户的环境变量
vim ~/.bash_profile

# 加入如下内容
export GOPATH=/Users/chenxingyi/work/go	# go的开发目录
export PATH=$PATH:${GOPATH//://bin:}/bin

# 让配置文件立即生效
source ~/.bash_profile
```

















