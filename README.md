# 📚 myskills - Hsieh's Claude Skills Collection

一套為教育工作者設計的 Claude 技能集合，涵蓋考卷設計、教學文件製作、Web 應用開發、設計系統等多個領域。適用於 SIVS（彰師附工）及其他教育機構的教學自動化和內容創作。

## 🎯 核心技能

### 📖 教學與評量
- **exam-designer** - 英語考卷自動設計系統（A2–B1 難度）
- **docx-teaching** - SIVS 教學文件製作（講義、學習單、成績單、公告）

### 🛠️ 開發與自動化
- **gas-webapp-builder** - Google Apps Script Web App 前後端整合
- **notion-daily-scheduler** - Notion 每日自動排程與防重複架構

### 🎨 設計系統
- **ckmdesign** - 綜合設計系統（logo、CIP、banner、icon、社群貼文）
- **ckmdesign-system** - 設計 tokens 架構與元件規格
- **ckmbrand** - 品牌聲音、視覺識別、訊息框架
- **ckmbanner-design** - 多平台 banner 設計（社群、廣告、網頁、列印）
- **ckmslides** - HTML 策略簡報製作（Chart.js）
- **ckmui-styling** - shadcn/ui + Tailwind 無障礙 UI 組件

### 💡 推薦與比較
- **product-recommender** - 智慧商品推薦（口碑、評價、場景）
- **price-comparison** - 跨平台商品比價（台灣電商、國際平台）

### 📊 UI/UX 設計
- **ui-ux-pro-max** - UI/UX 設計智能（50+ 風格、161 色板、57 字體配對）

## 🚀 快速開始

### 方法 1：查看 Skill 索引
```json
{
  "查看所有 skill": "SKILLS_INDEX.json",
  "描述和標籤": "每個 skill 都有詳細說明和觸發關鍵字"
}
```

### 方法 2：複製 Raw URL 給 Claude
每個 skill 的 `SKILL.md` 都可以透過以下格式使用：

```
https://raw.githubusercontent.com/iammiles-gif/myskills/main/{skill-name}/SKILL.md
```

範例：
```
exam-designer:
https://raw.githubusercontent.com/iammiles-gif/myskills/main/exam-designer/SKILL.md

gas-webapp-builder:
https://raw.githubusercontent.com/iammiles-gif/myskills/main/gas-webapp-builder/SKILL.md
```

### 方法 3：使用 SKILLS_INDEX.json
載入索引檔案，一次看所有 skill 的描述、版本、標籤：
```
https://raw.githubusercontent.com/iammiles-gif/myskills/main/SKILLS_INDEX.json
```

## 📋 Skill 清單

| Skill | 分類 | 用途 |
|-------|------|------|
| exam-designer | 教學 | 英語考卷自動設計 |
| docx-teaching | 教學 | 教學文件、講義、成績單 |
| gas-webapp-builder | 開發 | GAS 網頁應用前後端 |
| notion-daily-scheduler | 自動化 | Notion 每日排程任務 |
| ckmdesign | 設計 | 綜合品牌設計系統 |
| ckmdesign-system | 設計 | 設計 tokens + 元件 |
| ckmbrand | 設計 | 品牌聲音與視覺識別 |
| ckmbanner-design | 設計 | 多平台 banner 設計 |
| ckmslides | 設計 | HTML 策略簡報 |
| ckmui-styling | 設計 | 無障礙 UI 組件庫 |
| product-recommender | 工具 | 智慧商品推薦 |
| price-comparison | 工具 | 跨平台比價系統 |
| ui-ux-pro-max | 設計 | UI/UX 設計智能 |

## 📁 資料夾結構

```
myskills/
├── README.md                  # 本文件
├── SKILLS_INDEX.json          # 所有 skill 的索引與詳細資訊
├── exam-designer/
│   └── SKILL.md              # Skill 定義檔
├── docx-teaching/
│   └── SKILL.md
├── gas-webapp-builder/
│   └── SKILL.md
├── notion-daily-scheduler/
│   └── SKILL.md
├── ckmdesign/
│   ├── SKILL.md
│   ├── data/                 # 設計資料（色板、字體配對等）
│   ├── scripts/              # 自動化腳本
│   └── references/           # 參考資料
├── ckmdesign-system/
│   ├── SKILL.md
│   ├── data/
│   ├── scripts/
│   └── templates/
├── ckmbrand/
├── ckmbanner-design/
├── ckmslides/
├── ckmui-styling/
├── product-recommender/
├── price-comparison/
└── ui-ux-pro-max/
    ├── SKILL.md
    ├── data/
    ├── scripts/
    └── canvas-fonts/        # 預加載字體
```

