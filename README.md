# python-
This repository is usedd to store documents.
### 💌

1. **git 操作**

    ```bash
    配置
    $ git config --global user.name "用户名"  
    $ git config --global user.email "用户邮箱"

    生成令牌，钥匙
    $ cd ~/.ssh
    $ mkdir key_backup
    $ ssh-keygen -t rsa -C "用户邮箱"
    $ ssh -T git@github.com （测试链接状态）

    创建本地仓库
    $ git init
    $ git clone https://github.com/用户名/仓库名.git

    常用命令
    $git add . //添加文件
    $ git commit -m "commit-messages" //提交本地仓库
    $ git push origin master //提交远程仓库
    $ git pull //拉取远程文件，与以下命令类似
    $ git branch temp //创建本地分支
    $ git fetch origin master:temp #更新远程代码到本地仓库
    $ git merge master #合并分支
    添加文件
    $ git init
    $ git clone https://github.com/name/repository.git
    $ git add 文件名.md                  #如果想一次全部添加则：git add -A
    $ git commit -m '添加了name文件'    #提交并添加操作说明
    $ git push origin master

    删除文件夹
    $ git init
    $ git clone https://github.com/name/repository.git
    $ git pull origin master        #将远程仓库里面的项目拉下来
    $ git dir                       #查看有哪些文件夹
    $ git rm -r --cached target     #删除target文件夹
    $ git commit -m '删除了target文件夹'    #提交并添加操作说明

    上传超过100M的文件到github
    $ git lfs install   #在本地仓库下安装lfs
                        #添加了大文件后...
    $ git lfs track "文件名.后缀名"  #正确会显示提示：'Tracking "文件名.后缀名"'
    $ git add .
    $ git commit -m "提交信息"
    $ git push -u origin master


1. **markdown 学习**

        1.标题(#有几个就是几级标题)
    # 一级标题
    ## 二级标题
    ## 三级标题
    #### 四级标题
    ##### 五级标题
    ###### 六级标题
    > PS:标题最多可以分六级
    

        2.列表
+ 一级列表

    + 二级列表

        + 三级列表
+ 二级列表
    >PS:加号可以制作列表，没有级数限制，但是三级以后表述符号相同,列表还分为有序列表和无序列表

        3.字体
    
    *斜体*（粗体表示）

    **粗体**（斜体表示）
    
    ***粗斜体***（粗斜体表示）

    ~~删除线~~


    ~~**粗体**~~


    分割线:
+ 第一种
		```
		---
		```
+ 第二种
        ```
        ***
        ```

        4.表格

    # 例如

    |表格1|表格2|表格3|表格4|
    |:------|:-----|:-----|:-----|
    |内容|内容|内容 |内容|
    > 用直竖线、冒号、减号制表冒号代表内容填充方式例如居中靠左等

        5.超链接(文件类型和网址类型)

    [点我前往网页](https://www.baidu.com/)


    [点我打开文件](1572225922088.png)

    <img src="psb9UKAU3PW.webp" width="400">


    > 超链接设置方式为[]()中括号里面是描述，小括号里面是网址或者文件地址，第三种是图片插入方式(html用法)

        6.代码块

    ```python
        def f(n,x):
        a=[0,1,2,3,4,5,6,7,8,9]
        b=[]
    
        while True:
            s=n//x
            y=n%x
            b=b+[y]
           if s==0:
               break
            n=s
        b.reverse()
        for i in b:
           print(a[i],end='')

        S = input(" ")
        L = S.split(',')
        f(int(L[0]),int(L[1]))
    ```
    >代码插入方式```开始，```结尾，在第一个```后注明语言类型即可标注语言关键词

        7.引用

    > 一级引用
    >> 二级引用
    >>> 三级引用
    >>>>>   while True:
                s=n//x
                y=n%x
                b=b+[y]
                if s==0:
                break
    :(代码块引用 

        8.其他

    行末空两格加回车直接跳到下一行与上一行行首同位置处




1. **假期任务，做一个 Pygame 小游戏，或者 PyQt5 的小程序**

    + *要求：* 提交到 GitHub 新建的一个仓库下面，链接在发给我，我要求会看！
