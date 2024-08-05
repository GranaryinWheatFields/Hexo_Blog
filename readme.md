- 主题：git clone https://github.com/SineObama/hexo-theme-butterfly.git themes/butterfly

- 安装Hexo: npm install -g hexo-cli --registry=https://registry.npmmirror.com

- 编译用的依赖：npm install hexo-renderer-pug hexo-renderer-stylus --registry=https://registry.npmmirror.com

- 发布用的依赖 ：npm install hexo-deployer-git --save --registry=https://registry.npmmirror.com

- hexo s：启动本地服务器，用于预览主题。默认地址： http://localhost:4000/

- hexo d：自动生成网站静态文件，并部署到设定的仓库。部署之后执行 clean

- hexo clean: 清除缓存文件 db.json 和已生成的静态文件 public。