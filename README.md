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

- 和远程仓库解除关联

  ```js
  git remote remove origin
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

- 从SSH切换到HTTP  

  ```js
  1、方法一：修改命令：git remote set-url origin [url]    （注释：后面的url不要带[]）
  2.先删后加
  	git remote rm origin
  	git remote add origin [url]
  3.直接修改config文件
  ```


- 往远程非master分支推送代码

```js
git push origin  远程分支名字
```

- 把某个分支上的内容都拉取到本地 

  ```js
  git pull origin <branchName>(远程分支名称)
  ```

- 删除远程分支

  ```js
  git push origin --delete <branchName>
  ```

- 删除本地分支

  ```js
  git branch -d <branchName>
  ```

- 在本地创建分支dev并切换到该分支 

  ```js
  git checkout -b dev(本地分支名称) origin/dev(远程分支名称)
  ```

  