# 學生 Agent 入門（教學簡報網頁）

屏北高中「學生 Agent 入門」暗色簡報式網頁，**老師投影、帶學生一起做**。單一 `index.html`，不需要建置工具。

預定網址：https://frentexx.github.io/ppsh-student-agent-intro/（GitHub Pages，尚未上線時打不開）

## 內容（21 頁）

| 區段 | 頁 | 內容 |
|---|---|---|
| 開場 | 1–2 | 封面、今天的三件事 |
| A 認識 Agent | 3–9 | Chat AI vs Agent、五個組成（LLM／Context／Memory／Tools／Harness）、LLM vs Harness、Context 桌面、專案資料夾、技能、交辦四問 |
| B 領取點數 | 10–14 | 點數池三個限制、**班級密碼**免登入領取、套用設定 ZIP、個人⇄專案點數池切換、三條安全規則 |
| C 專案起始 | 15–17 | 初始化／開工／收工、初始化的環境檢查、**作業成果**資料夾規則 |
| D 動手生成 | 18–19 | 圖片與影片的範例提示語（可一鍵複製） |
| E 做完之後 | 20–21 | 學習歷程報告、帶走清單 |

不含：MCP、教材與考卷製作、ComfyUI 工作流與提示語教學（由美術老師教）、平台分享者端功能（建池、報告、組織額度）。

## 操作

- `←` `→`／空白鍵：換頁　`F`：全螢幕　`N`：顯示／隱藏講者備忘稿　`Home`／`End`
- 網址後加 `#7` 直接跳到第 7 頁
- 手機（寬度 900px 以下）自動改為直向捲動閱讀

## 檔案

```
index.html     成品（由 _parts 合併而成，直接部署這個）
_parts/        原始分段：00-head（CSS）、10/20/30（各區段投影片）、90-foot（JS）
```

修改後重新合併：

```bash
cat _parts/00-head.html _parts/10-slides-a.html _parts/20-slides-b.html _parts/30-slides-c.html _parts/90-foot.html > index.html
```

## 注意

- **班級密碼、Token、設定 ZIP 不放進本網頁與本 repo。**
- Codex 的實際畫面（提供者與點數池確認位置）、Codex 內建生圖、影片工具與 ComfyUI 連線方式，投影片與備忘稿中標有「待實測」，請先在教室電腦走一遍再上課。
- 搭配技能包：[ppsh-student-agent-starter](https://github.com/frentexx/ppsh-student-agent-starter)

## 授權與來源

內容採 CC BY-NC-SA 4.0。概念部分改編自屏北高中 AI Agent 概念入門教材，其中部分改編自三師爸 Sense Bar（經原作者同意教育使用與改作）；領取點數的步驟依 NMKING AI Gateway 分享者操作手冊 v2.6 整理，畫面以平台當下為準。
