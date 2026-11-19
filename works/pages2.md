# 多頁網站製作二：由多頁網頁建立詳細規格並維護網頁
- 學號：(請務必填寫)
- 姓名：(請務必填寫)
- 信箱：(請務必填寫)

## 作業目標

- 使用 AI 逆向整理全站共用規格及各頁詳細規格。
- 透過修改 Markdown 規格，更新網站內容。
- 使用 Git 保存修改紀錄，將規格及網頁同步至 GitHub。

> [!important]
> 本次流程：sitemap.md → AI → 三頁 HTML＋共用 CSS → AI → site.md＋各頁詳細規格 → 修改規格 → AI → 更新原網站。
> sitemap.md 是學生修改的初步大綱；site.md 是網站完成後，由 AI 整理的共用詳細規格。
> 所有路徑中的「學號」均須換成自己的學號。提示詞中的資料夾名稱也須一併修改。

## 操作流程

### 一、GitHub登入：
1. 登入(Sign in)：[https://github.com/signin](https://github.com/signin)
   - 使用Google帳號：![](../images/ContinueWithGoogle.png)

### 二、使用VSCode複製GitHub上2個儲存庫Repo
1. 使用 VS Code「檔案 → 開啟資料夾」，開啟資料夾：`D:\Web`
2. 開啟終端機，輸入git指令，設定GitHub帳號資訊
```shell
git config --global user.email [輸入EMail信箱]
```
```shell
git config --global user.name [輸入GitHub帳號]
```
3. 由GitHub複製Repo：WebSpec_學號、WebPage_學號
- GitHub網址：https://github.com/(GitHub名稱)/WebSpec_學號
- GitHub網址：https://github.com/(GitHub名稱)/WebPage_學號
```shell
git clone [貼上WebSpec網址]
```
```shell
git clone [貼上WebPage網址]
```

### 三、使用 AI 逆向生成詳細規格

1. 在 AI 對話框輸入以下提示詞，並替換學號：

```text
請讀取 WebPage_學號/pages/ 下的所有 HTML、
共用 CSS 及 JavaScript，依實際完成的網站逆向整理詳細規格。

請建立：
1. WebSpec_學號/pages/site.md
   記錄實際色碼、字體、字級、字重、行高、版面寬度、
   間距、導覽列、頁尾、按鈕、卡片、手機版及共用互動規則。
   包含共用檔案位置與各頁規格索引。

2. WebSpec_學號/pages/index.md
   記錄 index.html 的詳細規格。

3. WebSpec_學號/pages/about.md
   記錄 about.html 的詳細規格。

4. WebSpec_學號/pages/contact.md
   記錄 contact.html 的詳細規格。

各頁規格須記錄：
- 對應 HTML 的輸出位置
- 依循 site.md 的說明
- 區塊順序、實際文字、圖片路徑與替代文字
- 排列方式、按鈕、連結目的地、互動及手機版呈現

要求：
- 共用設計集中在 site.md，各頁內容集中在對應分頁規格。
- 規格須具體到足以支援後續修改網站。
- 與原 sitemap.md 不一致的地方，另列差異供我確認。
- 未完成的功能不可記為已完成。
- 保留 sitemap.md，本次只整理規格，不修改網頁。
```

2. 確認 site.md 與三份分頁規格都已建立。
3. 使用 VS Code「開啟側邊預覽」閱讀 Markdown。
4. 對照網站確認文字、圖片、連結及區塊順序。
5. 若有差異，確認預期內容後請 AI 修正。

> [!note]
> sitemap.md 保存初始大綱；site.md 管理共用詳細設計；
> home.md、about.md、contact.md 管理各頁內容。
> Markdown 是提供給 AI 閱讀的規格，瀏覽器實際載入的是 HTML、CSS 與 JavaScript。

### 四、修改分頁規格，再更新網頁

1. 開啟 WebSpec_學號/pages/about.md。
2. 自行修改至少一段文字，並新增一個內容區塊，例如團隊介紹或品牌理念。
3. 儲存規格檔案。
4. 在 AI 對話框輸入：

```text
我已修改 WebSpec_學號/pages/about.md。
請先讀取 WebSpec_學號/pages/site.md，
再比對更新後的 about.md 與
WebPage_學號/pages/about.html，
依新規格更新原本網頁，只修改有差異的部分。

沿用共用風格；若需新增專屬樣式，限定其作用範圍。
若修改共用 CSS，請檢查對首頁與聯絡我們的影響。
完成後核對規格與網頁一致，並說明修改項目。
```

5. 重新預覽，確認新增區塊及文字已更新。
6. 此次直接更新 about.html，不必另存 index2.html。

### 五、練習全站共用風格修改

1. 開啟 WebSpec_學號/pages/site.md。
2. 選擇一項共用設定修改，例如主色、按鈕圓角或內文字級。
3. 儲存後輸入：

```text
我已修改 WebSpec_學號/pages/site.md 的共用設計。
請依更新後的規格調整 WebPage_學號/pages/ 下的網站。
同步檢查三頁的共用樣式與手機版呈現，
保留各頁內容，核對網站與規格一致，並說明修改項目。
```

4. 逐頁確認三頁都已套用新的共用設定。
5. 如果只修改單頁文字或區塊，不需要修改 site.md。

### 六、提交並推送兩個儲存庫

1. 在 VS Code 原始檔控制中，分別選擇 WebSpec_學號 與 WebPage_學號。
2. 檢查本次修改的檔案。
3. 分別填寫版本說明、提交及推送。
4. 建議在完成初稿、整理規格與修改網站後，分別建立 Commit。
5. 版本說明範例：
   - 建立三頁網站大綱
   - 完成三頁網站與共用樣式
   - 整理共用及分頁詳細規格
   - 依規格新增關於我們內容
6. 到 GitHub 確認兩個儲存庫均已同步。

### 七、填寫成果紀錄

- 網站主題：
- WebSpec 儲存庫網址：
- WebPage 儲存庫網址：
- 網站展示網址（已啟用 GitHub Pages 者填寫）：
- 本次修改的分頁規格：
- 新增的內容區塊：
- 修改的全站共用設定：
- 遇到的問題及處理方式：

## 完成檢查

- [ ] 已填寫本檔的學號、姓名與信箱。
- [ ] 字體、配色、按鈕、導覽列及頁尾一致。
- [ ] 已生成 site.md 與三份分頁詳細規格。
- [ ] 已修改 about.md，並成功更新文字及新增區塊。
- [ ] 已修改 site.md，並確認三頁共用樣式同步更新。
- [ ] 已填寫成果紀錄。
- [ ] 已將規格與網頁分別提交、推送，並在 GitHub 核對。

> [!important]
> 請依教師指定期限完成。繳交前務必確認 GitHub 上的內容已更新；
> 僅儲存在電腦，尚未提交及推送，不算完成同步。

