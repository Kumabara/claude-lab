# Kuma Studio 熊 — 平面設計作品集 Landing Page

自由接案平面設計師「熊」的個人作品集單頁網站（Landing Page），以「深海」色階為視覺主題，展示品牌識別、包裝與編排設計作品。

## 網站功能

- **導覽列**：固定於頂端（sticky）的毛玻璃導覽列，可快速跳到「作品」與「合作」區塊，並支援平滑捲動。
- **英雄區塊（Hero）**：主標語、自我介紹、接案檔期狀態，以及「與我聯繫」、「觀看作品」兩個行動按鈕，搭配淡入動畫。
- **精選作品**：以卡片呈現作品案例（潮間帶 Tidal Coffee、山湯 Onsen 沐浴系列、深藍以下 獨立誌）。
- **合作聯繫**：以 `mailto:` 連結直接寄信洽詢合作。
- **頁尾**：版權資訊（年份自動更新）與社群連結（Behance、Instagram、Dribbble）。
- **視覺效果**：深海漸層背景、擺動的光束動畫、顆粒質感，以及捲動時區塊淡入（Intersection Observer）。
- **RWD 響應式設計**：針對平板（≤ 960px）與手機（≤ 640px）調整版面與字級，按鈕維持至少 44px 觸控尺寸，並避免手機出現水平捲軸。
- **無障礙**：支援 `prefers-reduced-motion`，偏好減少動態的使用者會關閉動畫；連結與圖示附有 `aria-label`。

## 使用技術

- **HTML5**：語意化標籤（`header`、`main`、`section`、`footer`）。
- **CSS3**：CSS 變數（自訂屬性）、Grid / Flexbox 排版、漸層與 `backdrop-filter` 毛玻璃效果、`@keyframes` 動畫、Media Queries。
- **Google Fonts**：Inter 與 Noto Sans TC。
- 少量原生 JavaScript：自動更新年份與捲動淡入效果（不使用任何框架或建置工具）。

## 如何用瀏覽器開啟

整個網站只有一個 `index.html` 檔案，不需要安裝任何套件或伺服器。

**方法一：直接開啟**

1. 在 Finder（或檔案總管）中找到專案資料夾 `claude-lab`。
2. 對 `index.html` 按兩下，或按右鍵 →「打開檔案的應用程式」→ 選擇 Chrome、Safari 等瀏覽器。

**方法二：使用終端機（macOS）**

```bash
cd claude-lab
open index.html
```

**方法三：本機伺服器（選用）**

```bash
cd claude-lab
python3 -m http.server 8000
```

接著在瀏覽器開啟 <http://localhost:8000>。

> 提示：想查看手機版效果，可在 Chrome 按 `Cmd + Option + I` 開啟開發者工具，再點選「切換裝置工具列」（`Cmd + Shift + M`）。

## 專案結構

```
claude-lab/
├── index.html   # 網站主頁（HTML + CSS + JS 全部內含）
├── note.txt     # 筆記
└── README.md    # 專案說明
```
