# khazix-writing-skill

基於對「數字生命卡茲克（@Khazix0918）」**2026 全年 184 篇 X 長文（Articles）**與其公開內容方法論的系統實證蒸餾，封裝而成的開箱即用 **中文深度長文寫作 Agent Skill**。

適用於 **Claude Code、Codex CLI、Antigravity、Cursor、Grok Build** 等支援標準 `SKILL.md` 的 AI Agent。

> **聲明**：本專案旨在學習與複用「有見識的普通人在認真聊一件打動他的事」之敘事結構、口述呼吸感、喜劇「升三番」節奏與去 AI 味紅線；敘述者始終是使用者本人，**不會冒充原作者身份，也不會捏造第一人稱假經歷**。

---

## 核心特色（與一般「文風模仿 Prompt」的差別）

這不是只塞了一堆「講道理、牛逼、呆逼」的模仿秀，而是從 184 篇真實長文與 2026 下半年最新演化中提煉出的寫作作業系統：

1. **材料先行，拒絕瞎編**：動筆前先過「開題五問」檢查是否有真實經歷、數據、動作或踩坑傷口；材料不足先追問最多 3 題，絕不編造假親歷。
2. **修正自述盲區**：實證區分「實測／教程／系統復盤類（清晰 `一、二、三`＋`寫在最後`）」與「人文／單點敘事類（無編號流淌式白描）」。
3. **喜劇「升三番」推進引擎**：多個案例或測評點不平鋪直敘，按「常規預期 → 真實踩坑反差 → 腦洞炸裂高潮」層層遞進，拉高長文完讀率。
4. **語音口述呼吸感 ＋ 末句慢鏡頭斷裂**：短段交替、原件直貼＋人話秒翻、收尾碎句留白，以及高文學濃度時自動撤除「求三連」口播。
5. **2026 最新去 AI 味紅線**：全面封殺翻案腔（`不是……而是……`、`與其說……不如說……`）、AI 路標詞（`說白了`、`這意味著`、`值得注意的是`）、破折號 `——` 與過度堆砌口頭禪。

---

## 快速安裝

### 方式一：使用 `skills` CLI（推薦）

```bash
npx skills add ChrisHKAI/khazix-writing-skill
```

### 方式二：手動安裝到 Claude Code / Codex / Antigravity / Cursor

```bash
git clone https://github.com/ChrisHKAI/khazix-writing-skill.git

# Claude Code
cp -r khazix-writing-skill/skills/khazix-longform-writer ~/.claude/skills/

# Codex CLI
cp -r khazix-writing-skill/skills/khazix-longform-writer ~/.codex/skills/

# Antigravity
cp -r khazix-writing-skill/skills/khazix-longform-writer ~/.gemini/config/skills/
```

---

## 使用方式

安裝完成後，在對話中直接觸發即可：

- 「用 `khazix-longform-writer` 幫我把這次用 AI 做 3D 動畫的踩坑經歷寫成 X 長文，口語吐槽多一點，簡體中文」
- 「幫我把這份產品實測筆記，按卡茲克長文節奏改寫成一篇 4,000 字深度評測」
- 「用卡茲克寫作風格幫我給這篇文章去 AI 味、拉高完讀率」

---

## 倉庫結構

```text
khazix-writing-skill/
├── README.md
├── LICENSE
└── skills/
    └── khazix-longform-writer/
        ├── SKILL.md                         # 主 Skill 規範（可直接被 Agent 載入）
        └── references/
            ├── style-distillation.md        # 184 篇全量實證風格蒸餾報告
            └── templates-and-checklists.md  # 三大文體骨架模板與 60 秒終審清單
```

## License

MIT
