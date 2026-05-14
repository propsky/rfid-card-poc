# 儲值卡雲端備份 POC

擎天有限公司 × 翔飛達｜2026 TAGE 展後洽談

---

## 📄 文件

👉 **[完整規格書](https://propsky.github.io/rfid-card-poc/)** — 資料結構、API 端點、前端模組說明、工作拆解

👉 **[UI 線框稿](https://propsky.github.io/rfid-card-poc/ui-wireframe.html)** — 六個頁面的版面與元件配置，工程師實作依據

---

## ✅ 任務追蹤方式（給工程師看）

本專案使用 **GitHub Issues** 追蹤開發進度。

### 怎麼找到 Issues？

1. 打開這個 repo 頁面（就是你現在看到的這個頁面）
2. 點上方的 **Issues** 標籤頁
3. 你會看到兩個 Issue：**Milestone 1** 和 **Milestone 2**

### 怎麼打勾？

1. 點進 Issue
2. 在任務清單裡，直接點 `[ ]` 方框就會變成 `[x]`（打勾）
3. **不需要留言、不需要 commit**，直接點就好
4. Sam 可以隨時進來看你的進度

### 注意事項

- Milestone 1（前端）和 Milestone 2（後端）是兩個獨立的 Issue
- 請按照 Issue 裡的順序完成任務
- 有問題直接在 Issue 下方留言，Sam 會收到通知

---

## 🗂 專案結構（開發時參考）

```
poc/
├── frontend/          ← Milestone 1：React + Vite 前端
│   ├── src/
│   │   ├── mock/      ← mock/db.js、mock/api.js（先在這裡作業）
│   │   ├── pages/
│   │   └── components/
│   └── package.json
│
└── backend/           ← Milestone 2：Python + FastAPI 後端
    ├── main.py
    ├── database.py
    ├── routers/
    └── requirements.txt
```

---

## 🚀 啟動方式

### Milestone 1（前端只）
```bash
cd frontend
npm install
npm run dev
# 開啟 http://localhost:5173
```

### Milestone 2（前後端）
```bash
# Terminal 1：後端
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
# 後端跑在 http://localhost:8000
# API 文件在 http://localhost:8000/docs

# Terminal 2：前端
cd frontend
npm run dev
```

---

*擎天有限公司內部文件 · Draft v1.0 · 2026-05*
