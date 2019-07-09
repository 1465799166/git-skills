- 关联远程库 `git remote add origin xxxx`
- 创建并切换分支 `git checkout -b xxx`
- 关联远程分支 `git branch --set-upstream-to origin/xxx`
- 变基 `git rebase xxx` 以xxx为标准
- 修改head指向 `git checkout HEAD~xxx`
- add dev mark
- 撤回本地操作
```
git reset --soft xxx // 撤回到指定版本，保留本地代码
git reset --hard xxx // 撤回到指定版本，不保留本地代码
```
- 撤回远程提交 `git revert HEAD xxx`
- 查看分支树 `git log --graph --all`
- 删除分支 `git branch -d xxxx`

- 合并本地某个分支多个commit 
``` bash
git rebase -i HEAD~3 // 选择最近的3个commit进行合并选择，会合并到最近的第三个
```
