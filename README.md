# 学习使用vue-cli

## 使用vue-cli 能快速搭建一个项目的基础结构  

踩坑纪实：因为使用了ESLint代码风格及错误查找工具 在运行npm run dev指令时报错  
导致http://localhost:8080/#/ 本地服务器打不开 
查询后原因为在App.vue 文件中添加了一个换行导致报错no-multiple-empty-lines

即受ESLint代码风格控制，文件内不允许有多余的空格出现-_-||


# 继续学习vue-router

## 使用vue-router 是搭建一个单页应用的关键

1.新建路由步骤：（1）.src=>components文件夹下新建xx.vue文件;  
              （2）.src=>router文件夹下index.js文件内进行修改，新增import xx form '@/components/xx'路径引入;  
              （3）.src=>router文件夹下index.js文件内进行修改，routes数组内新增路由对象，格式为下：  
              {  
                path: '/Hi',  
                name: 'Hi',  
                component: Hi  
              }  
2.新建子路由步骤:（1）.src=>components文件夹下新建xx.vue文件;    
               （2）.src=>router文件夹下index.js文件内进行修改，新增import xx form '@/components/xx/xx'路径引入;   
               （3）.src=>router文件夹下index.js文件内进行修改，routes数组内父级页面对象内新增children数组：  
               （4）.src=>components文件夹下父页面内新增<router-view/>标签;  
####  踩坑纪实：在(2)步引入时注意从属关系路径"import xx form '@/components/xx/xx1'",xx为父级页面，xx1为子路由
               
                 
          
