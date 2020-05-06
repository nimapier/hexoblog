---
title: 将hexo博客项目托管到GitHub上
date: 2019-07-05 13:19:45
tags:
catagory: hexo
---
七月的第一天从实习了将近五个月的公司离职了，公司电脑上的项目不多，都托管到了GitHub上，唯独hexo的博客项目有些不太一样。
参考文章地址：{% blockquote %}
<https://juejin.im/post/5acf22e6f265da23994eeac9>
{% endblockquote %}
在同一个项目下新建hexo分支备份博客部署文件，master分支保持不变，依然用于保存博客静态资源，提供博客页面供人访问。
上传部署文件时由于没有更新主题，主题文件中的package-lock.json上传到GitHub时上报了security错误，修改后上传成功。
在新电脑上clone hexo分支，安装hexo，执行npm install，再使用hexo指令hexo g，hexo server，均没有问题。添加本文后执行hexo d，成功部署到master分支，迁移完成。