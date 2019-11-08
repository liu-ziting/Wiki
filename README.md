# wiki

## 项目介绍

> wiki基于GitBook搭建的知识库管理，用于记录碎片化的代码片段，文章集合，破解软件下载地址等等，持续更新中...

* 如果对您对此项目有兴趣，可以点 "Star" 支持一下！

* 或者您可以 "follow" 一下，如有问题请直接在 Issues 中提

* 传送门：[wiki][1] --项目部署于GitPage

----------


### 产品依赖于:
 - [GitBook][2]
 - [NodeJS][3]


## 项目运行

    # 克隆到本地
    git clone https://github.com/liu-ziting/Wiki.git
    
    # 进入文件夹
    cd Wiki
	
    # 安装依赖
    gitbook install
	
    # 开启本地服务器
    gitbook serve
    
    # 发布环境(打包成静态文件_book)
    gitbook build

## 项目目录结构
```
Wiki
├── book.json		配置文件数据(可选)
├── README.md		简介-书籍的简单介绍(必填)
├── SUMMARY.md		文章目录配置
├── AboutUs.md		介绍
├── style		自定义css
├── docs		打包生成的文件夹
└── page		存放单个文件（章节）

```		

## 项目从零开始构建

使用NPM全局安装

```	
$ npm install gitbook-cli -g
```	
创建一本书

```	
$ gitbook init

```	

如果你想用现有的目录来创建一本书，你可以通过运行
```	
$ gitbook init ./directory

```	
预览您创建的图书
```	
$ gitbook serve

```	
构建静态网站
```	
$ gitbook build
```	

详情见[gitbook中文文档][4]

  [1]: http://wiki.lihail.cn
  [2]: https://www.gitbook.com/
  [3]: http://nodejs.cn/
  [4]: http://gitbook.hushuang.me/