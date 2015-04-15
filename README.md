# JSMarkdownEdit
JSMarkdownEdit

## JSMarkdownEdit 

+ 整合markdown.css marked.js editor.js  支持requirejs 方式调用
+ markdown.css 前台显示css用 .markdown-body 包裹markdown HTML
+ marked.js markdown js 解析器  nodejs 使用marked 模块解析 npm install marked --save
+ editor.js html页面编辑器


## require.js 调用  

+ 请先配置好requirejs path 路径
+ 
  ```
      require(['markdown'], function (tip,markdown) {
      
          var K = new markdown({
          
                  element: document.getElementById('post'),
                  
               });
               
          var html = K.value(); // 获取markdown html 
          
      })       
  ```     

+ nodeJS 解析markdown 

+ ```
     var marked = require('marked'); 
     
     var html = marked('# markdown');
     
     ```
     



