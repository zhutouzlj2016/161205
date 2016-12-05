- Workspace 工作区
- Index ／ Stage 缓存区
- Repository 仓库区／本地仓库
- Remote 远程仓库

mkdir <name>  创建一个目录
ls            查看当前目录下的文件及目录
ls -a         查看当前目录下的文件及目录，包含隐藏文件
cd <name>     进入指定目录
git init      初始化当前目录为git项目
git init <name> 创建 <name> 的文件夹，并初始化为git项目
git add .     提交工作区变更到缓存区
git commit -m 'msg' 提交缓存区到本地仓库
git config --global user.email 'email'  设置全局git提价邮箱
git config --global user.name 'name'    设置全局git提交用户名
git config --list                       查看当前项目git配置
git config --list --global              查看全局git配置
git config -e                           编辑当前项目git配置文件
git config -e --global                  编辑全局git配置文件
git status     查看当前git项目的文件变更


* 操作顺序
 ```
 //获取远程仓库代码
    git clone https://code.aliyun.com/tasktest/task2016.git
    
 //进入项目目录
    cd task2016
 
 //初次或用户信息发生变化时，才去执行
 //设置git 提交、下载用户名 --global 全局环境，不加则是这是本地环境
 git config --global user.name 'tasktest'
//设置 git 提交、下载邮箱 --global 全局环境，不加则是这是本地环境
git config --global user.email '596778373@qq.com'

//做文件的修改等任意操作

//提交到本地缓存
    git add .
    
//提交到本地仓库
    git commit -m '提交信息'

//推送到远程仓库
    // origin  远程分支名，  master 本地分支名
    git push origin master
    //https 模式链接下，需要输入git提价用户名以及密码
```
    



    