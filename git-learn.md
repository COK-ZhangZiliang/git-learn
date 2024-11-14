
# git-learn
## 工作区域和文件状态
![](images/1.png)

## 添加和提交文件
```bash
git status
git add *.txt # 添加所有txt文件到暂存区
git add . # 添加当前文件夹下所有文件到暂存区
git commit -m "..."
git log [--oneline] # 查看提交信息
git reflog # 查看所有操作记录
```

## git reset
![](images/2.png)

# git diff
```bash
git diff # 比较工作区和暂存区
git diff HEAD # 比较工作区和版本库
git diff --cached # 比较暂存区和版本库
git diff $ID1/HEAD~i $ID2/HEAD [$FILE]# 比较两次版本提交（可只比较具体文件）
git diff $BRANCH1 $BRANCH2 # 比较两个分支
```