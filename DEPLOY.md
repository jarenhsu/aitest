# 🚀 GitHub Pages 部署指南

## 問題排查

如果網頁崩潰或題目不顯示，請按以下步驟檢查：

### 1️⃣ 確認所有檔案已上傳

你需要將以下 5 個檔案上傳到 GitHub 的 `aitest` 倉庫：

```
📁 aitest/
├─ index.html                (必需) ✅
├─ all_questions.json        (必需) ✅
├─ genai_100.json            (必需) ✅
├─ genai_200.json            (必需) ✅
└─ advanced_questions.json   (必需) ✅ 新增
```

**檔案大小參考：**
- index.html: ~33 KB
- all_questions.json: ~73 KB
- genai_100.json: ~35 KB
- genai_200.json: ~74 KB
- advanced_questions.json: ~119 KB (新增)

### 2️⃣ 上傳步驟

#### 方法 A：GitHub Web 界面（推薦最簡單）

1. 訪問 https://github.com/jarenhsu/aitest
2. 點擊「Add file」→「Upload files」
3. 選擇以下 5 個檔案一起上傳：
   - `index.html`
   - `all_questions.json`
   - `genai_100.json`
   - `genai_200.json`
   - `advanced_questions.json`
4. 點擊「Commit changes」

#### 方法 B：命令行（如果你熟悉 Git）

```bash
cd ~/path/to/aitest
cp /mnt/user-data/outputs/AI_Practice_System/* .
git add .
git commit -m "Add advanced 500-question database"
git push origin main
```

### 3️⃣ 驗證部署

上傳後，訪問 https://jarenhsu.github.io/aitest/

**檢查清單：**
- [ ] 頁面正常載入
- [ ] 4 個頁籤都顯示（🐕 工程素養、🐕 生成式 AI 100、🐕 生成式 AI 200、🦴 進階題庫）
- [ ] 每個頁籤都能點擊切換
- [ ] 可以看到題目和選項
- [ ] 點擊「下一題」能正常翻頁

### 4️⃣ 常見問題

**問題：頁面顯示「無法加載 xxx.json」**
→ 檔案沒有上傳到 GitHub。檢查倉庫根目錄是否有所有 JSON 檔案。

**問題：只顯示 3 個頁籤，沒有「進階題庫」**
→ HTML 檔案沒有更新。確保上傳的是新的 `index.html`（32.9 KB）。

**問題：進階題庫頁籤點擊後崩潰**
→ `advanced_questions.json` 沒有上傳。確保檔案大小是 ~119 KB。

### 5️⃣ 所有檔案清單

最終應該在 GitHub 上看到：

```
https://github.com/jarenhsu/aitest/
├─ index.html (32.9 KB) ✅
├─ all_questions.json (73.2 KB) ✅
├─ genai_100.json (34.9 KB) ✅
├─ genai_200.json (74.4 KB) ✅
└─ advanced_questions.json (118.6 KB) ✅ 新增
```

---

## 快速修復

如果網頁當前崩潰，最快的修復方式：

1. **下載所有檔案** 從本地目錄
2. **訪問 GitHub 倉庫**
3. **點擊「Add file」→「Upload files」**
4. **一次性上傳所有 5 個檔案**
5. **等待 1-2 分鐘** GitHub Pages 自動更新
6. **訪問 https://jarenhsu.github.io/aitest/**

---

## 檔案驗證

已確認的檔案狀態：
- ✅ index.html: 包含 4 個頁籤（包括新的進階題庫）
- ✅ all_questions.json: 200 題（格式正確）
- ✅ genai_100.json: 100 題（格式正確）
- ✅ genai_200.json: 199 題（格式正確）
- ✅ advanced_questions.json: 500 題（格式正確）

所有檔案都已準備就緒，可立即上傳！
