# 決戰台北：第一人稱選戰模擬 (Showdown Taipei 2026)

> 2026 台北市長第一人稱選戰模擬遊戲。體驗站在講台後面面對全場記者閃光燈與尖銳追問的壓迫感！

## 🌟 M1 版本亮點 (記者會垂直切片)
- **第一人稱視角 (POV)**：講台手部視差、呼吸晃動、閃光燈爆破白光、心跳倒數震顫。
- **動態追問與翻舊帳**：衝動許下的政見承諾會被記者當場反咬，即時考驗應變能力。
- **原創吉祥物記者團**：狐狸、柴犬、三花貓、貓頭鷹記者各懷不同立場與性格。
- **純程式聲光引擎**：純 HTML5/Web Audio API，整站體積小於 60KB，免載入 MP3，手機順暢 60FPS。
- **無障礙支援**：一鍵開啟「減少動態 (Reduce Motion)」、字體放大、全域靜音。
- **靈活 AI 接口**：內建離線智慧評判；亦提供自備金鑰（BYOK）的 LLM 連線能力，保障隱私與資安。

---

## 🚀 部署到 GitHub Pages (3 分鐘上手)

本專案為純靜態無伺服器架構，支援任何 GitHub 帳號與儲存庫名稱。

### 方式 A：直接上傳（最簡單）
1. 在 GitHub 上建立一個新的公開儲存庫（例如 `taipei-campaign-2026`）。
2. 將本專案的 `index.html` 直接上傳至該儲存庫根目錄。
3. 進入儲存庫的 **Settings** -> **Pages**。
4. 在 **Build and deployment** > **Branch** 選擇 `main`，資料夾選擇 `/ (root)`，點擊 **Save**。
5. 稍等約 1 分鐘，即可透過 `https://<您的帳號>.github.io/<您的repo名稱>/` 開啟遊玩！

### 方式 B：透過 GitHub Actions 自動部署
本專案包含 `.github/workflows/deploy.yml`。只要將完整資料夾推送到 GitHub，工作流將自動完成 Pages 部署。

---

## 💻 本機開發與執行
因為是純靜態架構，本機遊玩無需安裝任何 Node.js 套件：
1. 下載或複製專案檔案。
2. 直接雙擊 `index.html` 在任何現代瀏覽器（Chrome, Safari, Edge, Firefox）中開啟即可。
3. 若需測試音效與完整功能，建議搭配 VSCode Live Server 或 Python 簡易伺服器：
   ```bash
   python3 -m http.server 8080
   # 開啟 http://localhost:8080 體驗最佳效能
