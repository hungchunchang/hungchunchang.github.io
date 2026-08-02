# \_private

本機專用的暫存區。這個資料夾裡除了本檔案以外，**所有內容都被 `.gitignore` 排除**，不會被 commit、不會出現在 GitHub 上，也不會被 Jekyll build（底線開頭的資料夾預設就不會進 `_site`）。

適合放：

- 旅遊行程表、訂票與住宿資訊、收據
- 現場流水帳、還沒整理成文章的筆記
- GPX 軌跡、照片原檔
- 任何含有他人姓名、聯絡方式、地址的東西

## 重要前提

這個 repo 是 **公開的**。`published: false` 只是叫 Jekyll 不要 build，檔案本身在 GitHub 上仍然全文可讀 — 它不是隱私機制。要私密就放這裡，或放在 repo 之外。

而且 **git 歷史是永久的**：東西一旦 commit 進去，之後刪掉也還留在歷史裡，除非重寫歷史並強制推送。所以判斷要在 commit 之前做。

## 注意

- 這裡的東西 **不受 git 保護也不會同步到 GitHub**，備份請靠 iCloud / Time Machine。
- 照片原檔請留在這裡，只把縮圖（約 1600px 寬）放進 `assets/img/blog_photo/`。大圖一旦進 git 就永久留在歷史裡，會讓 clone 和 build 越來越慢。
