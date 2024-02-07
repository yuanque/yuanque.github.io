# 圆缺的站点

## 准备环境

在这里下载 VSCode:

https://code.visualstudio.com/Download

在这里下载 git 程序：

https://git-scm.com/downloads

在这里下载 hugo_extended_xxxx_windows_adm64.xxx 的文件，解压后使用：

https://github.com/gohugoio/hugo/releases/tag/v0.122.0

第二步是下载这个仓库的文章：

```bash
git clone git@github.com:yuanque/yuanque.github.io.git
```

然后进入到 yuanque.github.io 这个文件夹中，使用这个命令下载网站主题：

```bash
cd yuanque.github.io
git submodule update --init
```

先准备一下文章作者的信息：

```bash
git config --global user.email "1196518478@qq.com"
git config --global user.name "Yuan Que"
```

## 使用方法

创建新文章：

```bash
hugo new posts/2024/02/ggg/index.md
```

创建完成后，就可以在 content/posts 文件夹中找到并编写你的文章内容。

编写时，随时可以使用这个命令预览网站效果：

```bash
hugo server --buildDrafts
```

编写完毕后，使用这个命令发布新的文章：

```bash
git add .
git commit -am "new post"
git push
```
