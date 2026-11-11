# Ich'en — Side A / Side B

GitHub Pages 个人主页。一个 HTML 文件，无构建步骤、无外部依赖。

- **Side A**：白色面，物理与研究，英文为主。旧版项目卡片已清空。
- **Side B**：黑色面，中文个人博客。文章区暂时为空。
- 顶部按钮与页面底部入口可切换两面，支持键盘、浏览器前进／后退和减少动态效果设置。
- 默认进入 Side A；地址添加 `#b` 可直接进入 Side B。
- 关闭 JavaScript 后，两面的内容会按顺序显示。

## 内容原则

只列真实开展的项目，不把兴趣、准备中的方向写成已完成工作。
2026-11-11 已移除旧项目卡片；以后添加项目的具体状态以用户确认的信息为准。
博客不放虚构文章、发布日期或无效下载链接。

## 更新项目

在 `index.html` 的 `#project-list` 中添加 `article.entry`：

```html
<article class="entry">
  <h3>真实项目标题</h3>
  <span class="entry-status">准确的实际状态</span>
  <p>具体做了什么，以及目前可展示的结果。</p>
</article>
```

如果有已公开材料，可为标题添加真实链接。暂时没有材料时，保持普通标题。

## 添加中文博客

1. 在仓库中新建 `writing/your-post.html`，写入文章全文；文章页可返回 `../index.html#b`。
2. 在 `index.html` 的 `#post-list` 中添加入口，使用相对路径：

```html
<article class="entry">
  <h3><a href="writing/your-post.html">你的文章标题</a></h3>
  <time datetime="YYYY-MM-DD">YYYY.MM.DD</time>
  <p>简短摘要。</p>
</article>
```

3. 提交到 `main`。列表数量会自动更新，有内容时会隐藏对应空状态。

以上代码仅为编辑示例，不是已发布内容。

## 发布

保留现有 GitHub Pages 配置：`main` 分支、`/ (root)`。
`.nojekyll` 保持静态文件直接发布。

- 研究面：https://ycwsop.github.io/ichen.github.io/
- 个人面：https://ycwsop.github.io/ichen.github.io/#b
