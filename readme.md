# GIT使用

工作区 - 暂存区 - 本地仓库

1. 在电脑上创建一个文件夹作为工作区
2. 打开文件夹右键 git base here 进入当前目录
3. 工作区持有项目实际文件

## readme 文档
1. readme文件可以是txt文档，也可以是md文档

## 全局配置
1. 配置用户名：
2. 配置用户邮箱：

## 初始化
1. git init 初始化版本库
2. 当前目录路径后面有（master）代表初始化成功
3. 在当前目录下会生成一个隐藏文件 .get 代表这是一个版本库
4. 千万别操作 .git 文件，让他隐藏 不管他

## 工作区内容提交到本地仓库
1. 执行命令 git add 文件名 将工作区的内容提交到暂存区
2. 命令 git add . 将所有变动（新增、修改、删除）提交到暂存区
3. 从暂存区提交到本地仓库 git commit -m '提交注释'

## 版本回退
1. 命令：git reset --hard HEAD^ 回退到上一个版本（一个^代表上一个版本）
2. 命令：git reset --hard 版本号 回退到指定版本

## 辅助命令
1. 命令 git status 查看当前目录下的操作
2. git log 查看日志
3. git reflog 查看简版日志

## 将本地仓库提交到远程仓库
1. 在githup创建一个远程仓库
2. 本地工作区先提交到本地仓库
3. git remote add origin https://github.com/zxl082674/Git-Test.git
4. git remote -v  查看本地仓库所关联的远程仓库地址
5. git push -u origin master 第一次执行
   git push  把本地仓库推送到远程仓库
   -u origin master 设置默认提交
6. git push -u -f origin master 强制推送到远程，不推荐！！！

## 下载项目到本地
1. 克隆项目：git clone 项目远程仓库地址 整个版本库克隆下来
2. git clone 适用于本地没有该项目，直接从远程下载到本地
3. 一定要先把工作区的修改到本地仓库再更新远程到本地
4. 切换分区
   git pull
   
  
远程仓库修改
