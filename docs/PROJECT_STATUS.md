# Project Status

GitHub 個人主頁（`ShowXD/ShowXD`），內容只有 `README.md` 與產生貪吃蛇動畫的 workflow。

## 目前狀態（2026-11-04，branch `main`）

已 commit 並 push（`d7d545c`）：

- `README.md`：標語改為 Software Engineer；技能徽章依現有技能重寫並分組；Twitter 改為 X；修正 LinkedIn 連結；統一徽章樣式。
- `.github/workflows/main.yml`：`crazy-max/ghaction-github-pages` 升到 `v5`（Node 24）；`Platane/snk/svg-only@v3` 維持不變。

已修改，尚未 commit：

- `.github/workflows/main.yml`：新增 `actions: write` 權限，以及每次執行時用 `gh api` 重新啟用自己的步驟，避免 repo 60 天沒有活動時排程被 GitHub 自動停用。
  （原本常用的 `gautamkrishnar/keepalive-workflow` 已被 GitHub 封鎖，無法使用。）

## 阻塞

- 排程 workflow 目前處於停用狀態，需要手動到 Actions 頁面按 Enable workflow；停用期間連 push 也不會觸發。

## 驗證

- 39 個 shields.io 徽章皆回 200，指定 logo 的徽章都有顯示 logo。
- 社群連結皆回 200；LinkedIn 回 999（反爬蟲機制，屬正常）。
- workflow 尚未在 GitHub 上執行，要推送後才能確認 `output` 分支有正常產出 SVG。

## 約定

- 徽章使用 shields.io，logo 用 Simple Icons slug；Simple Icons 沒有的品牌（如 Microsoft 系列、Semgrep、Gitleaks、Cursor）只放文字。
- SonarQube 的 slug 是 `sonarqubeserver`，不是 `sonarqube`。

## 下一步

- 在 Actions 頁面啟用 `generate animation`，commit 並 push keepalive 的修改，再手動 Run workflow，確認三個步驟都成功、`output` 分支的 SVG 有更新。
