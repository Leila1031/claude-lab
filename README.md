# Leila Interior Studio｜室內設計作品集 Landing Page

Leila 室內設計工作室的單頁式形象網站（Landing Page），介紹設計理念、精選作品，並提供合作洽詢入口。

## 網站功能

- **導覽列（Sticky Nav）**：固定於頁面頂端、帶毛玻璃效果，可快速跳至「作品」與「合作洽詢」區塊。
- **Hero 主視覺**：品牌標語、檔期預約資訊、行動按鈕與工作室數據統計。
- **精選作品**：以卡片呈現代表作品（靜光之宅、日常咖啡 Daily Brew、舊巷新生）。
- **合作洽詢**：「與我聯繫」按鈕可直接開啟 Email 撰寫視窗。
- **頁尾**：版權資訊（年份自動更新）與快速連結。
- **動態效果**：進場淡入動畫，以及捲動到區塊時的漸現效果（支援 `prefers-reduced-motion`，會為偏好減少動態的使用者關閉動畫）。
- **RWD 響應式設計**：
  - 寬度 ≤ 900px：作品卡片改為單欄、隱藏導覽連結。
  - 寬度 ≤ 560px（手機）：標題字級縮小為桌面版 75%、按鈕滿版排列，所有可點擊元素維持至少 44px 觸控高度。

## 使用技術

- **HTML5**：語意化標籤（`header`、`main`、`section`、`footer`）。
- **CSS3**：CSS 變數（Custom Properties）、Flexbox、Grid、`clamp()` 流體字級、漸層背景、`backdrop-filter`、`@keyframes` 動畫、Media Queries。
- **Google Fonts**：Inter、Noto Sans TC。
- 少量原生 JavaScript：自動更新年份、以 `IntersectionObserver` 觸發捲動漸現動畫。

無需任何框架、套件或建置工具。

## 如何開啟

1. 下載或 clone 此專案：
   ```bash
   git clone https://github.com/Leila1031/claude-lab.git
   ```
2. 進入專案資料夾，直接用瀏覽器開啟 `index.html`：
   - **Windows**：在檔案總管中雙擊 `index.html`，或於終端機執行 `start index.html`
   - **macOS**：執行 `open index.html`
   - **Linux**：執行 `xdg-open index.html`
   - 也可以將 `index.html` 直接拖曳到瀏覽器視窗中。
3. 想檢視手機版效果：按 `F12` 開啟開發者工具，切換「裝置模擬（Device Toolbar）」選擇手機尺寸即可。

> 字型由 Google Fonts 載入，離線時會自動改用系統字型，版面不受影響。

## 專案結構

```
claude-lab/
├── index.html   # 網站主頁（含 HTML 與 CSS）
└── README.md    # 專案說明
```
