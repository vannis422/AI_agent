# 探針筆記 / Probe Notes

繁體中文 PubMed 論文導讀網站，首篇介紹 Jaskot 等人（2025）的 PFB-FDG 物種選擇性研究。
純 HTML/CSS；無需安裝或登入即可在電腦本機閱讀。

## 1. 先看網站
解壓縮整個專案，雙擊 index.html，以 Chrome 或 Edge 開啟。
不要只搬走 index.html：assets 與 papers 資料夾必須一起保留。
首頁點「閱讀導讀」可開啟文章，左上連結可以返回首頁。

## 2. AGENTS.md 怎麼用
這是寫給 AI 的專案說明書，不是要貼到網頁執行的程式。
在能讀取專案檔案的 AI 開發工具開啟此資料夾，再明確要求先閱讀 AGENTS.md。
若使用一般聊天介面，附上 AGENTS.md、templates/paper.html、既有文章與論文來源。
不要只給論文標題就要求 AI 補齊所有研究數據。

可直接使用的指令：
> 請先閱讀 AGENTS.md、README.md、templates/paper.html 與 papers/40603620.html。
> 我想新增這篇論文：[貼上 PubMed 連結]。
> 請核對原始來源，依照範本建立 papers/<PMID>.html，更新首頁清單與篇數。
> 區分實驗結果與機制推測，不編造未提供的數據或我的個人心得。
> 最後依照 AGENTS.md 檢查並告訴我哪些項目尚未驗證。

## 3. 上傳 GitHub（網頁介面）
1. 登入 GitHub，建立新的公開 Repository，例如 pubmed-probe-notes。
2. 在空白 Repository 選 uploading an existing file；已有內容時選 Add file → Upload files。
3. 將本專案資料夾「裡面的所有檔案與子資料夾」拖入上傳區。
   根目錄必須直接看到 index.html、AGENTS.md、assets/、papers/、templates/。
   不要只上傳 ZIP，也不要多包一層 pubmed-probe-notes 資料夾。
4. 寫入提交訊息，例如 Add paper reading website，按 Commit changes。
5. 確認 AGENTS.md 與網站檔案都已出現在 Repository。

## 4. 公開網站
1. 開啟 Repository 的 Settings → Pages。
2. Build and deployment → Source 選 Deploy from a branch。
3. Branch 選 main，資料夾選 /(root)，按 Save。
4. 等待部署完成；若尚未完成，可在 Actions 查看進度與錯誤。
5. 回到 Pages，使用顯示的實際網站連結。不要把預期網址當成已發布成果。
6. 使用未登入的瀏覽器測試首頁、文章與返回連結。
官方說明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

一般專案網址形式是 https://<帳號>.github.io/<Repository名稱>/。
這份檔案包本身尚未部署。

## 5. 繳交前
閱讀首篇原文，加入自己的心得並檢查 AI 摘要。
填寫 SUBMISSION.md 的學校、學號、系級、姓名、Repository 與實際網站網址。
不必把個人學號放到公開網站；可只填在課程繳交介面。

## 6. 延伸方式
固定規則（AGENTS.md）＋固定版型（templates/paper.html）＋共用 CSS，
讓新文章沿用一致風格與證據標準。每篇文章有獨立網址，可直接分享。

## 來源與聲明
PubMed：https://pubmed.ncbi.nlm.nih.gov/40603620/
全文：https://pmc.ncbi.nlm.nih.gov/articles/PMC12222868/
網站文字為 AI 協助製作的中文導讀，未重製原文圖片；非 PubMed 官方服務。

