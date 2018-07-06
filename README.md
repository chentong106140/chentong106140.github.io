npm install hexo-cli -g   

hexo init #保证当前目录没有任何内容

npm install   


npm install hexo-deployer-git --save  #安装这个才能部署到github


hexo clean
hexo generate
hexo server

编译并立即部署到git
hexo g -d