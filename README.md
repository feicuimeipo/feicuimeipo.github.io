# hexo 建的网站



D:\favorite-work\nx-web-site\nianxi_blog



# 安装配置



## 安装

- hexo
- node.js (version <= 10.13，建议10.12)
- 安装nodes.js ...
- 安装hexo

```bash
npm install hexo  #博主安装
或者
npm install hexo-cli g  #推荐
```

- 配置环境变量

bash echo'PATH="$PATH:./node_modules/.bin"'>> ~/.zshrc source ~/.zshr



## 选定建站的工作目录

在指定的目录下运行如下文件

```bash
hexo init [文件夹名称]   #新建一个网站 hexo init blog
cd [文件夹名称]          #进入网站目录
hexo s                 #启动服务器
```



以上是最简建站方法



## 选择主题

(略)



# 部署我们的项目到github



### 首次部署

hexo clean

hexo deply

hexo s #运行，http://localhost:4000/  访问



### 重新部署

```text
hexo clean  && hexo g --d
# hexo g 命令可以编译博客文件，生成要部署到远程服务器的文件。 hexo d 命令是执行部署操作。 hexo g -d 是将这两个命令的合在一起使用，编译后直接部署。通常出现这个就是成功了。

hexo s #运行
```



发布到githug

1. hexo clean && hexo g  -d 
2. git add * && git commit -m 'update‘
3. git push (git push -u origin main)





