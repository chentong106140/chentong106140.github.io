一：新建github仓库，仓库名就是username.github.io，并且新建READ.md

二：首先复制一个仓库取名为deploy,主要是为了将部署相关代码放到此分支,此时有2个分支，master与deploy

三：使用sourceTree拉取deploy分支

四：创建hexo相关，设置git部署，部署分支为master

五：在deploy分支下执行hexo g -d，编译并且理解部署上传，就好了

六：修改deploy分之下的.gitgnore，添加忽略.idea等配置，最终上传此分支所有代码

七：切记：hexo部署代码，不能放在github的master分支下


npm install hexo-cli -g   

hexo init #保证当前目录没有任何内容

npm install   


npm install hexo-deployer-git --save  #安装这个才能部署到github


hexo clean
hexo generate
hexo server

编译并立即部署到git
hexo g -d


安装主题
cd themes && git clone https://github.com/Mrminfive/hexo-theme-skapp.git
修改_config.yml的theme为hexo-theme-skapp

删除node_modules目录
rm -rf node_modules

安装python 下载window版本，安装后，确认python的path是否配置

安装window依赖环境,进入根目录，找到cmd文件，右击选择管理员运行，输入d:切换到当前项目根目录，执行安装如下命令
cnpm install -g windows-build-tools
cnpm install -g node-gyp
cnpm install -g lodash
安装依赖
cnpm install --save hexo-autoprefixer hexo-filter-cleanup hexo-generator-feed hexo-generator-sitemap hexo-renderer-sass hexo-renderer-swig mamboer/lunr.js moment node-sass object-assign
如果报错找不到vendor目录就重装如下：
cnpm rebuild node-sass --save

再进行安装
cnpm install 





