# Ich'en — Research & Chinese blog

纯静态 GitHub Pages 主页，无外部依赖。默认 Side A，`#b` 直达 Side B，小按钮在两面间切换。

- Side A 恢复原研究主页排版，仅保留用户指定的 ongoing transfer learning 项目。
- Side B 使用独立的黑色博客排版：居中站名、文章列表导航、按年份分组的日期／标题／分类列表。
- 不包含评论区、留言板或评论服务。目前文章列表为空。

## 添加文章

1. 新建 `writing/slug.html`，写入文章全文，返回链接使用 `../index.html#b`。
2. 编辑 `index.html` 脚本顶部的 `posts` 数组，添加真实文章：

```js
const posts = [
  // {title: '文章标题', date: 'YYYY-MM-DD', category: '随笔', url: 'writing/slug.html'}
];
```

日期必须为实际发布日，链接使用相对路径。页面会按年份和日期倒序生成目录；无文章时显示“暂无文章”。
项目内容直接编辑 `#transfer-learning`，状态按实际进度更新。

## 发布

保留 `main / (root)` 和 `.nojekyll`。

- https://ycwsop.github.io/ichen.github.io/
- https://ycwsop.github.io/ichen.github.io/#b
