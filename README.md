本项目由 [wsq127](https://blog.wsq127.top)/[zMr](https://blog.517group.cn) 开发qwq。

游戏名暂定为《MiniLinux:prologue》

logo:![logo](/img/logo.png)

如果有大佬们看见并且有意见可以去B站私信我们或者直接PR.

PR 的话可以不用在意码风，最后会用 VScode 格式化的。

暂定规则：
    游戏机制: 
        当你的五个文件全部被删除，视为你被淘汰。
        当你有一个文件处于别人的目录下时，你才能操作这个目录上的文件。
        当仅剩一个玩家存活时，这个玩家获胜。
    游戏流程: 
        准备阶段：每人拿四张牌，将每人的五个文件放至玩家的根目录。
        从 1 号玩家轮流: 
            摸牌阶段: 摸 4 张牌。
            出牌阶段: 可以出任意张牌
                cd: 跳转到当前文件目录下任意文件夹内
                mkdir: 在当前目录创建一个文件夹
                mv: 将任意一个文件移动到当前目录
                rm: 删除当前目录下的一个文件
                echo: 重新新建你被删除的文件
                sudo: 使用 sudo rm 删除的文件不能被 echo 回来，使用 sudo 可抵消非 sudo 命令
            弃牌阶段: 手中只保留 你的文件个数 张牌。
