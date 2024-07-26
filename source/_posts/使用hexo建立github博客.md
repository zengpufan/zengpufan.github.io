---
title: 使用Hexo建立Github博客
date: 2024-07-22 11:49:37
tags:
---

## 摘要
本文主要介绍通过hexo框架搭建个人博客，并将博客部署到github平台上。
## 所需技术简介
1. Hexo 是一个快速、简洁且高效的博客框架。 Hexo 使用 Markdown（或其他标记语言）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。
2. github pages
github pages可以针对一个github账号或者一个github仓库创建一个网页。  
github pages官网：https://pages.github.com/
## Hexo安装配置
1. 安装Node.js  
Node.js官网 https://nodejs.org/  
点击download即可   
![](使用Hexo建立Github博客/1.jpg)

1. 安装hexo  
   
   进入cmd，输入
    ```cmd
   npm install -g hexo-cli
    ```
    安装完成后，输入
    ```
    hexo -v
    ```
    查看是否安装成功
    ![](使用Hexo建立Github博客/2.jpg)

1. 初始化hexo  
    创建一个空的项目文件夹，进入cmd，输入以下命令    
    ```py
    hexo init  
    ```
    如下图所示，hexo项目创建成功  
    ![](使用Hexo建立Github博客/3.jpg)  
      
    Hexo的初始项目结构如下:  
    ![](使用Hexo建立Github博客/4.jpg)  
    ```py
    _config.yml 
    # 该文件是网站的配置档案，网站的配置基本上写在这里，后面会详细说明
    package.json 
    # 依赖包的配置文件
    scaffolds 
    # 模板文件夹，新建文章时，Hexo会根据scaffold创建文件夹 
    source 
    # 资源文件夹，用来存储用户资源的地方（一般指文章的原稿和相关图片资源）
    # 除 _posts 文件夹之外，开头命名为 _ (下划线)的文件 / 文件夹和隐藏的文件将会被忽略。 # Markdown 和 HTML 文件会被解析并放到 public 文件夹，而其他文件会被拷贝过去。
    themes 
    # 主题文件夹。 Hexo 会根据主题来生成静态页面
    # 主题文件夹规定网站的样式，模板文件夹规定文章的排版
    ```

2. Hexo快速开始  
   输入“生成指令”
   ```py
   hexo generate
   ```
   可以将markdown文档转换为网页  
  
   输入启动服务器指令
   ```py
   hexo server
   ```
   即可启动服务器，看到初始网站的样式
   ![](./使用Hexo建立Github博客/5.jpg)