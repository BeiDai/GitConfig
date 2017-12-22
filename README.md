# Git_Config

简述：git的配置与一些常用命令

- [git文件配置](.gitconfig)

- [本地用户名邮箱](README.md#本地用户名邮箱)

- [上传本地仓库](README.md#上传本地仓库)
- [同步远程仓库](README.md#同步远程仓库)
- [克隆远程仓库](README.md#克隆远程仓库)
- [SSH协议配置](README.md#SSH协议配置)
- [git常用命令](README.md#git常用命令)
- [git命令扩展](README.md#git命令扩展)


### 本地用户名邮箱

    git config --list

    git config --global user.name "BeiDai"

    git config --global user.email " "

    cat .gitconfig

    git log

### 上传本地仓库
    git init

    git status

    git add XXX/ 或 .

    git commit -m "XXXX"

    git commit -a -m "XXX"

    git show 哈希码

    git remote add origin https://github.com/xxx/xx.git

    git remote -v

    git push -u origin master

### 同步远程仓库
    git pull origin master

### 克隆远程仓库
    git clone https:\\github.com\XXX\XXX

### SSH协议配置
    ssh-Keygen -t rsa -C "emailadress"

    ls ~/.ssh/

    cat id_rsa.pub

    复制到git服务端 SSH Keys

### git常用命令
    git

    git help -a

    git blame 文件名    //查看变更记录

    git blame -L 5,10 文件名 //从第五行到第十行

    git clean -n    //列出没有放到暂存区的文件

    git clean -f    //删除没有列到暂存区的所有文件

    git clean -x -f //删除被.gitignore忽略的文件

    git status -sb  //简化查看信息量

### git命令扩展
    git rm 文件名 // rm 文件名  //删除文件

    git mv a b //把a名改为b

    git mv b  ./xx  //把b移动到xx文件夹

    git diff //查看文件变更

    git add -p  // 按文件版本提交  y分割提交

    git diff --cached

    git show HEAD^
