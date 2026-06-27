# 李珮暄 Shirley Li — AI 醫療教育作品集

一頁式作品集網站，展示獨立設計、開發並上線的醫療教育 AI 平台。
純靜態網站（單一 `index.html`，無後端、無建置步驟）。

## 檔案

| 檔案 | 用途 |
|------|------|
| `index.html` | 網站本體（含所有樣式與內容，單檔即可運作） |
| `render.yaml` | Render 一鍵部署設定（Blueprint） |
| `netlify.toml` | 改用 Netlify 部署時的設定（擇一即可） |

---

## 部署方式（擇一）

### 方式 A：Render Static Site（推薦，永久免費）

**A‑1　用 Blueprint（最省事，已附 `render.yaml`）**
1. 把這個資料夾推上一個 GitHub repo（`index.html` 與 `render.yaml` 放在根目錄）。
2. Render Dashboard → **New + → Blueprint** → 連接該 repo。
3. 確認變更內容無誤 → **Deploy Blueprint**。
4. 完成後會得到一個 `xxx.onrender.com` 網址。

**A‑2　不想用 yaml，手動建立也可以**
1. 把 `index.html` 推上 GitHub repo。
2. Render Dashboard → **New + → Static Site** → 連接 repo。
3. **Build Command** 留空；**Publish Directory** 填 `.`（根目錄）。
4. **Create Static Site** → 取得網址。

> Render 靜態網站永久免費，含全球 CDN、自動 HTTPS，可綁自訂網域，且不需要信用卡。

### 方式 B：Netlify Drop（最快，不需 GitHub）
1. 打開 https://app.netlify.com/drop
2. 把 `index.html`（或整個資料夾）直接拖進去。
3. 幾秒後即得到公開網址。

> 為什麼不用 Streamlit：Streamlit 是用來跑 Python 應用的，無法直接放純 HTML 網頁，並會附帶它自己的工具列，不適合靜態作品集。

---

## 更新內容

所有文字與連結都在 `index.html` 裡：
- 作品卡片：搜尋 `class="work"`，每張卡的 `href` 是平台網址，中文標題在 `work__zh`、英文在 `work__en`。
- 若用 Render（Git 部署）：改完 push 到 GitHub，Render 會自動重新部署。
- 若用 Netlify Drop：改完重新拖一次檔案即可。

## 上線後

把網址貼到：
- LinkedIn 個人檔案的 **Featured（精選）** 區（連結可點、會有預覽縮圖）。
- 履歷的作品集／聯絡資訊處。

## 小提醒

- 字型透過 Google Fonts 線上載入，需在連網瀏覽器開啟才會顯示完整字體（離線會以系統字替代，版面不受影響）。
- 部署前先自己點過每個平台連結，確認都能開啟。
