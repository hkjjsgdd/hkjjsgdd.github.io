1： 下载Node.js
http://nodejs.org/download/
2： 下载并安装git
https://git-scm.com/download/win
3：  去GitHub官网申请一个账号
Github官网：https://github.com/

！【你想输入的替代文字】（用Node,github和hexo搭建的个人博客/www.jpg）

配置ssh
1：https://blog.csdn.net/qq_42351033/article/details/99182662（链接里面博主里讲的很清楚）  切记不要整条复制，把网址复制下来就可以

搭建hexo
1：先创建一个文件夹用来装blog里的东西，再windows+s 打开命令提示符，
    输入以下命令：cd desktop   
                            cd 你这个文件夹的名字
2：再安装hexo
   npm install hexo -g

3：初始化
   在建的文件夹里右键，点git bash    在git bash 里面输入 hexo init

4：生成网站
    在git bash 里输入  hexo generate或者hexo g
    最后右击你的文件夹，选择git bash 
    输入 hexo s命令 会出现一个网站 复制粘贴打开就是一个博客了
 （此网站只可以自己看得到}

5：在GitHub网站上建立仓库
     名称必须是your_name.github.io   我的为：hkjjsgdd.github.io
     记得勾选“使用自述文件初始化此存储库”（initialize this repository with a README）  仓库英文名称（Repository ）
6：配置文件
     找到自己保存blog文件的文件夹下的  _config.yml，双击打开
     deploy:
     type: git
     repository: https://github.com/xxx/xxx.github.io.git
     branch: master     （将此处修改为以上的，注意xxx为你的用户名）
     最后在cmd中输入
      git config --global user.name "yourname"
      git config --global user.email "youremail"

终端cd到blog文件夹下执行生成静态页面命令：

        hexo g

此时若出现如下报错：

ERROR Local hexo not found in ~/blog
ERROR Try runing: 'npm install hexo --save'

尝试执行命令：

npm install hexo --save

（若无报错，自行忽略此步骤）

然后在当前目录下，终端输入：

hexo d

如果执行命令hexo d仍然报错：无法连接 git 或找不到 git，则执行如下命令来安装hexo-deployer-git：

npm install hexo-deployer-git --save

完成安装之后，再次执行hexo g和hexo d命令。

随后按照提示，分别输入自己的 GitHub 用户名和密码，开始上传。

完成上传之后，通过http://xxx.github.io/ (xxx换成您自己的仓库名，也就是用户名)来访问自己刚刚上传的网站。

7：新建一篇文章
    hexo new"hkjjsgdd"
   hexo g -d 即可


8：查找并下载你喜欢的博客主题
    https://hexo.io/themes/  下载的博客主题添加进保存blog文件的themes文件里，每一个主题都有自己的名字需要把该主题文件夹的名字命名为改主题的名字
    在git bash 上输入hexo clean ,再输入hexo g -d 即可修改主题




！！！！！！！！以上操作基于github上 阿里云的还在摸索 













