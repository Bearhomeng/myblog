title: "hexo部署时git没有任何文件上传"
date: 2015-05-16 11:31:25
tags: hexo
---
跟着网上教程搭建hexo的时候碰到一个问题
当我使用

	$ hexo d

部署hexo的时候，我的gitpage怎么都没反应

然后我捣鼓了半天，都没搞明白怎么回事

后来发现我这里生成的没有`.deploy`目录，只有一个`.deploy_git`目录。然后手动改名

	$ mv .deploy_git .deploy

重新部署，发现就好。真是无语了，暂时不知道什么缘故。