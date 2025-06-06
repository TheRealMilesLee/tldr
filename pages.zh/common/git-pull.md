# git pull

> 从远程仓库获取分支，并将其合并到本地仓库。
> 更多信息：<https://git-scm.com/docs/git-pull>.

- 从默认的远程仓库拉取代码并执行合并：

`git pull`

- 从默认的远程仓库拉取代码并采用变基策略实现合并（将你的本地提交“移植”到远程获取的分支上）：

`git pull {{[-r|--rebase]}}`

- 从给定的远程仓库和分支中拉取代码，并合并到本地对应分支：

`git pull {{远程仓库名}} {{分支名}}`
