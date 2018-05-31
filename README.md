### 常用git指令
- 在本地初始化git仓管
```js
cd 目录
git init
```
- 添加到暂存区     
```js 
    git add test.text (添加某一个指定的文件)
    git add . (全部添加到暂存区)
```

- 查看git状态
```js    
    git status  
```

- 提交到本地仓库
```js
    git commit -m '注释' 
```


- 查看从最近到最远的提交日志
```js
    git log (详细版本)
    git log --pertty=oneline (精简版本)
```

- 查看git管理中的所有提交日志
```js
    git reflog
```

- 回退到上一个版本
```js
    git reset --hard HEAD^
```
- 回到某个指定版本
```js
    git reset --hard 1094a (1094a是日志信息上前面几个字母)
```

- 和远程空仓库建立关联
```js
    git remote add origin git@github.com:abiaoLHB/aboutGit.git

```

- 推送
```js
    git push -u origin master (第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令)

    git push origin master (以后提交)
```








- 从远程仓库现在代码   
```js
    git clone git@github.com:abiaoLHB/aboutGit.git
```

- 