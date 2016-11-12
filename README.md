# Gcs-Vno-Jekyll

基于 Jekyll 的个人博客主题。

## 样式预览

![](http://ww4.sinaimg.cn/large/005Xtdi2jw1f9pvpcwm0rj313y0maade.jpg)

### [点击这里查看实际部署效果](http://www.gcssloop.com/)

## 使用方法

1.如果是使用 GitHub Pages 则直接复制该文件到对应仓库的对应分支即可，发布完成后，过几分钟就能在对应的网址看到效果了。

2.如果需要本地调试预览，则需要在本机安装 Ruby，并配置好 Jekyll 环境，环境配置方式自行搜索。

3.文章应放在 `_posts` 目录下，并按照 `year-month-day-filename.md` 的格式命名。

4.配置文件为 `_config.yml`， 这个就不用多说了吧。

## 可选功能

#### 1.本地调试方法

本机环境配置完成后，在命令行中进入该文件夹根目录，输入 `jekyll server` 稍等片刻就能在 <http://localhost:4000> 看到效果了。

#### 2.添加文章评论

到 [多说官网](http://duoshuo.com/) 申请一个账号，之后将自动生成的代码复制到 `/_includes/comments.html` 文件中即可。

注意修改自动生成代码中的url，多说中会有提示，示例写法：

``` html
 <div id="comments" class="ds-thread" data-thread-key="{{page.id}}" data-title="{{page.title}}" data-url="{{site.url}}{{page.url}}"></div>
```

#### 3.博文置顶

在文章最上面添加 `istop: true` 属性会让该博文置顶显示，但该文章原始位置依旧会显示，这就意味址如果你置顶了第一页的文章，你会在第一页看到两篇文章。

如果想要修改博文置顶的逻辑可以在 `index.html` 文件中修改。

#### 4.站内搜索

目录页面的站内搜索实际上是利用了 Google 搜索的一个特性，如果想要删除或者修改都可以，文件中有注释。

不要问我为什么不用百度，因为百度收录速度太慢了，经常收录不全。 ╮ (￣ 3￣) ╭

#### 5.站点地图

站点地图会自动生成，地址为 `域名/sitemap.xml`，建议将该地址提交给搜索引擎，方便引擎快速抓取收录你的页面。

#### 6.多链接访问

有时修改文章标题，分类会使原始链接丢失，可以使用 `redirect_from` 属性将原始链接重定向到新链接地址。

``` yml
redirect_from:
  - /1970/01/about/
```

#### 7.SEO优化

为了增加你博文被搜索到的概率，可以考虑使用 SEO 优化，我定义了两个属性，`keywords` 和 `excerpt` ：

``` yml
keywords: GcsSloop, gcssloop
excerpt: 我是 GcsSloop， 一名生活在2.5次元的魔法师，平时研究一下魔法，做一些魔法卷轴，也会把一些研究成果贡献出来，以帮助新入门的魔法师更快速的成长为高级魔法师。点击此处查看我公布的魔法研究成果。
```

**关于文章开头常用的属性示例可以参考 `1970-01-01-about.md` 文件。**


## Licence

本主题是基于 onevcat 大神的 [OneV-s-Den](https://github.com/onevcat/OneV-s-Den) 修改而来的，非常感谢 onevcat 以及之前作者作出的贡献。

Great thanks to [Dale Anthony](https://github.com/daleanthony) and his [Uno](https://github.com/daleanthony/uno). Vno Jekyll is based on Uno, and contains a lot of modification on page layout, animation, font and some more things I can not remember. Vno Jekyll is followed with Uno and be licensed as [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/). See the link for more information.


