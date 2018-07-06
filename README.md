一：新建github仓库，仓库名就是username.github.io，并且新建READ.md

二：首先复制一个仓库取名为deploy,主要是为了将部署相关代码放到此分支,此时有2个分支，master与deploy

三：使用sourceTree拉取deploy分支

四：创建hexo相关，设置git部署，部署分支为master

五：在deploy分支下执行hexo g -d，编译并且理解部署上传，就好了

六：修改deploy分之下的.gitgnore，添加忽略.idea等配置，最终上传此分支所有代码


npm install hexo-cli -g   

hexo init #保证当前目录没有任何内容

npm install   


npm install hexo-deployer-git --save  #安装这个才能部署到github


hexo clean
hexo generate
hexo server

编译并立即部署到git
hexo g -d