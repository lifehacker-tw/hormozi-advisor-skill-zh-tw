# AI 顧問：Hormozi（非官方・台灣用語版）

本版改編自香港學員 **RS0715** 的 [原始作品](https://github.com/RS01985/hormozi-advisor-skill)。感謝他同意我們 fork，讓台灣讀者也能使用這份知識整理。原作者經營 [Whale Digital Consulting](https://whaledigitalconsulting.com.au/)；本版依 [CC BY 4.0](LICENSE) 標示來源與修改內容，詳見 [CHANGES.md](CHANGES.md)。

原作者把 Alex Hormozi 官方 YouTube 頻道 518 部公開影片（約 218 小時）整理成一位能追溯出處的 AI 商業顧問，聚焦成長經濟、Offer、瓶頸（constraint）和單位經濟（unit economics）。本版保留原有知識庫，調整成台灣常用的繁體中文，並補上兩項決策檢查。

> ⚠️ 本作品不是 Alex Hormozi 本人，也不是他或 Acquisition.com 的官方產品，與他沒有授權、合作或背書關係。原作者的 510 份字幕逐字稿（另有 8 部無官方字幕）與 518 份逐片筆記沒有公開；本版也未重新核對全部影片。

## 它會做什麼

問它一個商業決策，它先讀本 repo 的知識庫，再回答四段：

1. **本質**：問題卡在成長鏈（市場 → Offer → 潛在客戶 → 銷售 → 交付 → 留存 → 現金）哪一環
2. **底層邏輯**：實際套用總綱框架，每個論點標出處
3. **我會怎麼做**：提出 2～3 項有負責人、數字、期限與停止條件的行動
4. **盲點**：指出需要本地資料、專業意見或其他角度的部分

它也寫明適用邊界：所在地區的法規與稅務、投資建議、品牌文案的最後定稿不在範圍內；影片中的收入數字只當講者自述。

## 安裝

```bash
npx skills add lifehacker-tw/hormozi-advisor-skill-zh-tw
```

也可以手動：把整個資料夾放進你所用 Agent 的 skills 目錄。

用法：「問 Hormozi：……」或「用 Hormozi 角度看看……」。

## 內容

| 檔案 | 內容 |
|:--|:--|
| `SKILL.md` | 顧問設定：角度、四段輸出、誠實線、紀律 |
| `references/advisor-card.md` | 素材範圍、三條心法、管與不管、12 條反模式、矛盾與張力、批評者角度、三關篩選 |
| `references/playbook.md` | 518 部跨影片知識總綱（主正本）；「代表影片」直接連到 YouTube |
| `docs/tests.md` | 6 條回歸測試題與結果（Skill 作答時不讀） |

知識庫的顧問卡與測試說明已轉成台灣用語；總綱原本就是書面語。關鍵術語和原片連結均保留。

## 測試結果

以下是**原作者的測試紀錄**，不是本版的獨立測試。同一組題目使用 Claude Sonnet（2026-09-28 公開版為 Claude Sonnet 5；2026-09-16 兩組未記錄確切版本）：

| 版本 | 答過題要點 | 作假出處 | 作數字 | 新情境標「推測」 |
|:--|:--|:--|:--|:--|
| 只靠模型印象（2026-09-16） | 6/9 | 3 句 | 1 題 | 0/1 |
| 作者私人完整版（可讀逐片筆記與逐字稿，2026-09-16） | 9/9 | 0 | 0 | 1/1 |
| 本公開版（2026-09-28） | 7/9（另 1 點半中） | 0 | 0 | 1/1 |

公開版沒有收錄逐片筆記：Q1 的「降價 25%，銷量需增加逾 33% 才能維持營收」原本未明寫在公開總綱。台灣用語版的 `SKILL.md` 已加入通用算式 `1 ÷ (1 − 降價比例) − 1`，這是算術推導，並非 Hormozi 原話。逐題細節見 [docs/tests.md](docs/tests.md)。

## 授權

- 原作者撰寫的整理、顧問設定與測試題以 [CC BY 4.0](LICENSE) 授權：可以 fork、修改、翻譯與分享；必須註明原作者、附上原作連結與授權連結，並標明修改內容。
- Alex Hormozi 的原創內容、名稱與商標不屬作者，不在上述授權範圍內，詳見 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。
- 本版署名：`原作 RS0715 · Whale Digital Consulting｜台灣用語改編 雷蒙三十｜CC BY 4.0`

## 作者

原作者 RS0715，經營 [Whale Digital Consulting](https://whaledigitalconsulting.com.au/)。台灣用語改編：雷蒙三十。
