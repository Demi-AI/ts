GitHub Pages: https://chun-lin-huang.github.io/ts/

**網站設計理念：**  
我們自己在打工的公司有打卡系統，但這個系統主要只能進行上下班打卡，並沒有其他功能。當主管上傳班表時，我們需要額外打開行事曆來記錄上班日期，劃假時也需聯絡主管，這樣不僅浪費時間，還降低了系統的實用性。

**設計原則：**  
1. 簡約、直觀的設計，通過導航欄快速切換到其他頁面使用方式。
2. 集中展示所有與工作相關的功能（如上班日期、請假日期、代辦事項等），提高員工的使用便利性和效率。

**技術選用：**  
1. **JavaScript:**  
   - 功能: 實現網站的互動和動態內容。用於處理前端邏輯，如：
     - 打卡系統：根據用戶操作，記錄上班和下班時間，並自動計算當日工時和累積總工時。
     - 劃假系統：用戶在日曆中選擇請假日期並記錄。
     - 任務管理：顯示待辦事項並更新狀態，幫助員工組織每日工作。
   - JavaScript 還負責與伺服器端交互，通過 AJAX 請求進行數據傳輸和更新。

2. **CSS:**  
   - 功能: 控制網站樣式和排版，提升用戶體驗，設計簡約直觀的界面，使頁面不僅功能完善，還具美觀外觀。
     - 實現響應式設計，支持不同設備（桌面、平板、手機）提供優質的使用體驗。
     - 添加動態效果（如按鈕 hover 效果）和色彩搭配，使界面更加吸引人。

3. **HTML:**  
   - 功能: 網站的結構標記語言，負責頁面元素的排列和顯示方式。
     - 設置頁面結構，如表單、表格、按鈕等元素來收集用戶信息（打卡時間、請假日期、任務狀態）。
     - 創建頁面容器，設置導航條及頁面跳轉功能（如打卡頁、請假行事曆頁）。
     - 結合其他技術（JavaScript 和 CSS）增強互動性和可視化效果。

4. **React:**  
   - 功能: 用於構建用戶界面的 JavaScript 库，特別適合單頁應用（SPA）。
     - 組件化開發：將頁面拆分成不同組件（打卡記錄、請假日曆、任務列表等），提高代碼的可維護性和可重用性。
     - 動態更新：React 動態更新頁面，無需刷新整個頁面。
     - 狀態管理：通過 `useState` 和 `useEffect` 等 Hooks 管理應用狀態，如記錄打卡時間、管理待辦事項。

總結來說，這些技術的結合能夠高效實現動態交互、清晰頁面結構和美觀設計，使打卡、劃假、任務管理和財務功能順暢運行，為員工提供集中的工作平台。

**規劃：**  
此網站共分為六個頁面，除了首頁以外，以下為其餘五個頁面：

1. **財務管理系統頁面:**  
   員工可以輸入當月的收入、支出和薪資，系統將自動計算當月獎金、勞保費、健保費以及淨收入，並以長條圖呈現。

2. **行事曆任務管理系統頁面:**  
   員工可以在行事曆中註記上班日期，並能新增代辦事項，查看和更新代辦事項完成狀態。

3. **打卡系統頁面:**  
   員工可記錄上下班時間，系統會自動計算當日工時及累積總工時，並顯示打卡記錄。

4. **劃假行事曆系統頁面:**  
   員工可在行事曆中選擇請假日期，公司可以檢視完整的請假行事曆，員工也能查看已選擇的請假日期。

5. **反饋問題系統頁面:**  
   員工遇到問題或有建議時，可以透過表單進行反饋，讓公司了解問題內容及員工需求。