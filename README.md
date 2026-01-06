# sedvvvc9
由 EZPage 建立的網站 - Deployed by EZPage
# 🚀 2025 Vibe Coding 期末專案：[建立專屬於學校專用的問題追蹤平台]

## 🌟 1. 專題願景 (Vibe)
* **目標對象：本校大學生
* **設計風格：極簡風
* **核心功能：建立類公共政策平台，能直接與行政老師反映，以解決學生之問題。

## 🤖 2. Gemini 協作紀錄 (Prompt Log)
*請貼出你餵給 Gemini 最關鍵的一個 Prompt：*
>範例指令：「建立一個 學校專用的問題追蹤平台（School Issue Tracking System） ，不僅能提升校園行政效率，還能增進學生與校方的溝通透明度。

請幫助我構建這個系統，我將這份計畫分為四個階段：需求規劃、系統架構設計、資料庫設計以及程式碼實作範例。..」

*在開發過程中，你遇到了什麼 Bug？Gemini 怎麼幫你修好的？*
* **遇到的問題：**  針對處理歷程加入左右滾動頁面
* **Gemini 的建議：** 針對上方內容問題的失敗，以上方問題語言加強敘述，如;加入左右滾動按鈕： 在歷程區塊左右兩側加入了箭頭按鈕。
* 智慧顯示：平常隱藏，滑鼠移入該區塊時才會浮現，保持介面簡潔。 平滑滾動：點擊按鈕時，時間軸會平滑地左右移動。


## 📂 3. 檔案結構說明
* `index.html`(網頁主結構)：我們以關聯式資料庫 (如 MySQL 或 PostgreSQL) 為例，核心表格設計如下：

1. Users (使用者表)
id (PK)
username (學號/職工號)
email
role (student, teacher, admin)
2. Issues (問題表)
id (PK)
title (標題)
description (描述)
category (類別)
location (地點)
status (default: 'open')
priority (low, medium, high)
reporter_id (FK -> Users.id)
assigned_to (FK -> Users.id, nullable)
image_url (照片連結)
created_at (建立時間)
updated_at (更新時間)
3. Comments (留言/溝通紀錄表)
id (PK)
issue_id (FK -> Issues.id)
user_id (FK -> Users.id)
content (留言內容)
timestamp

## 📈 4. 自我心得與反思
* 使用 Vibe Coding (與 AI 對話寫 Code) 的心得：詢問它的時候，它會搞不清楚狀況，無法讓詢問問題回答延續。
* 如果可以再優化，我希望增加什麼功能？: 希望我的系統可以加強內部介面的美化功能。

---
**🔗 網頁預覽網址：** [https://github.com/pses103177/sedvvvc9/tree/main?tab=readme-ov-file、[https://pses103177.github.io/sedvvvc9/)]
