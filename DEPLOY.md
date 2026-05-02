# GitHub Pages 發布步驟

GitHub repo：

```text
https://github.com/calvin830812-spec/wolong357-internal-report
```

## 一、初始化與推送

在 `github-pages-mvp/` 資料夾內執行：

```bash
cd github-pages-mvp
git init
git branch -M main
git add index.html assets README.md DEPLOY.md
git commit -m "Add Wolong357 internal report GitHub Pages MVP"
git remote add origin https://github.com/calvin830812-spec/wolong357-internal-report.git
git push -u origin main
```

若 repo 已經有內容，請先確認遠端狀態後再推送，避免覆蓋既有資料。

## 二、GitHub Pages 設定

1. 進入 GitHub repo：`wolong357-internal-report`
2. 點選 `Settings`
3. 左側選單點選 `Pages`
4. `Build and deployment` 選擇 `Deploy from a branch`
5. Branch 選擇 `main`
6. Folder 選擇 `/ (root)`
7. 點選 `Save`

## 三、發布後檢查

發布完成後，檢查以下項目：

| 檢查項目 | 標準 |
|---|---|
| 首頁是否開啟 | 能看到臥龍357完整 HTML 報告 |
| 圖表是否顯示 | 5 張 SVG 圖表皆可正常載入 |
| 樣式是否正常 | 寶舖藍綠色系與表格樣式正常 |
| 列印是否正常 | 瀏覽器列印預覽可輸出 PDF |
| 外部資源 | 不應出現外部 CDN 或外部圖片載入 |

## 四、更新方式

若後續更新 `index.html` 或 `assets/visuals/`：

```bash
cd github-pages-mvp
git status
git add index.html assets/visuals README.md DEPLOY.md
git commit -m "Update Wolong357 report"
git push
```
