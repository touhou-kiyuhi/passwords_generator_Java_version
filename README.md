# password_generator
## Rules
* 密碼規則說明
    1. 密碼最長有效期30天，請每30天更換密碼。
    2. 密碼最短使用期 1 天，變更後需 1 天過後方可變更新密碼。
    3. 密碼不可與前6次重覆
    4. 密碼必須符合複雜性需求
        * 長度至少為 14 個字元
        * 密碼中，不可包含帳號相關字眼
        * 包含下列四種字元中的四種
        * 英文大寫字元 (A 到 Z)
        * 英文小寫字元 (a 到 z)
        * 10 進位數字 (0 到 9)
        * 非英文字母字元 (例如: !、$、#、%)
    5. 修改密碼後請務必修改相關系統或郵件設定，並取消任何記憶密碼功能。
    6. 密碼錯誤10次將自動鎖定，15分鐘後自動解除，並請15分鐘後重新登入系統。
    7. 公司加入網域電腦，變更完，請重新開機或登出重新登入。
---
## 更新日誌
* 2025/01/28
    * **first commit**
    * **更新 README.md**
    * **修改 repository 名稱為 password_generator_Java_version**
    * **新增 Initialization 部分**
    * **修正 initialization\JsonInitialization.java 中的 bugs**
    * **完成 Initialization 部分**
* 2025/01/29
    * **更新 README.md**
    * **新增 password_generator\PasswordGenerator.java**
    * **新增 jsonControllerInitialization\JsonControllerInit.java ，更新 password_generator\PasswordGenerator.java 中的 Constructor 、 Getter, Setter 並先實現【使用者名稱、備份密碼 元素】部分**
    * **更新 password_generator\PasswordGenerator.java 並實現【設定 密碼長度、非英文字母字元長度、英文大寫字元 (A 到 Z)、英文小寫字元 (a 到 z)、10 進位數字 (0 到 9)、非英文字母字元 (例如: !、$、#、%)】部分**
    * **更新 password_generator\PasswordGenerator.java 並實現生成密碼**
    * **更新 password_generator\PasswordGenerator.java 中新增 checkPasswordSubstringsNotInUserName 、 checkPasswordNotInPasswordsBackupElements 以檢查生成出來的密碼是否符合規則**
    * **完成 password_generator 部分**
    * **修正 password_generator 名稱為 passwordGenerator**
    * **新增 Initialization 部分，使其繼承 jsonControllerInitialization**
    * **將 initialization_test 支線同步到 main ，完成 Initialization 部分**
    * **完成 Update Json 部分**
    * **更新 Main.java 函式名稱**
* 2025/02/03
    * **統一所有 Backup 名稱**
---
## 參考資料
* [ASCII可顯示字元（共95個）](https://zh.wikipedia.org/zh-tw/ASCII#%E5%8F%AF%E6%98%BE%E7%A4%BA%E5%AD%97%E7%AC%A6)
### Java
* [getter setter for Hashmap using generics](https://stackoverflow.com/questions/26306147/getter-setter-for-hashmap-using-generics)
* [Get values from List<Map<String, String>>](https://stackoverflow.com/questions/36410003/get-values-from-listmapstring-string)
* [Java HashMap With Different Value Types](https://www.baeldung.com/java-hashmap-different-value-types)
### Maven
* [在 VS Code 上建置 Maven 環境](https://jiaxiang2015.neocities.org/learning/java/vscode-maven)
* [Maven POM](https://www.runoob.com/maven/maven-pom.html)
* [Maven 构建生命周期](https://www.runoob.com/maven/maven-build-life-cycle.html)
### Test
* [（图文）详细介绍Maven的test命令](https://blog.csdn.net/weixin_43978412/article/details/99977481)
### Json
* [Java 中 JSON 的使用](https://www.runoob.com/w3cnote/java-json-instro.html)
* [Gson 與 Jackson](https://ithelp.ithome.com.tw/articles/10329180)
* [FasterXML/jackson](https://github.com/FasterXML/jackson)
* [好用的Jackson , 做一個POJO 和 JSON轉換的JSONUtils](https://central.sonatype.com/artifact/com.fasterxml.jackson.core/jackson-databind)
* [Java 使用 Jackson 進行JSON和Java物件互相轉換](https://lakesd6531.pixnet.net/blog/post/353231536)
* [Java Jackson ObjectMapper 教學與注意事項](https://ithelp.ithome.com.tw/articles/10310212)
* [Day13-實作(五)Jackson annotation](https://ithelp.ithome.com.tw/articles/10219803)
* [Jackson Java（它如何為開發者工作）](https://ironpdf.com/zh-hant/java/blog/java-help/jackson-java/)
* [How to parse JSON string with Jackson](https://mkyong.com/java/jackson-how-to-parse-json/)
* [What is the simplest way to configure the indentation spacing on a Jackson ObjectMapper?](https://stackoverflow.com/questions/28256852/what-is-the-simplest-way-to-configure-the-indentation-spacing-on-a-jackson-objec)
### Git
* [Git-了解分支&分支(建立、切換、刪除、回復)](https://ithelp.ithome.com.tw/articles/10211790)
* [Git 分支管理](https://www.runoob.com/git/git-branch.html)
* [功能開發完畢，要如何合併回主線呢？歡迎git merge，快轉merge](https://ithelp.ithome.com.tw/articles/10208932)
* [如何在 Git 中重命名本地或远程分支](https://www.freecodecamp.org/chinese/news/how-to-rename-a-local-or-remote-branch-in-git)