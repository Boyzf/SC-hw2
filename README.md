# 安装go语言开发环境
## 安装vscode

在ubuntu的应用商店中找到vscode，直接下载即可。
！[]()

## 安装golang

在终端输入命令“sudo apt-get install golang”即可安装golang。
使用命令“go version”即可检验是否安装成功。
！[]()

## 设置环境变量

用指令“sudo vim ~/.bashrc”打开bashrc文件，在文件末尾输入以下指令 -p
export GOPATH=~/go_workspace # 工作包的位置 -p
export PATH=$PATH:$GOPATH/bin

## 完成第一个程序

创建一个目录：$ mkdir -p $GOPATH/src/github.com/user
在目录中选择包路径：$ mkdir $GOPATH/src/github.com/user/hello

创建 hello.go 文件
！[]()

输入以下代码：
！[]（）

运行代码，结果如下：
！[]()

go 工具构建并安装此程序了:
![]()

## 创建第一个库

选择包路径并创建包目录，在目录下创建一个名为 reverse.go 的文件：
![]()

在文件中输入以下代码：
![]()

使用命令“go bulid”来测试包的编译。

将原来的 hello.go 文件修改成如下代码：
![]()

使用命令“go install”对程序进行安装，之后可以运行程序。

## 测试

在 stringutil 目录下新建一个 reverse_test.go 文件来进行测试，在文件中输入以下代码：
![]()

使用“go test”运行该测试。

## 远程包

运行以下指令即可：
$ go get github.com/golang/example/hello
$ $GOPATH/bin/hello
