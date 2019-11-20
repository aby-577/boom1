# git 笔记： http://note.youdao.com/noteshare?id=82594d8e6b22d52e8d3b29dc64b613e0

# 第一个仓库
1. `git init` 用于初始化仓库

2. 新建一个readme.md文件

3. `git add 文件名` 添加文件到本地仓库
```
git add .   //添加所有文件
```

4. 添加用户名和邮箱(第一次的时候需要)
```
git config --global user.email '你的邮箱'
git config --global user.name '你的用户名'
```

4. 提交
```
git commit -m '注释' //注释是对本次提交的说明
```

5. 添加远程仓库地址
```
git remote add origin git@github.com:lizelong/ceshi.git
```
6. 将本地提交的内容推送到远程仓库
```
git push 远程仓库的别名 master
git push abc master
```

6. 没有权限，先生成ssh key
```
ssh-keygen -t rsa -C '邮箱'

执行完上一条命令后，会在 ~/.ssh/ 文件夹下面生成公钥文件 id_rsa.pub 
将公钥文件中的内容，放到GitHub中：
	右上角头像 -> settings -> SSH and GPG keys -> New SSH key
	title： 仓库名
	Key： id_rsa.pub 的内容
```




# 工作流程
1. 初始化本地仓库
2. 跟远程仓库建立连接
	git remote add 远程仓库的别名(origin) 远程地址
	git remote add origin git@github.com:lizelong/ceshi.git
3. 开发模块
4. 先添加所有文件
	git add .
5. 提交到本地仓库
	git commit -m '添加index.html'

git pull //拉取并合并

# github pages
目的： 为了更方便的查看HTML文件解析后的内容





# bootstrap 前端框架
## 官网 bootcss.com



# i love you 3000遍

# git push -u origin master  //-u 将origin设置为默认的远程仓库，下次再push的时候就可以不用加 origin 了

# http状态码
- 200  ok
- 404 没找到
- 403 没权限
- 500 服务器错误
- 301 永久重定向
- 302 临时重定向


### 扩展：
> 标题、列表、代码段、引用、粗体、斜体、图片、链接
#标题
##二级标题
-列表
-列表
```
代码
```
**粗体**
*斜体*

![图片](http://img4.imgtn.bdimg.com/it/u=3209370120,2008812818&fm=26&gp=0.jpg "图片")
[链接](https://note.youdao.com/ynoteshare1/index.html?id=82594d8e6b22d52e8d3b29dc64b613e0&type=note "链接")



### markdown预览快捷键绑定
```
//首选项 -> 按键绑定-用户
{ "keys": ["alt+m"], "command": "markdown_preview", "args": {"target": "browser", "parser":"markdown"} },
```