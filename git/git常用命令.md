### 分支管理

* 创建分支

    ```bash
    git branch dev
    ```

* 切换分支

    ```bash
    git checkout dev
    ```

* 创建并切换分支

    ```bash
    git checkout -b dev
    ```

* 查看当前分支  该命令会列出所有分支，当前分支前会标有一个`*`号

    ```bash
    git branch
    ```

* 查看远程分支

    ```bash
    git branch -r
    ```

* 删除本地分支

    ```bash
    git branch -d dev
    ```

### 暂存与恢复

* 将当前未提交的修改暂存起来

    ```bash
    git stash
    ```

* 将当前未提交的修改暂存起来，并添加说明信息，便于了解stash的内容

    ```bash
    git stash save '说明信息'
    ```

* 列出当前仓库下的stash列表条目，每条均以`stash@{n}`来标识

    ```bash
    git stash list
    ```

* 恢复暂存到当前分支，若不加`stash@{n}`则默认恢复第一条，且stash内容不会被删除

    ```bash
    git stash apply stash@{n}
    ```

* 删除stash内容，若不加`stash@{n}`则默认删除第一条，可以指定`stash@{n}`来删除指定的stash条目

    ```bash
    git stash drop stash@{n}
    ```

* 恢复暂存并删除stash内容，若不加`stash@{n}`则默认恢复和删除第一条，可以指定`stash@{n}`来指定恢复和删除的stash条目

    ```bash
    git stash pop stash@{n}
    ```

* 清除所有的stash条目

    ```bash
    git stash clear
    ```

* 查看stash的具体内容

    ```bash
    git show stash
    git show stash@{n}
    ```






### 更新项目

### 检查和比较