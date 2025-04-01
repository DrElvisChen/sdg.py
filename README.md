# 國立臺中科技大學 SDGs 課程統計儀表板 (NUTN SDG Course Statistics Dashboard)

這是一個使用 Streamlit 開發的互動式儀表板，用於視覺化分析國立臺中科技大學 (NUTN) 的課程與聯合國永續發展目標 (SDGs) 的關聯性。使用者可以上傳包含課程資料的 Excel 文件，儀表板會自動處理數據並生成多種圖表與統計數據。

This is an interactive dashboard developed using Streamlit to visualize and analyze the relationship between courses at the National Taichung University of Science and Technology (NUTN) and the United Nations Sustainable Development Goals (SDGs). Users can upload an Excel file containing course data, and the dashboard automatically processes the data to generate various charts and statistics.

## ✨ 功能 (Features)

* **⬆️ Excel 文件上傳 (Excel File Upload):** 支援 `.xlsx` 和 `.xls` 格式的課程資料文件上傳。
* **📊 主要指標 (Key Metrics):** 顯示總課程數、SDG 相關課程數及佔比。
* **📅 動態標題 (Dynamic Title):** 儀表板標題會根據資料中的學年度自動更新。
* **🎨 自訂樣式 (Custom Styling):** 包含自訂 CSS，提供更美觀的卡片和標籤頁樣式。
* **📑 互動式分頁 (Interactive Tabs):**
    * **SDG 分佈圖 (SDG Distribution):** 以水平長條圖顯示各個 SDG 目標被課程涵蓋的次數。
    * **科系 SDG 分佈表 (Department SDG Table):** 以表格熱圖呈現各科系與 SDG 目標的關聯程度，可篩選顯示前 N 個科系，並可點擊欄位排序。
    * **SDG 課程統計 (SDG Course Statistics):** 提供各 SDG 的詳細統計表、課程數量長條圖、佔比圓餅圖，以及分析單一課程涵蓋多個 SDG 的分佈直方圖。
    * **課程資料探索 (Course Data Exploration):**
        * 提供依「科系」、「SDG」、「開課年度」篩選課程的功能。
        * 允許使用者自選要顯示的資料欄位。
        * 顯示篩選後的課程資料表格。
        * 提供篩選後資料的 CSV 下載功能。
        * 顯示篩選後資料的 SDG 分佈長條圖與圓餅圖。
* **📄 範例資料 (Sample Data):** 若未上傳文件，會顯示操作說明、範例資料表格，並提供範例 CSV 文件下載。
* **⚠️ 錯誤處理 (Error Handling):** 包含文件讀取錯誤、必要欄位 ('final SDGs') 缺失等錯誤處理機制。

## ⚙️ 需求 (Requirements)

* Python 3.7+
* Streamlit
* Pandas
* Numpy
* Plotly
* openpyxl (用於讀取 `.xlsx` 文件)

你可以使用 pip 安裝所需的套件：
```bash
pip install streamlit pandas numpy plotly openpyxl
