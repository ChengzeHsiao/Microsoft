在AD服务器上做操作，将user.csv文件复制到AD服务器目录下

1，user.csv文件用户模板，在文件中添加相应的用户

2，需要修改的内容
参数详解：
OU ---组织单位,例如:研发部门
dc ---域名前缀,例如:test
dc ---域名后缀,例如:com
%d@ --域名全称,例如:test.com

3，在CMD命令行执行的语法：

命令如下：

for /f "tokens=1,2,3,4,5 delims=," %a in (user.csv) do dsadd user "cn=%c,ou=研发部门,dc=test,dc=com" -samid %d -upn %d@test.com -ln %a -fn %b -pwd %e -disabled no
