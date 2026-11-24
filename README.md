# 陳鈞甯 Narina Chen — 個人簡歷與作品集網站

本專案為個人簡歷單頁式網站（Single Page Portfolio），結合個人經歷、繪畫與視覺創作技能，以及高中時期跨領域專題作品，並完整實作 Git 分支管理、Pull Request 審查、版本回復（`git revert`）、A/B 測試與 GitHub Pages 自動化部署。

## 🌐 網站預覽與專案資訊
- **GitHub Pages 公開網址**：https://narina-042.github.io/portfolio/
- **GitHub 儲存庫連結**：https://github.com/Narina-042/portfolio
- **使用技術**：HTML5、CSS3（Grid / Flexbox / 響應式設計 `< 600px`）、Vanilla JavaScript（平滑捲動與懸浮按鈕互動）

## 🧪 A/B 版本實驗說明（技能展示區）
針對「繪畫與視覺創作技能」區塊，本專案分別建立兩個功能分支進行 A/B 設計實驗並各自發起 Pull Request：
- **版本 A（`feature/skills-bars` — 進度條版，PR #2）**：以量化百分比與橫向進度條呈現各項繪畫技能的熟練程度。
- **版本 B（`feature/skills-tags` — 標籤雲版，PR #3）**：以不同字級權重排列圓角標籤，並結合滑鼠懸停（hover）放大與變色互動效果呈現多元視覺創作能力。
- **採用與未採用原因**：最終採用**版本 B（標籤雲版）**合併至 `main` 主分支，並保留版本 A 的 PR 為未合併狀態作為對照紀錄。原因在於繪畫與視覺創作屬於質性與美感導向的跨領域能力，標籤雲設計能更靈活呈現多元技能面向且視覺版面較輕盈、富設計感；相對地，版本 A 的主觀百分比數字較難客觀衡量藝術創作程度，因此未採用。

## 🔄 版本回復（`git revert`）操作說明
我在這次作業中使用 `git revert` 回復某個 commit，原因是：在開發過程中曾嘗試將網站主色調變數（`--primary`）修改為高飽和亮螢光綠（commit `bf2c078`：`style: test neon green primary color`）進行視覺測試，但實際檢視後發現與整體暖色調美學不協調且降低文字閱讀對比度，因此使用 `git revert` 安全還原至原本的暖珊瑚橘配色，同時完整保留版本修改與回復的歷史紀錄。