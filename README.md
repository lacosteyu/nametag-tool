# 姓名貼排版工具 (Name Sticker Generator)

網頁版姓名貼產生器，使用 HTML5 Canvas 即時預覽，支援列印輸出 (300 DPI)。

## 功能 Features

- **紙張大小**：A4 / A5 / 自訂 300x255 mm
- **輸出底色**：可選純色填充 / 透明背景
- **貼紙底色**：單張貼紙背景色 / 透明去背
- **多張背景圖**：可上傳多張背景圖，自動分配到不同列
- **自訂字體上傳**：支援 .ttf / .otf，透過 FileReader + FontFace API 載入後自動切換
- **Google Fonts 預載**：思源黑體、思源宋體、馬善政毛筆體、站酷快樂體
- **中英雙語**：中文姓名 + 英文姓名，獨立控制大小與垂直位置
- **尺寸彈性**：自訂貼紙寬高 (預設 3×1.3 cm)
- **裁切間距**：自訂控制左右 / 上下間距 (mm)
- **下載 PNG**：300 DPI 高品質列印圖檔

## 使用方式 Usage

直接在瀏覽器開啟 `index.html` 即可使用，無需安裝。

1. 選擇紙張大小
2. 設定底色 / 是否透明
3. 上傳背景圖（可選）
4. 上傳自訂字體 .ttf / .otf（可選，預設使用 Google Fonts）
5. 輸入中文 / 英文姓名
6. 調整字體大小與位置（滑桿即時預覽）
7. 點擊「下載列印圖檔」存 PNG

## 本地啟動 Local Development

```bash
# 直接開啟
open index.html

# 或用本地伺服器（建議，避免某些瀏覽器限制）
python3 -m http.server 8000
# 然後開 http://localhost:8000
```

## 部署 Deploy

GitHub Pages 已啟用：https://lacosteyu.github.io/nametag-tool

## 技術棧 Tech

- 純 HTML + CSS + Vanilla JavaScript
- HTML5 Canvas API（`drawImage`, `fillText`, `toDataURL`）
- 無後端、無外部依賴

## 授權 License

MIT