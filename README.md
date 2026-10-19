# 邓琰 · 视觉传达设计作品集

网站地址：https://zzzbkkk.github.io/deng-yan-portfolio/

中文个人作品网站，包含首页、作品分类、项目图集、个人介绍与联系方式。当前版本为 V0.5：作品页采用编辑式画廊、真实素材组合封面、桌面主次网格与手机单列，保留全部12件作品。首页默认展示《无象之境》，AIGC 分类包含3件作品。

## 文件与维护

- `dist/`：完整静态网站；HTML、CSS、JavaScript、图片及本地字体。
- `dist/content.js`：作品文字、分类标签、图片索引及联系方式。
- `dist/app.js`：导航、作品筛选、海报切换与大图查看。
- `dist/works.css`：作品画廊的独立样式；不影响首页和详情页。
- `.github/workflows/pages.yml`：推送到 `main` 后部署 `dist/` 至 GitHub Pages，也支持手动运行。

无需安装依赖或构建。可以直接打开 `dist/index.html`；本地 HTTP 预览可运行：

```sh
python -m http.server 4175 --directory dist
```

修改后提交并推送 `main`，等待 GitHub Actions 中的部署任务完成。修改脚本或样式时，同步更新 HTML 中对应资源的版本参数，便于刷新缓存。

客户原始 PPT、素材索引和内部工作记录不属于发布内容。作品图像用于本作品集展示，未另行授予复制或商用许可。本地 Anton 字体的许可见 `dist/assets/fonts/Anton-OFL.txt`。
