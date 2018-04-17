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
