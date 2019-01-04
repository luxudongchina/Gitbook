# Gitbook 本地写书并部署至 GitHub Pages

GitBook 是一个基于 Node.js 的命令行工具，可使用 Markdown 来制作精美的电子书。但目前Gitbook改版之后，资料文档使用的是 Digital Ocean 的主机，而 DO 家的很多地址被墙了，导致往往无法访问。因此在线使用Gitbook写书就变得不方便了，这篇文档介绍利用Gitbook本地写书，再将编写好的.md文件通过Gitbook处理成静态网站。将md文件与Github Pages静态文件存放在一个仓库中。md文件为master分支，而html文件为 gh-pages分支。这样不但能共享，而且还能进行多人协作。

GitHub Pages 简单说就是一个可以托管静态网站的 Git 项目，支持使用 markdown 语法以及 Jekyll 来构建，或者直接使用已经生成好的静态站点。

由于 Gitbook 书籍可以通过 Gitbook 本地构建出 html  格式，所以可以直接将构建好的书籍直接放到 GitHub Pages 中托管，之后，可以通过如下地址访问书籍：

&lt;username&gt;.github.io/&lt;project&gt;

例如：这本书可以通过地址：

[https://luxudongchina.github.io/Gitbook/ ](https://luxudongchina.github.io/Gitbook/)来访问。

