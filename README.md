# flyingman

科技飞侠 PC 引流站 —— 纯展示性落地页，为微信小程序引流。

- 托管：GitHub Pages（`https://wxzhongwang.github.io/flyingman/`）
- 技术：单文件静态站（`index.html`，内联 CSS/JS），无构建步骤
- 数据：页面加载后调用平台公开接口拉取全站热门资料
  `GET https://flyingman.mypetstore.cn/api/miniprogram/products/hot?limit=8`
  接口不可用时保留 HTML 内静态兜底卡片（同时也是 SEO 可抓取内容）
- SEO：meta description/keywords、Open Graph、Twitter Card、JSON-LD（WebSite/WebPage）、语义化标签
- 物料：`gh_397ccaeab142_*.jpg` 为官方小程序码（258/344/430/860/1280 五尺寸）

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```

直接双击 `index.html` 也能看，但接口数据需联网（跨域已放行）。

## 维护

改 `index.html` → commit → push，Pages 自动重建。
主仓 `prototype/ui-refresh/pc.html` 为原型稿，正式维护在本仓。
