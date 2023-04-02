# git-subtrees

使用 git subtree 管理共享多项目使用

# 1、subtree 帮助

```sh
git subtree -h
```

# 2、添加子项目

```sh
# 添加命令
# git subtree add --prefix=<子项目目录> <代码源> <分支>
git subtree add --prefix=subtree/git-subtree-module-1 https://github.com/kinvirgo/git-subtree-module-1.git main
```
- 注意: `Working tree has modifications.  Cannot add.`需要当前项目没有修改状态的文件
