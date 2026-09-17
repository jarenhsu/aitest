# 🚀 10 單元系統部署指南

## 部署步驟

### 步驟 1：確認檔案

確保你的 `/aitest` 目錄中有以下檔案：

```
/aitest/
├── index.html                    ← 新的 10 單元網頁
├── advanced_questions.json       ← 1000 題題庫
├── 10UNITS_README.md            ← 使用說明
└── DEPLOY_10UNITS.md            ← 本檔案
```

### 步驟 2：本地測試（可選）

如果想在本地先測試：

```bash
# 進入目錄
cd path/to/aitest

# 啟動本地 Web 服務器
python3 -m http.server 8000

# 在瀏覽器開啟
# http://localhost:8000
```

### 步驟 3：上傳到 GitHub

```bash
# 進入你的本地倉庫
cd ~/jarenhsu.github.io/aitest

# 添加新檔案
git add index.html advanced_questions.json 10UNITS_README.md

# 提交
git commit -m "feat: 10 units structure with 1000 questions"

# 推送
git push origin main
```

### 步驟 4：確認部署

1. 等待 GitHub Actions 完成（通常 1-2 分鐘）
2. 訪問 https://jarenhsu.github.io/aitest/
3. 應該看到 **10 個單元標籤**

---

## ✅ 驗證清單

- [ ] `index.html` 已覆蓋舊版本
- [ ] `advanced_questions.json` 在正確位置
- [ ] GitHub 倉庫已推送
- [ ] 網頁已加載（查看 10 個標籤）
- [ ] 能夠點擊標籤切換單元
- [ ] 題目正確顯示
- [ ] 隨機和重置功能正常

---

## 🔧 若出現問題

### 問題 1：看不到 10 個單元

**原因**：瀏覽器快取
**解決**：按 `Ctrl+Shift+R`（Windows）或 `Cmd+Shift+R`（Mac）強制重新整理

### 問題 2：題目無法載入

**原因**：`advanced_questions.json` 路徑錯誤
**解決**：確認檔案在與 `index.html` 同目錄

### 問題 3：標籤頁無法切換

**原因**：JavaScript 執行錯誤
**解決**：
1. 按 `F12` 開啟開發者工具
2. 查看 Console 是否有錯誤訊息
3. 刷新頁面重試

### 問題 4：進度無法保存

**原因**：瀏覽器隱私模式或 localStorage 被禁
**解決**：使用正常瀏覽模式，檢查瀏覽器隱私設定

---

## 📊 新舊版本對比

| 功能 | 舊版（4 單元） | 新版（10 單元） |
|------|---------------|-----------------|
| 題庫數量 | 1099 題 | 1000 題 |
| 單元數量 | 4 個 | 10 個 |
| 難度分級 | 無明確分級 | 3 個難度級別 |
| 單元大小 | 250-300 題 | 40-200 題 |
| 學習路徑 | 單一線性 | 多種可選 |
| 移動版相應 | 有 | 優化加強 |

---

## 💡 推薦使用

### 新使用者
1. 從「單元 1：基礎概念」開始
2. 按順序完成前 4 個單元
3. 再進入深度學習部分

### 有基礎的學習者
1. 跳過單元 1-4
2. 直接從「單元 5：神經網路」開始
3. 重點準備單元 9-10

### 備考衝刺
1. 完成單元 1-4 的快速複習
2. 集中練習單元 6、7（視覺和語言）
3. 最後衝刺單元 9-10（應用和進階）

---

## 📞 支援

如有任何問題，請查閱：
- `10UNITS_README.md` - 完整使用說明
- `advanced_questions.json` - 題庫結構

祝備考順利！🐕
