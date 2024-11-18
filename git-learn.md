
# git-learn
## 工作区域和文件状态
![](images/1.png)

## 添加和提交文件
```bash
git status [-s]
git add *.txt # 添加所有txt文件到暂存区
git add . # 添加当前文件夹下所有文件到暂存区
git commit -m "..."
git commit -am "..." # 自动将已追踪的文件的修改添加到暂存区并提交
git log [--oneline] # 查看提交信息
git reflog # 查看所有操作记录
``` 
## git reset
![](images/2.png)

## git diff
```bash
git diff # 比较工作区和暂存区
git diff HEAD # 比较工作区和版本库
git diff --cached # 比较暂存区和版本库
git diff $ID1/HEAD~i $ID2/HEAD [$FILE]# 比较两次版本提交（可只比较具体文件）
git diff $BRANCH1 $BRANCH2 # 比较两个分支
```

## git rm
```bash
git rm $FILE # 从工作区和暂存区删除
 git rm --cached $FILE # 从暂存区中删除，但保留在工作区
```

## .gitignore
![](images/3.png)
```bash
*.a # 忽略所有.a文件
!lib.a # 但追踪lib.a
/TODD # 忽略当前目录下的TODO文件
build/ # 忽略任何目录下的build文件夹
doc/*.txt # 忽略doc/notes.txt，但不忽略doc/server/arch.txt
doc/**/*.txt # 忽略doc/notes.txt和doc/server/arch.txt 
```