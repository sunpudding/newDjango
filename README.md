# newDjango
django

1.可注册新用户，须提供用户名、密码。http://127.0.0.1:8000/register

2.已注册用户可登录、注销、修改密码。http://127.0.0.1:8000/login 注销做的是清除session http://127.0.0.1:8000/changepwd/

3.已登录用户可留言，可以查看自己的所有留言。 http://127.0.0.1:8000/login

4.首页须翻页显示所有留言（每页最多20条），每一条留言须包括留言者、时间以及内容。http://127.0.0.1:8000

5.提供接口 "/latest_msg"，返回最近 10 分钟的所有留言，须使用 json 格式， 每一条留言包含 4 个字段，如下： user（留言者）, timestamp（留言时间）, title(留言标题)，content（留言内容）http://127.0.0.1:8000/latest_msg/


在test-django文件夹下
通过selenium对django的接口进行测试 ，在MessageB中包含各个接口的测试文件
运行run_all_case可以对MessageB中的各个文件进行总的运行，在report文件中生成我的自动化测试报告