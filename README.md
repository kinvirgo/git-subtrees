# git-subtrees

使用 git subtree 管理共享多项目使用

# 1、subtree 帮助

```sh
git subtree -h
```

# 2、添加子项目

```sh
# git subtree add --prefix=<子项目目录> <代码源> <分支>

# 添加命令
git subtree add --prefix=subtree/git-subtree-module-1 https://github.com/kinvirgo/git-subtree-module-1.git main

# 添加--squash合并提交日志，不推荐
git subtree add --prefix=subtree/git-subtree-module-1 https://github.com/kinvirgo/git-subtree-module-1.git main --squash
```

# 注意

-   `Working tree has modifications. Cannot add.`需要当前项目没有修改状态的文件
-   不建议使用`--squash`;如果添加使用了`--squash`参数,防止出现问题。之后
    的`git subtree add`、`git subtree megre`、`git subtree pull`都尽量带上

