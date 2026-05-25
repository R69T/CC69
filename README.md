# cc69

cc69 是一個 Windows GUI 工具，主要用來透過圖形介面管理工作流程、登入狀態、任務發佈與執行狀態。  
本專案的主要入口版本是 **ChaCha69**，對應檔案為：

```text
gui_chacha69.py
```

---

## 主要版本：ChaCha69

`gui_chacha69.py` 是 cc69 的簡單版入口檔。  
它會設定程式版本名稱與工作通道數，然後啟動主 GUI 程式。

```python
YT_HELP_VERSION_CODE = "CHACHA69"
YT_HELP_VERSION_NAME = "ChaCha69"
YT_HELP_MAX_CHROME_WORKERS = "1"
```

簡單來說，這個版本適合一般單通道使用：

- 啟動名稱：`ChaCha69`
- 工作通道數：`1`
- 主要 GUI 由 `main.py` 提供
- 適合先測試、展示、或提供基本版下載

---

## 介面功能

cc69 的 GUI 主要包含：

- 語言切換
- URL 輸入欄
- 登入按鈕
- 開始工作 / 停止工作
- 發佈任務 / 停止發佈任務
- 狀態紀錄區
- 使用說明區
- 分數與每日使用狀態顯示

目前介面支援多語言：

- 中文
- English
- 日本語
- Deutsch
- Tiếng Việt

---

## 基本使用方式

1. 開啟程式。
2. 按下登入按鈕，完成登入。
3. 輸入網址。
4. 按下「開始工作」開始執行。
5. 如需停止，按下「停止工作」。
6. 如需停止發佈自己的任務，按下「停止發佈任務」。

> 注意：  
> 「停止工作」與「停止發佈任務」是兩個不同開關。  
> 停止發佈不代表停止目前正在執行的工作。

---

## 檔案說明

| 檔案 | 說明 |
|---|---|
| `gui_chacha69.py` | ChaCha69 簡單版入口，使用 1 個 Chrome 工作通道 |
| `main.py` | 主要 GUI、語言文字、工作流程與畫面邏輯 |
| `supabase_client.py` | 負責任務發佈、領取、完成回報與分數資料 |
| `gui_chacha69_pro.py` | Pro 版本入口，使用 3 個 Chrome 工作通道 |
| `gui_chacha69_sub.py` | Sub 版本入口，使用 5 個 Chrome 工作通道 |

---

## 其他版本補充

除了簡單版 `ChaCha69`，專案中也包含其他入口版本：

### ChaCha69 Pro

```text
gui_chacha69_pro.py
```

特點：

- 版本名稱：`ChaCha69Pro`
- 工作通道數：`3`
- 適合需要多通道執行的版本

---

### ChaCha69 Sub

```text
gui_chacha69_sub.py
```

特點：

- 版本名稱：`ChaCha69Sub`
- 工作通道數：`5`
- 適合更高通道數的版本

---

## 執行需求

本專案使用 Python GUI 與瀏覽器自動化相關套件，主要會用到：

- Python
- PyQt5
- Selenium
- Google Chrome
- Supabase 相關設定
- `config.py` 設定檔

> 注意：  
> 目前上傳的檔案中沒有包含 `config.py`。  
> 如果要讓程式完整執行，需要補上對應設定檔與必要環境設定。

---

## GitHub 下載建議

如果要在 GitHub 提供 Windows 使用者下載，建議不要直接放 `.exe` 在首頁。  
推薦做法是使用 GitHub Releases：

```text
cc69.zip
```

ZIP 裡面可以放：

```text
cc69/
├─ cc69.exe
├─ README.txt
└─ 其他必要檔案
```

然後在 GitHub 的 Releases 頁面提供下載。

---

## 免責與使用提醒

本工具僅供研究、測試與內部流程管理用途。  
使用時請遵守相關平台規範、服務條款與所在地法律規定。  
請勿將本工具用於違反平台規則、濫用服務、或造成他人困擾的行為。

---

## 專案名稱

```text
cc69
```
