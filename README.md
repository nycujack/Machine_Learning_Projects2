# Machine Learning & AI Projects Portfolio

本儲存庫收錄了三個核心的機器學習與人工智慧專案，涵蓋從傳統結構化資料的預測模型（員工離職預測、銀行定存轉換預測），到結合大型語言模型的 AI 應用（財務分析 AI Agent）。專案旨在展示端到端的數據分析、特徵工程、模型建構與 AI 系統開發能力。

## 核心專案介紹 (Projects)

### 1.財務分析 AI Agent (`財務分析AI_Agent.ipynb`)
**專案目標**：打造能自動解讀財務資訊、分析個股並輔助投資決策的智慧助理。
* **技術應用**：結合大型語言模型 (LLM) 與 RAG（檢索增強生成）技術，透過 Google Cloud AI Platform 等工具建構 AI 投資顧問，並使用 Gradio 建立互動介面。
* **亮點功能**：
  * **財報知識庫 (RAG)**：支援上傳財報 PDF 檔，透過 AI 自動檢索並精準回答特定財務問題（如營收成長率、毛利率等）。
  * **個股資訊速查**：串接即時股價與財務數據，快速進行個股摘要分析。
* **商業價值**：大幅縮短投資人或財務分析師閱讀長篇財報的時間，提供即時、精準的投資與營運洞察。

### 2.員工離職預測模型 (`員工離職預測專案.ipynb`) 
**專案目標**：透過歷史人事資料與工作行為數據，預測潛在的高風險離職員工，協助 HR 部門提前介入留才。
* **資料與特徵**：分析超過 1.4 萬筆訓練資料，涵蓋 47 項特徵（包含近一年請假數、出差集中度、年度績效等級、訓練時數、薪資職等與通勤成本等）。
* **技術應用**：
  * 數據預處理：缺失值處理 (Missing value imputation)、標籤編碼 (Label Encoding) 與獨熱編碼 (One-Hot Encoding)。
  * 建模演算法：使用決策樹 (Decision Tree) 與隨機森林 (Random Forest) 進行二元分類預測。
* **商業價值**：精準找出影響員工離職的關鍵痛點，以數據驅動人力資源管理，降低企業人才流失成本。

### 3.銀行定存轉換預測分析 (`DEPOSITE預測分析專案.ipynb`)
**專案目標**：針對銀行電話行銷活動，預測客戶申辦定期存款 (Deposit) 的意願，優化行銷資源分配。
* **資料與特徵**：分析 11,162 筆客戶資料，包含 17 個特徵（如年齡、職業、帳戶餘額、房貸狀態、前次行銷活動結果等）。
* **技術應用**：
  * 探索性資料分析 (EDA)：運用 Seaborn 與 Matplotlib 繪製箱型圖與長條圖，分析數據分佈與目標變數的平衡度。
  * 建模演算法：運用羅吉斯迴歸 (Logistic Regression) 等機器學習模型預測轉換率。
* **商業價值**：有效辨識高潛力客戶輪廓，協助業務團隊精準行銷，大幅提高行銷活動 (Campaign) 的轉換率並降低盲目撥打的成本。

## 技術棧 (Tech Stack)
* **程式語言**: Python
* **資料處理與視覺化**: Pandas, NumPy, Matplotlib, Seaborn
* **機器學習**: Scikit-learn (Random Forest, Decision Tree, Logistic Regression)
* **AI 與自然語言處理**: LLM, RAG (Retrieval-Augmented Generation), Google Cloud AI Platform
* **開發環境**: Jupyter Notebook / Google Colab

## 如何執行 (How to Run)
本儲存庫中的程式碼皆於 Google Colab 環境下開發與測試：
1. 將 `.ipynb` 檔案匯入 Google Colab 或本地端的 Jupyter 環境。
2. 確保掛載 Google Drive 或上傳相關的資料集（如 `bank.csv`, `train.csv`, `test.csv` 或 PDF 財報檔）。
3. 依照 Notebook 頂部的指示安裝必要的套件，即可依序執行區塊並重現分析結果。
