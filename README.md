# how-to-push-windows
    本人是刚开始学习github的小白，因为网上经常有人好为人师，浪费别人时间，所以我想大家小白共享一下，哪里有不对欢迎指正。
    我用的github本地客户端是msysGit。
    前提：本地和github线上建立连接（你有本地的sshkey）
    1.在github上新建一个repository，如果你有想要上传的仓库就不用了，这个仓库（文件夹）是存储你要上传的内容的，
    我假设名字为name。
    2.打开你的客户端（我的是mysGit），cd到你要上传的那个文件或文件夹。
    3.git init
    4.git add .            (add和.有空格)
    5.git commit -m "这里填对这次commitde信息"
    6.touch README.md
    7.git add README.md
    8.git status
    9.git remote add origin git@github.com:1995benWeal/name (1995benWeal是我的账号)
              （如果出现fatal: remote origin already exists.输入：
                git remote rm origin再重复9操作）
    10.git push -u origin master
            （第二次好像直接可以用git push）
###遇到的问题
        git add . git push -u origin master 然后就提示：Branch master set up to track remote branch master，
        ssh -T git@github.com提示PTY allocation request failed on channel 0
        找不到解决方案。
    

