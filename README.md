# 18417-2
质因数



将一个正整数分解质因数。例如：输入90,打印出90=2*3*3*5。



n=int(input())
l=[]

while n!=1:
    for i in range(2,n+1):
        if n%i==0:
            l.append(i)
            n=int(n/i)
            break

print('the num can be made for',l)



一个数如果恰好等于它的因子之和，这个数就称为"完数"。例如6=1＋2＋3.编程找出1000以内的所有完数。

for x in range(1,1001):
    l=[]
    a=0
    for y in range(1,x):
        if x%y==0:
            a+=y
            l.append(y)
    if x==a:
        print(x)
        print(l)
