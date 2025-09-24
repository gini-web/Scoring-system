# 評分系統（無後端版，GitHub Pages）

- 版本：v1.0｜建置：20250924-040054（UTC）
- 無需 Firebase / 後端，資料存放在 **瀏覽器 localStorage**（鍵：`rating_scores_v1`）。
- 支援 **JSON 匯入/導出**、**CSV 導出**，可離線使用。
- 以 **/docs** 目錄發布到 GitHub Pages。

## 發佈步驟
```bash
git init
git add .
git commit -m "init: rating system (local)"
git branch -M main
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```
GitHub → **Settings → Pages**：選擇 `main` 分支、資料夾 `/**docs**`，儲存即可。

## 匯入/導出
- 右上方按鈕可 **導出 JSON/CSV**；亦可 **匯入 JSON**（跨裝置備份/搬移）。
- 欄位：judge、presenter、各評分項、total_score、weighted_score、comment、created_at。
