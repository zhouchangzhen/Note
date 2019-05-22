### Git命令

> #### 设置名字和邮箱

```shell
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```

> #### 初始化版本库

```shell
$ git init
```

> #### 添加文件、提交文件（必须是仓库目录内的文件）

```shell
$ git add <fileNmae>
$ git commit -m <Message>
```

> #### 查看工作目录暂存区的状态

```shell
$ git status
```

> #### 查看具体的修改内容

```shell
$ git diff <fileName>
```

> ####`git status`与`git diff`的区别

`git status`可以查看仓库内的哪些文件被修改了，`git diff`可以查看文件的具体修改了什么内容，需要注意的是，`git diff`命令只能修改你上一次`git add`与现在的文件的区别么，如果你修改之后使用`git add`添加了再使用`git diff`命令查询的话就不会提示任何内容。

> #### 查看`commit`记录

```shell
$ git log
```

`git log`命令的提示信息为最近的提交记录到最远的提交记录，即第一条为最后一次`commit`的内容，最后一条为第一次`commit`的内容(从上往下的顺序)