# AGENTS.md - NBA 球員進攻框架分析庫（Court Vision）開發規範

## 1. 專案目的
本專案為個人「NBA 球員進攻框架分析庫（Court Vision）」，旨在將不同球星的進攻體系、武器庫與戰術定位，拆解為結構化的圖文網頁。本文件的目的是讓 AI 協作時，能完全理解網站架構與分析框架，並在維持統一視覺風格的前提下，快速新增或更新球員分析頁面。

## 2. 技術棧與檔案結構
本專案採用純靜態網頁開發（HTML5 + Tailwind CSS CDN），無需任何建置工具（Build tools），可直接透過 GitHub Pages 部署。

```text
nba-offense-lab/
├── AGENTS.md                 # 本專案開發與擴充規範文件
├── index.html                # 首頁（網站介紹、篩選標籤與所有球員卡片總目錄）
└── players/                  # 存放所有獨立球員分析頁面的資料夾
    ├── template.html         # 空白球員分析範本（AI 新增頁面時必須參考此結構）
    └── kyrie-irving.html     # 第一位球員範例：Kyrie Irving 進攻框架解析
