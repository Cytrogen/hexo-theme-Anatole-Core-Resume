# hexo-theme-Anatole-Core-Resume

[ENGLISH](README-en.md)


## 关于主题

本主题基于mrcore的[hexo-theme-Anatole-Core](https://github.com/mrcore/hexo-theme-Anatole-Core)主题进行了更倾向于简历的魔改。

### 本主题的特点：

- 超简约（指只有一个主页，删除了大量的功能）
- 根本没有写完！之后再说！
- 目前功能更倾向于国外的使用习惯（比如支持添加linkedin账户而移除了原主题里支持添加的知乎账户）

如果需要上传证书照片，可以使用以下Markdown语法来自动设置照片的尺寸：

```markdown
![CERTI](图片链接)
```

## 外观

DEMO：https://hexo-theme-anatole-core-resume.netlify.app


## 使用

### 安装
```bash
# 在博客根目录下克隆该仓库至themes文件夹、修改文件夹名为anatole-core-resume
git clone https://github.com/Cytrogen/hexo-theme-Anatole-Core-Resume.git themes/anatole-core-resume

# 安装pug渲染器
npm install hexo-renderer-pug --save
```

### 配置

修改hexo根目录下的 `_config.yml` ： `theme: anatole-core-resume`

其他需要配置的地方请看 `themes/anatole-core-resume/_comfig.yml`

> 鉴于还没写完，侧边栏的个人信息需要手动去 `themes/anatole-core-resume/layout/_partial/sidebar.pug` 里修改。
> 红豆泥狗咩纳塞……之后再说！


## 许可证

[MIT License](LICENSE)

## 其他

和原主题的作者一样，我也不是前端工作者，也是现学现改。如果往后发现了更好的代码优化方法，我会尽量改进。

当然，自己动手，丰衣足食~

### 11/29/2023

- 更新了`package.json`中的依赖版本
- 添加了对图片尺寸的自动调整功能

### 09/04/2023

- 添加了网页图标
- 修改了 `languages/` 下的语言文件，后续会改回来
- 修改了配置文件内的内容，添加了个人信息的配置项
- 修改了导航栏的显示逻辑。现在是基于博客根目录下的 `source/_post` 内的 markdown 文件的 `title` 属性来自动调整导航栏的显示内容
- 修改了导航栏的导向逻辑。现在在点击导航栏的某一项时，会自动滑向主页的对应部分
- 修改了主页面对博客文章的显示。原主题中默认是仅显示摘要，现在为了更好地展示简历，改为显示全文
- 修改了主页面中博客文章的标题显示。原主题中默认使用 `<a>` 来包裹标题，现在改为直接显示标题
- 修改了侧边栏的背景颜色为深蓝色
- 修改了侧边栏在移动端下的高度，使其完全占据屏幕高度
- 修改了侧边栏的内容。原主题中仅会显示社交账号的图标，现在改为也会显示手机号码、住址、社交帐号的内容来让网页看上去更像简历
- 修改了主页内容的响应式布局逻辑，以便在桌面端和移动端窗口大小发生变化时，页面能够更好地适应不同的屏幕大小
- 修改了copyright的年份
- 修改了网页的标题为 `个人姓名's Resume`
- 修改了 `layout/partial/layout.pug` 中的排序逻辑（实际上可能没有变化，后续可能会改回来）
- 移除了valine评论功能
- 移除了百度统计和tag词云
- 移除了标签功能
- 移除了文章中的收藏和分享功能
- 移除了归档、留言板、关于页面
- 移除了live2d展示和aplayer播放器，以及 `package.json` 中对应的依赖
- 移除了公安备案