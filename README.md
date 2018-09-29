# git-demo
git  test demo

add one line

#### 查看 Git 配置信息

`git config --list`

#### 查看详细日志状态

`git log --stat`

#### 修改 commit 信息

`git commit --amend "message2"`

#### 标签的使用

`git tag -a v1.0 -m "my version 1.0"`

#### 查看标签

`git show v1.0`

#### 分支的分类

> release:  用于发布生产环境
>
> master:  用于测试环境
>
> feature:  特性分支,开发环境
>
> hotfix-*: 用于紧急修复线上 bug，修复合回 release 和 master，临时分支，用完将删除

#### 合并分支的来源

在合并的时候使用 `git merge` , 在主分支上不知道提交的来源，一般在合并是增加参数`--no-ff`  ,

建议使用 `git merge --no-ff `

#### 撤回修改

撤回暂存区修改的内容

`git checkout 文件名`

将添加暂存区的内容移除到工作区

`git reset HEAD 文件名`

#### 查看文件位置的修改

`git blame 文件名`

#### git rebase 使用

```
#current  topic
          A---B---C topic
         /
    D---E---F---G master
```

执行命令

```
git rebase master 或者 git rebase master topic
```
