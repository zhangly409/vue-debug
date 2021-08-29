# 搭建 Vue 源码调试环境步骤

- npm install
- npm run setup
- 修改 \build\config.js 文件中的 function genConfig (name) {}内部的配置对象const config = {xxx}，在其中加入sourceMap: true 字段
- npm run dev 启动调试环境
- 打开 /example/demo/index.html 文件，修改其中 script[src]对 vue 的引用，修改其文件名为：vue.min.js->vue.js，然后在浏览器中直接打开该 html,进行调试。
