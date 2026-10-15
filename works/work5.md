# 第5次作業(3%)
- 學號：(請務必填寫)
- 姓名：(請務必填寫)
- 信箱：(請務必填寫)

## 作業目標
### 一、VSCode + Extensions + Git 使用一鍵安裝：
1. 請於以下連結下載後，並**以系統管理員身分執行**：[下載](https://ocu.tw/download/VSCodeAI.exe)

### 二、VSCode複製GitHub上2個儲存庫Repo
1. 選擇放置儲存庫的資料夾：`D:\Web`
2. 開啟終端機，輸入git指令
- 請將EMail信箱更換為GitHub的申請信箱
```shell
git config --global user.email [輸入EMail信箱]
```
- 請將GitHub帳號更換為GitHub帳號
```shell
git config --global user.name [輸入GitHub帳號]
```
3. 由GitHub複製Repo：WebSpec_學號
- GitHub網址：https://github.com/(GitHub名稱)/WebSpec_學號
```shell
git clone [貼上WebSpec網址]
```
4. 由GitHub複製Repo：WebPage_學號
- GitHub網址：https://github.com/(GitHub名稱)/WebPage_學號
```shell
git clone [貼上WebPage網址]
```

### 三、在VSCode上開啟/WebSpec_學號/specs/onepage.md
1. 另存為/WebSpec_學號/specs/onepage1.md

### 四、修改/WebSpec_學號/specs/onepage1.md
1. 修改hero區域，目標為增加一個既有的圖片
   1. 將右欄的內容改為：
      ```htm
      不使用 CSS 插畫，使用既有圖片
      ```
   2. 在hero區域，增加以下內容
      ```html
      **右欄圖片**

      - 檔案位置
      - `images\hero.jpg`
      - 使用 `<img>` 元素顯示
      - 圖片寬度：400px
      - 圖片高度：300px
      ```

### 五、在VSCode將檔案/WebSpec_學號/specs/onepage1.md上傳至GitHub

### 六、使用AI工具產生符合意境的圖片
1. 開啟Gemini，選擇輸入以下的提示詞：
   ```html
   - 由AI生成以下圖片 
   - 圖片為實景，比例為4:3 
   - 室內空間，在窗戶前，有一張桌子和椅子，桌上放有濾杯與咖啡壺 
   - 窗外為太陽、及山景，具有藍天白雲的天空
   ```
2. 下載圖片，並儲存至/WebSpec_學號/onepage1/images/hero.jpg

### 七、使用AI工具製作網頁
1. 開啟AI工具視窗或單機版程式(以下以Codex為例)
2. VSCode + Codex Extension製作網頁
   1. 使用VSCode開啟/WebSpec_學號/specs/onepage1.md
   2. 開啟Codex側邊對話框，輸入以下提示詞
      ```htm
      請依據目前開啟的內容為網頁規格，製作一個網頁index.html，並儲存於資料夾：WebPage_學號/onepage1/中
      ```
3. 檢查/WebPage_學號/onepage1/index.html網頁內容
4. 以瀏覽器或Live Server Extension檢視網頁

### 八、在VSCode將資料夾/WebPage_學號/onepage1上傳至GitHub
   
## 評分方式
- 檢查項目：完成後請打勾
    - [ ] 在VSCode上修改/WebSpec_學號/works/work5.md：填寫學號、姓名，並同步於在GitHub上
    - [ ] 在VSCode上複製/WebSpec_學號/specs/onepage1.md：修改各項內容後，並同步於在GitHub上
    - [ ] 在VSCode使用AI工具以onepage1.md生成/WebPage_學號/onepage1/index.html網頁，並同步於在GitHub上
    - [ ] 在GitHub上確認以上檔案是否完全同步內容

> [!important]
> 請於上課時完成，若未到課同學，請於下次上課(**第6週**)前完成
