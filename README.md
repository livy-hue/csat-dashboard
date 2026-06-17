# LINE GO FAQ 維護儀表板

每月從 Zendesk 匯出 ZIP 報告後上傳即可自動更新。

## 使用方式

### 上傳更新資料
1. 在 Zendesk Explore → 知識庫報告，匯出以下五份報告的 ZIP：
   - Knowledge Base（知識庫概覽）
   - Search（搜尋分析）
   - Quick Answers（快捷回答）
   - Self-service（自助服務）
   - Knowledge Capture（知識捕獲）
2. 點擊儀表板右上角「上傳 ZIP」
3. 一次選擇所有 ZIP 檔案（4～5 個），系統自動合併解析

### 篩選功能
- **時間範圍**：最近 30 / 60 / 90 / 180 天
- **服務類別**：TAXI、機場接送、租車、代駕⋯等
- **問題類型**：搜尋無結果 / 有結果但沒點 / 停留時間過短 / 需新增文章

### 儀表板說明
| 指標 | 說明 |
|------|------|
| 搜尋無結果 | 客人搜尋但完全找不到文章，代表 FAQ 缺口 |
| 有結果但沒點 | 有文章但客人不點，代表標題待優化 |
| Quick Answer 觸發 | 搜尋後直接看到答案，自助成功 |
| 自助解決率 | Quick Answer / 總搜尋，目標 70% |

## 部署到 GitHub Pages

1. 建立新的 GitHub 儲存庫
2. 上傳 `index.html` 和 `data.json`
3. Settings → Pages → Source 選 main branch
4. 幾分鐘後即可透過網址存取

每次更新資料：直接替換 `data.json` 即可（或使用儀表板內的上傳功能）
