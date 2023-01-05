配置：

    name:git config --global user.name "zhuhongliang"

    email: git config --global user.email "541546904@qq.com"

使用git:

    git status

        -查看当前仓库状态

    git init

        -初始化仓库

        未跟踪 ---->  暂存

            git add <filename>    将文件切换到暂存状态

            git add *    将所有已修改的文件暂存

        暂存 --->  未修改

            git commit -m "描述"    将文件存储到仓库中

            git commit -a -m "xxx"    提交所有已修改的文件

        未修改 ---> 修改

            修改代码后变成修改状态
