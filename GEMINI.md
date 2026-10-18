# 官方教學網站維護與學生儀表板雙軌同步規範

## 1. 學生能力儀表板同步原則 (Mandatory Student Dashboard Sync)
- **展示學員名單**：
  - 柏文 (`bowen`)：國中教育會考 A++ 滿級分（全民英檢中級初試 172 分 / 複試雙合格）
  - 育穎 (`yuying`)：多益 550~600+ 扎根衝刺
  - 子恩 (`zien`)：雅思 Academic Band 7.0+ 跨學科精讀
  - Joseph (`joseph`)：高中英文學校段考 90+ 頂標
  *(注意：恩忻 `enxin` 依老師特別指示已自官方首頁展示名單移除，請勿擅自加回首頁)*
- **強制連動機制**：
  - **每次上述學生的課後白板分析、學習數據或能力儀表板更新時，必須同步更新本網站 `index.html` 中的 `studentData` 資料模型！**
  - 同步欄位包含：階段目標與進度、最新實力落點、白板筆跡數量與回數、作業掌握度百分比、六維雷達多邊形座標 (`polygon`)、弱點與掌握標籤 (`tags`)、以及最新家長課後回饋 (`parentMsg`)。
  - 更新後立即執行 Git 提交與推送 (`git add index.html; git commit -m "..."; git push origin main`)，確保 GitHub Pages 線上版永遠呈現最新數據。

## 2. 聯絡與隱私防護原則
- **官方諮詢 Email**：`wandymellow2@gmail.com`（全站表單直連 FormSubmit AJAX 後端）。
- **官方 LINE ID**：`TingZheng2`（提供一鍵複製與直接開啟好友連結）。
- **個人電話隱私**：嚴禁在網站任何地方顯示手機或電話號碼。
