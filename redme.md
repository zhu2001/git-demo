配置：

    name:git config --global user.name "zhuhongliang"

    email: git config --global user.email "541546904@qq.com"

使用git:

    git status

        -查看当前仓库状态

    git init

        -初始化仓库

    文件状态：
        1.未跟踪
        2.已跟踪
        3.暂存
        4.未修改
        5.已修改

        未跟踪 ---->  暂存

            git add <filename>    将文件切换到暂存状态

            git add *    将所有已修改的文件暂存

        暂存 --->  未修改

            git commit -m "描述"    将文件存储到仓库中

            git commit -a -m "xxx"    提交所有已修改的文件

        未修改 ---> 修改

            修改代码后变成修改状态

常用命令

```
文件重置
    git restore <filename>    将工作区的文件恢复到暂存区的样子
    git restore --staged <filename>    将暂存区的文件恢复到仓库中的样子
删除文件
    git remove <filename>
    git remove <filename> -f 强制删除
```

移动文件

```bash
git mv <from> <to> #移动文件 重命名文件
```

#### 分支

git在存储文件时，每一次代码的提交都会创建一个与之对应的节点，git通过一个一个节点来记录代码的状态的。节点会形成一个树状结构，默认只有一个分支，命名为master

```bash
查看分支 git branch

创建新的分支 git branch xxx 

删除分支 git branch -d xxx

切换分支 git switch xxx

创建并切换分支 git switch -c <branch name>

合并分支 git merge <要合并的分支名> 在主分支下执行该命令
```

#### 变基

在开发中除了通过merge来合并分之外，还可以通过变基来完成分支的合并。

```bash
git rebase
```