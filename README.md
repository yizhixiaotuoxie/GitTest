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
>>
