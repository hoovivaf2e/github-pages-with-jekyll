---
title: "Learning GitHub Pages"
date: 2020-07-28
---

在GitHub Pages的課程中，將創建一個託管在GitHub Pages上的部落格，並學習如何：

* 啟用GitHub Pages
* 使用靜態網站生成器 Jekyll
* 使用主題和內容自定義Jekyll網站


1. 啟用GitHub頁面 (Enable GitHub Pages)
	- 在你的儲存庫(Repository)名稱下，點擊【設置】(Settings)
	- 找到 GitHub Pages 的部分，在【來源】(Source)下拉列表中選擇【master】分支
	等待啟用GitHub Pages並啟動網站。

2. 自訂首頁 (Customize your homepage)
	- 可以通過向index文件或README.md文件添加內容來自定義主頁。GitHub Pages首先查找index文件。如果找到index文件，則GitHub Pages使用文件中的內容創建主頁。如果找不到index文件，則使用README.md來創建主頁。
	- 為此提交創建新分支並啟動拉取請求(pull request)

3. 合併分支 (Merge your pull request)
	- 將剛剛上傳的分支合併到 master 分支
 
4. 自定義網站詳細信息 (Customize site details)
	- Jekyll使用`_config.yml`來存儲網站的設定，設定主題和可重複使用的內容(如網站標題和GitHub設定)。
	- 為此提交創建一個新分支，並啟動拉取請求。

5. 建立網誌文章 (Create a blog post)
向您的部落格添加一些內容
	- 建立名為 _posts/YYYY-MM-DD-title.md 的文件
		* 如果您的博客發布日期未遵循正確的日期約定，則會收到錯誤消息，並且您的網站將無法構建。有關更多信息，請參見[頁面構建失敗：無效的發布日期](https://docs.github.com/en/github/working-with-github-pages/troubleshooting-jekyll-build-errors-for-github-pages-sites)。
	- 將更改提交到剛建立的分支。

6. Add blog post metadata
- 創建了文章後，可以對其添加語法。Jekyll文件使用的語法為YAML。它位於文件的頂部，看起來像這樣：

	```yaml
	---
	title: "Welcome to my blog"
	date: 2019-01-20
	---
	```

	還可以在這裡添加其他有用的東西，例如佈局，類別或任何其他對您有用的邏輯。相關配置可以參考[Jekyll front matter documentation](https://jekyllrb.com/docs/front-matter/)

7. 合併你的第一篇文章 (Merge your first post)
