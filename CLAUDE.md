# 紀錄時數 手機 App（h14-hours-app）

## 目的
把 Google Drive「紀錄時數」資料夾裡 5 張結構相同的 Google Forms（內部／視覺〔原光園，2026-09-21 更名〕／遊戲開發／專家／燈光）
合成一個手機用的單頁 PWA：記住姓名、時段用時間選擇器、時數自動算、金額手填、離線先存再送。
送出仍寫回原本 5 張表單的回應試算表（走 formResponse），下游（勞務費用總表 seed 列、排班↔工時對帳 bot）完全不動。

## 範圍鐵則
- 純靜態：index.html + manifest.webmanifest + sw.js + 圖示，無後端、無金鑰。
- 不新增任何 Google 端資源；表單結構若改（entry ID 變動），只改 index.html 的 FORMS / ENTRY 兩個常數。

## 退場條件
表單改用 AppSheet 或其他系統時：關 GitHub Pages、repo 封存。

## 產出歸屬
- 正式網址：GitHub Pages（Hsiao-Tzu/h14-hours-app）。
- 表單來源資料夾：https://drive.google.com/drive/folders/16Kyia4Odht2PBPb-3vaw7IY5OjlLsvzc
