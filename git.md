### 安装git

windows直接到官网下载git安装。

安装完成后，点击右键会有Git Bash选项，可打开git命令窗口。

```g
git config --global user.name 'name'
git config --global user.email 'email'
```

上面两行命令可以设置用户名和邮箱。`--global`表示在全局范围设置。



### 创建版本库

```
mkdir learngit
cd learngit
pwd
```

上面三行代码依次表示 创建learngit文件夹、进入learngit文件夹、显示当前路径。

然后再输入命令`git init`可以创建git仓库。

在当前仓库文件夹中新建文件，例如创建一个readme.md文件，然后通过以下代码可以将其添加到版本库：

```
git add readme.md
git commit -m 'message'
```

`git add`可以将指定文件添加到暂存区，`git commit`可以将暂存区的文件添加到版本库中，`-m`指令表示为此次提交添加备注。

### 查看工作区状态

`git status`命令可以随时查看工作区当前的状态，可以查看当前所在的分支、文件提交状态等等。

`git diff`命令可以查看指定文件的更改信息。例如：`git diff readme.md`。



