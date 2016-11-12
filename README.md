# Gcs-Vno-Jekyll

基于 Jekyll 的个人博客主题。

## 样式预览

![](http://ww4.sinaimg.cn/large/005Xtdi2jw1f9pvpcwm0rj313y0maade.jpg)

### [点击这里查看实际部署效果](http://www.gcssloop.com/)

## 使用方法

1.如果是使用 GitHub Pages 则直接复制该文件到对应仓库的对应分支即可，发布完成后，过几分钟就能在对应的网址看到效果了。

2.如果需要本地调试预览，则需要在本机安装 Ruby，并配置好 Jekyll 环境，环境配置方式自行搜索。

3.文章应放在 `_post` 目录下，并按照 `year-month-day-filename.md` 的格式命名。

## 注意事项

### 1.添加文章评论

到 [多说官网](http://duoshuo.com/) 申请一个账号，之后将自动生成的代码复制到 `/_includes/comments.html` 文件中即可。

### 2.本地调试方法

本机环境配置完成后，在命令行中进入该文件夹根目录，输入 `jekyll server` 稍等片刻就能在 <http://localhost:4000> 看到效果了。



本主题是基于 onevcat 大神的 [OneV-s-Den](https://github.com/onevcat/OneV-s-Den) 修改而来的。
