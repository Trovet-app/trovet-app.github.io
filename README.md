# Trovet 珍物 — 官方網站

Trovet(珍物)的官方介紹網站,部署於 GitHub Pages,自訂網域 [https://trovet.app](https://trovet.app)。

## 內容

- 單頁 landing page,介紹 app 功能、隱私承諾與 Plus 規劃
- 中英雙語切換(zh-Hant / en),預設依瀏覽器語系
- 純 HTML + CSS + JS,**無 framework 依賴、無 build step**
- 包含實際 app 截圖(Galaxy S24 Ultra 1080×1920)

## 檔案結構

```
.
├── index.html       # 單頁網站本體
├── assets/          # app icon、wordmark、實際 app 截圖
├── CNAME            # GitHub Pages 自訂網域指向 trovet.app
├── .nojekyll        # 停用 GitHub Pages 的 Jekyll 處理(直接 serve 靜態檔)
├── robots.txt       # 允許爬蟲、指向 sitemap
├── sitemap.xml      # 單頁 sitemap(hreflang 雙語)
└── README.md        # 本檔
```

## 本機預覽

```bash
cd /path/to/this/repo
python3 -m http.server 8080
# 開瀏覽器到 http://localhost:8080
```

## 部署

Push 到 `main` branch 即由 GitHub Pages 自動部署。
DNS / Pages 設定請見 commit history 與 repo Settings → Pages。

## 授權

© 2026 Trovet. 本網站內容僅供 app 介紹用途。
