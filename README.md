# peng-ui-2
peng-ui是一个基于vue3写的UI组件库，技术栈是vue3 + vite + TS（部分用到）。
目前只实现了几个常见的UI组件，例如Switch 切换组，Button按钮组件，Dialog对话框弹窗组件，Tabs切换组件，并设计了项目的官网介绍页以及文档介绍页，下面请看详细介绍。
#官网页面
##1.官网整体采用清新风格，简洁大气。
![image](https://user-images.githubusercontent.com/100587019/230044198-ccbb2d09-2616-44dc-bf1c-b97ce4054e66.png)
##2.响应式布局，适配移动端
为了优化用户体验，官网做了响应式布局，页面会根据用户浏览窗口的尺寸自动重新计算元素的排列
![image](https://user-images.githubusercontent.com/100587019/230044797-dfd886b8-b8c8-495d-bc58-4f7d165e68a5.png)
![image](https://user-images.githubusercontent.com/100587019/230044894-7a93d500-92f8-47cf-85b5-7bf0eb0387e7.png)
#文档页面
![image](https://user-images.githubusercontent.com/100587019/230045113-732468a8-80f3-40df-b4d1-ed922996dfdd.png)
#组件介绍
##1.Switch组件
switch是开关的意思，该组件主打的是一个开关的功能，并且配备了一个禁止点击的开关按钮，用于特定的业务场景
![image](https://user-images.githubusercontent.com/100587019/230045899-ac29e3a6-3bb1-40a5-ab50-2b7b805f79d9.png)

##2.Button组件
Button组件相对比较多元，设计了不同大小，不同类型（按钮、超链接、文本）、不同标识作用等按钮
![image](https://user-images.githubusercontent.com/100587019/230046385-a4bb4f2e-9493-4799-8fad-2a26be7c07ad.png)
![image](https://user-images.githubusercontent.com/100587019/230046413-3c3c99e2-9bf3-4757-873b-5205951285b6.png)

#Dialog弹窗组件
弹窗组件可以支持用户自定义标题、内容、并获取用户点击【确定】、【取消】两个按钮的布尔值
![image](https://user-images.githubusercontent.com/100587019/230046948-3ef01c3a-c150-4521-92c6-d3da633e2ca3.png)
![image](https://user-images.githubusercontent.com/100587019/230046977-bdaff0c2-7edc-44f0-a401-b20db1973b6c.png)
#Tabs切换组件
点击导航栏上的不同按钮，可以切换不同的内容，为了优化视觉体验，特意添加了一条随点击位置飘动的下划线，该线还可以自动匹配导航栏内容的长度
![image](https://user-images.githubusercontent.com/100587019/230047187-b1fcd5ef-06ed-4dc6-af9a-98cffad127c5.png)