## 🔗 如何使用這些 Skill

### 與 Claude 一起工作

**直接告訴 Claude 使用某個 skill：**
```
請使用這個 skill：
https://raw.githubusercontent.com/iammiles-gif/myskills/main/exam-designer/SKILL.md

然後幫我設計一份 A2 程度的英文考卷...
```

**或者上傳 SKILL.md 檔案：**
1. 從本 repo 下載 `exam-designer/SKILL.md`
2. 上傳給 Claude
3. 告訴 Claude 使用該 skill

### 在 Cowork 或自動化中使用

將 raw URL 放入 prompt：
```markdown
## Available Skills
- Exam Designer: https://raw.githubusercontent.com/iammiles-gif/myskills/main/exam-designer/SKILL.md
- GAS Webapp: https://raw.githubusercontent.com/iammiles-gif/myskills/main/gas-webapp-builder/SKILL.md
```

## 📖 每個 Skill 的主要用途

### exam-designer 英語考卷設計
- 輸入：英文單字表、英文課文、文法句型
- 輸出：選擇題、克漏字、閱讀測驗
- 難度：A2–B1 CEFR
- 搭配：docx-teaching 輸出 Word 檔

### gas-webapp-builder GAS 網頁應用
- 前後端整合
- Sheet 即時寫入
- CORS 處理、API 代理
- 教學互動工具、儀表板、遊戲化平台

### ckmdesign 綜合設計系統
- Logo 設計（55 種風格）
- 企業識別系統 (CIP)
- HTML 簡報與 Chart.js
- 多平台 banner（社群、廣告、列印）
- SVG icon 設計
- 社群貼文自動化

### notion-daily-scheduler Notion 排程
- 每日自動內容生成
- 防重複架構
- Cowork Scheduled Task 整合
- 適合：書摘、新聞摘要、學習筆記、日誌

## 🔧 技術棧

- **Google Apps Script** - 後端自動化、Sheet 操作、PDF 生成
- **Claude API** - 內容生成、題目設計、推薦引擎
- **Notion API** - 資料庫管理、排程任務
- **HTML/CSS/JavaScript** - 前端介面、互動工具
- **Chart.js** - 資料視覺化
- **Tailwind CSS + shadcn/ui** - UI 元件庫
- **SVG** - 設計與圖示

## 📝 授權

MIT License - 你可以自由使用、修改和分發這些 skill，只需保留版權聲明即可。

## 💬 使用建議

### 對教師
- 使用 `exam-designer` 快速生成出題
- 用 `docx-teaching` 批量製作教材
- 用 `gas-webapp-builder` 建立互動課堂工具
- 用 `notion-daily-scheduler` 自動更新教學資源

### 對開發者
- 參考 `gas-webapp-builder` 的 GAS 最佳實踐
- 研究 `ckmdesign-system` 的 token 架構
- 學習 `ckmui-styling` 的元件設計模式
- 參考 `notion-daily-scheduler` 的防重複策略

## 🔄 版本管理

每個 skill 的版本資訊存放在 `SKILLS_INDEX.json` 中。查看更新日誌：

```bash
git log --oneline -- {skill-name}/SKILL.md
```

## 🤝 貢獻與改進

如果你改進了某個 skill，可以：
1. Fork 本 repo
2. 修改 skill 檔案
3. 更新 `SKILLS_INDEX.json` 中的版本
4. 提交 Pull Request

## 📞 聯絡

- GitHub: [@iammiles-gif](https://github.com/iammiles-gif)
- SIVS 英文教學部門

---

**最後更新：2026-04-27**  
**Skill 總數：13**  
**總容量：~8MB**

立即選擇一個 skill，開始提升教學效率吧！ 🚀
