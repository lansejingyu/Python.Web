# Python.Web  
基于Python的Web开发  

使用WSGI处理web:  
1.确保以上两个文件在同一个目录下，然后在命令行输入python server.py来启动WSGI服务器  
2.启动成功后，打开浏览器输入：http://localhost:8000/  就可以看到结果了。  

使用Flask.WEB框架：  
1.我们需要在WSGI接口之上能进一步抽象，让我们专注于用一个函数处理一个URL，至于URL到函数的映射，就交给Web框架来做。  
2.有了Web框架，我们在编写Web应用时，注意力就从WSGI处理函数转移到URL+对应的处理函数，这样，编写Web App就更加简单了。  
3.在编写URL处理函数时，除了配置URL外，从HTTP请求拿到用户数据也是非常重要的。Web框架都提供了自己的API来实现这些功能。Flask通过request.form['name']来获取表单的内容  
