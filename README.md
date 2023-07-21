# python-9-
python学习笔记(9)
# p32 分支结构_多分支结构
#语法结构:
if 条件表达式1:
elif条件表达式2:
elif条件表达式N:
[else:]

score=int(input('请输入一个成绩:'))
#判断
if score>=90 and score<=100:  # 可以写成if 90<=score<=100:  python是支持这样写的
    print('A级')
elif score>=80 and score<=89:
    print('B级')
#以下同理
#...
else:
    print('对不起，成绩有误，不在成绩的有效范围内')



# p33 分支结构_嵌套if的使用
#语法结构
if条件表达式1:
    if内层条件表达式：
      内层条件执行体1
    else:
        内存条件执行体2
else:
    条件执行体

answer=input('您是会员吗?y/n')
money=float(input('请输入您的购物金额:'))
#外层判断是否为会员
if answer=='y': #会员
    if money>=200:
        print('付款金额为:',money*0.8)
    elif money>=100:
        print('付款金额为:'money*0.9)
        else:
            print('不打折')
else:  #非会员
    if money>=200:
        print('打9.5折，付款金额为:'money*0.95)
    else:
        print('不打折，付款金额为:'money)



# p34 条件表达式
#正常写法
    num_a=int(input(‘请输入第一个整数’))
    num_b=int(input('请输入第二个整数'))
    #比较大小
    if num_a>=num_b:
        print(num_a,'大于等于'，num_b)
    else:
        print(num_a,'小于等于',num_b)

print('使用条件表达式进行比较')
print(   str(num_a)+'大于等于'+str(num_b)   if num_a>=num_b    else   str(num_a)+'小于'+str(num_b)   )
# if条件判断语句为True则执行左侧的代码，为False则执行右侧的代码
