# 这个仓库存放的是hexo的源文件
### 每次克隆到本地后，要把项目里的除了.git文件夹之外的所有文件夹替换本地的hexo的blog目录里,其实替换的目录就是下面这些
+ scaffolds
+ source
+ themes
+ .gitignore
+ _config.yml
+ db.json
+ package.json
+ package-lock.json

    
### 每次修改或更新博文后一定也要记得同步本仓库！！！
+ 更新方法同样是复制粘贴
+ 如何同步
    ```
    git status
    git add .
    git commit -m "你的更新信息"
    git remote add origin git@github.com:sherlockhsyoung/hexoFiles.git
    git push origin master 
    ```
    + 如果不幸遇到错误
        ```
        $ git push origin master
        To github.com:sherlockhsyoung/hexoFiles.git
        ! [rejected]        master -> master (fetch first)
        error: failed to push some refs to 'git@github.com:sherlockhsyoung/hexoFiles.git'
        hint: Updates were rejected because the remote contains work that you do
        hint: not have locally. This is usually caused by another repository pushing
        hint: to the same ref. You may want to first integrate the remote changes
        hint: (e.g., 'git pull ...') before pushing again.
        hint: See the 'Note about fast-forwards' in 'git push --help' for details.
        ```
        + 解决方法
        + 强制push
            ```
            git push origin master --force
            ```
        + [stackoverflow上的完整答案](https://stackoverflow.com/questions/28429819/rejected-master-master-fetch-first)