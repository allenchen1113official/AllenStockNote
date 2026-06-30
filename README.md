# Allen Stock Note · 技術分析複習

和同學一起複習用的靜態網站，包含：

- **翻卡複習**（`review-cards.html`）：18 張問答卡，可翻面自測、標記熟悉度、搜尋篩選。
- **康乃爾筆記**（`cornell-notes.html`）：三頁精華彙整，可列印成 A4。
- **首頁**（`index.html`）：整合入口。

## 檔案

```
index.html          ← 首頁（GitHub Pages 會自動以此為入口）
review-cards.html   ← 翻卡複習
cornell-notes.html  ← 康乃爾筆記
README.md
```

## 部署到 GitHub Pages

### 方法 A — 網頁上傳（最簡單，免指令）

1. 進入 repo：<https://github.com/allenchen1113official/AllenStockNote>
2. 點 **Add file → Upload files**，把 `index.html`、`review-cards.html`、`cornell-notes.html`、`README.md` 一起拖進去，按 **Commit changes**。
3. 點上方 **Settings → Pages**。
4. **Source** 選 **Deploy from a branch**，Branch 選 **main**、資料夾選 **/ (root)**，按 **Save**。
5. 等約 1 分鐘，網站會在：
   **https://allenchen1113official.github.io/AllenStockNote/**

把這個網址傳給同學即可。

### 方法 B — 用 Git 指令（在你的 Mac 上）

```bash
git clone https://github.com/allenchen1113official/AllenStockNote.git
cd AllenStockNote
# 把上面四個檔案複製進這個資料夾，然後：
git add .
git commit -m "Add technical analysis review site"
git push origin main
```

推送後，一樣到 **Settings → Pages** 啟用（main / root）。

## 更新內容

- 要改卡片：編輯 `review-cards.html` 最上方標示「只需要編輯這個區塊」的 `CARDS`。
- 改完重新 commit / 上傳即可，網站會自動更新。
