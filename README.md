# 一號隊友：統一獅球迷網站

此專案是以球迷視角製作的統一獅非官方網站，使用原生 HTML、CSS、JavaScript 與 JSON，沒有前端框架或建置程序。頁面與素材目前以相對路徑互相連結；整理時應先維持既有網址與資料夾位置，避免搬檔後連結失效。

## 專案地圖

- 根目錄 HTML：首頁 `index.html`、賽程月曆 `calendar.html`、球隊歷史 `history.html`、球員名單 `roster.html`、主場攻略 `stadium.html`、接駁資訊 `shuttle.html`、球場美食 `guide.html`、應援專區 `cheer.html`、網站故事 `story.html`、資料來源 `credits.html` 等。
- `player/`：球員個人介紹；`player/pitcher/`：投手個人介紹。
- `cheerlions/`：Uni-Girls 與應援人物的個人頁。
- `news/`：新聞內頁與週報資料。
- `images/`：全站圖片；其下再依球員、應援、歷史、月曆等用途分類。
- `style.css`：多數頁面共用的全站樣式與各頁專用樣式。
- `.vscode/`：VS Code 專案設定。

## 首頁資料流

- `schedule.json`：首頁比賽卡片讀取的賽程資料。
- `standings.json`：首頁戰績表資料；JavaScript 依勝敗場計算勝率與勝差。
- `home_focus.json`：球員異動、週報摘要和 YouTube 影片資料。
- `images/calendar/`：月曆頁與首頁展示的賽程圖片。

這些資料目前是專案內的靜態檔案，不會自動從 CPBL 更新。修改賽程、戰績或球員資訊時，應以 CPBL 或球團最新公告核對後再更新。

## 球員頁頁尾

球員個人頁使用與首頁相同的 `main-footer` 內容。因球員頁分在不同深度的資料夾，圖片與站內連結會使用相對應的 `../` 或 `../../` 路徑；新增球員頁時請沿用該頁所在資料夾的相對路徑深度。
