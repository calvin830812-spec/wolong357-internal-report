# 臥龍357內部檢討報告｜GitHub Pages MVP

本資料夾為臥龍357不續行案內部檢討 HTML 報告的 GitHub Pages 最小可行發布版本。

## 內容

| 路徑 | 用途 |
|---|---|
| `index.html` | GitHub Pages 首頁，內含臥龍357完整檢討報告與圖表 |
| `assets/visuals/` | 報告內嵌用 SVG 圖表素材 |
| `DEPLOY.md` | GitHub Pages 發布操作步驟 |

## 使用限制

- 本報告為內部管理檢討資料，不對外使用。
- 不使用外部 CDN。
- 不使用外部圖片資源。
- 圖表以相對路徑引用 `assets/visuals/`。
- 若要修改報告內容，應回到原始 V9 報告與 HTML 來源檔確認後再更新。

## 本地預覽

可直接用瀏覽器開啟：

```bash
open index.html
```

或使用本機靜態伺服器：

```bash
python3 -m http.server 8000
```

再開啟：

```text
http://localhost:8000
```
