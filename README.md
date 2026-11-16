# 材科筆記｜Materials Wiki

以繁體中文整理材料科學的入門知識庫，包含材料結構、相變與熱處理、機械性質。網站具有文章分類、即時搜尋、共用文章閱讀頁、深色模式與手機版排版。

## 專案目的
讓材料科學的術語與觀念更容易學習，並以 `AGENTS.md` 建立可供 AI 重複使用的開發規範，讓未來的文章可以快速新增而不破壞既有結構。

## 開啟方式
直接在瀏覽器開啟 `index.html`。不需要安裝套件、啟動本機伺服器或連接 API。

## GitHub Pages 部署
1. 在 GitHub 建立公開 repository，例如 `materials-wiki`。
2. 將解壓後的 `index.html`、`article.html`、`style.css`、`app.js`、`data.js`、`AGENTS.md`、`README.md` 全部上傳到 repository 根目錄（不可多包一層資料夾）。
3. 前往 Settings → Pages → Build and deployment，Source 選 `Deploy from a branch`，Branch 選 `main`、資料夾選 `/(root)`，按 Save。
4. 等待 GitHub 發布完成，取得 `https://你的帳號.github.io/materials-wiki/` 形式的網址。

## 檔案說明
- `index.html`：首頁
- `article.html`：文章共用閱讀頁
- `data.js`：所有文章內容，擴充時主要修改此檔
- `app.js`：互動與文章渲染
- `style.css`：網站樣式
- `AGENTS.md`：AI 開發與擴充規則

## 如何擴充
先閱讀 `AGENTS.md`，然後在 `data.js` 的 `window.ARTICLES` 新增一筆符合欄位格式的文章物件，首頁會自動增加卡片並納入搜尋功能，不必重寫 HTML。

## 作業說明
這是一個可持續擴充的小型學習網站；公開發布後，可將 repository 網址與 GitHub Pages 網址連同 `AGENTS.md` 內容一起提交。
