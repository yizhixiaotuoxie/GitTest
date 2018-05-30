## 测试熟悉git
####  [博客链接](http://git.oschina.net/progit/2-Git-%E5%9F%BA%E7%A1%80.html)
>>设置git用户名邮箱
 ```
     //设置本目录下使用的标记名
     git config user.name "tuoxie"
     git config user.email yizhixiaotuoxie@163.com

    //加上global 就是全局的变量 --所有项目公用 但是优先读取本目录设置的
    git config --global user.name "renb"
    
    可以使用 git config --list 检验，同名出现在后面的是最终的
    或者 git config user.name
 ```
>> 分支管理
>>>git  branch  dev-ccc 创建分支 (git branch 查看有哪些分支  git branch --merge 查看已经合并的分支)
>>>git checkout 选择到分支，
>>>然后就是合并分支，checkout 到要合并到的分支 
>>>如将分支 dep-111 合并到 master checkout到master; 然后git merge 选择需要合并的分支 dep-111 
>>>Git cherry-Pick 指定某几个提交合并到本分支，，如在develop中有多个提交版本 a b c，现在只需要 b 提交，在master分支 选中 b 提交的提交号 806db86 右键 Cherry-Pick 

### 问题
>> 合并分支报错:
>>>* Git Merge Failed
           		Your local changes would be overwritten by merge.
           		Commit, stash or revert them to proceed. 
           	√√	运行git stash (idea-->stash change) 清理本地未commit 的文件用远程的覆盖
>>>* Git Merge Failed
    		Your local changes would be overwritten by merge.
    		Commit, stash or revert them to proceed
    		√√ 合并后pull 报这个错 ；直接再commit 一下本地变化就好--好像也可以 stash一下 或者add一下(add 表示已经解决冲突)
   
 