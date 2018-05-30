# 常用git指令
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












- 从远程仓库现在代码   
```js
    git clone git@github.com:abiaoLHB/aboutGit.git
```

- 