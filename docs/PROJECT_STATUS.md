# Project Status

GitHub 個人主頁（`ShowXD/ShowXD`），內容只有 `README.md` 與產生貪吃蛇動畫的 workflow。

## 目前狀態（2026-11-04，branch `main`，基於 `3af85cd`）

已完成，尚未 commit：

- `README.md`：標語改為 Software Engineer；技能徽章依現有技能重寫並分組；Twitter 改為 X；修正 LinkedIn 連結；統一徽章樣式。
- `.github/workflows/main.yml`：`crazy-max/ghaction-github-pages` 升到 `v5`（Node 24）；`Platane/snk/svg-only@v3` 維持不變。

## 驗證

- 39 個 shields.io 徽章皆回 200，指定 logo 的徽章都有顯示 logo。
- 社群連結皆回 200；LinkedIn 回 999（反爬蟲機制，屬正常）。
- workflow 尚未在 GitHub 上執行，要推送後才能確認 `output` 分支有正常產出 SVG。

## 約定

- 徽章使用 shields.io，logo 用 Simple Icons slug；Simple Icons 沒有的品牌（如 Microsoft 系列、Semgrep、Gitleaks、Cursor）只放文字。
- SonarQube 的 slug 是 `sonarqubeserver`，不是 `sonarqube`。

## 下一步

- 確認 diff 後 commit，push 到 main，觀察 Actions 執行結果。
