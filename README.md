# Flask Recipe Sharing App

這是一個使用 Flask 與 SQLite 建立的簡易食譜分享網站，專門設計用於部署至 Render.com。

## 專案結構
- `app.py`: 後端主程式與資料庫設定
- `requirements.txt`: 依賴套件清單
- `render.yaml`: Render 部署設定檔
- `templates/`: 存放 HTML 模板 (base.html, index.html, create.html)

## 部署至 Render.com
1. 將此資料夾內的檔案全部上傳至你的 GitHub Repository。
2. 登入 [Render.com](https://render.com/) 並點擊 **New+** -> **Web Service**。
3. 連結你的 GitHub Repository。
4. 設定:
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `gunicorn app:app`
5. 點擊 **Create Web Service** 即可完成部署！
