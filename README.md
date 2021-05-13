# rev-of-mid
n=int(input())
temp=n
rev=0
c=0
while n:
    r=n%10
    n=n//10
    c+=1
n=temp
c=c-1
m=(n//10)%pow(10,c-1)
f=n//pow(10,c)
r=n%10
while m:
    mi=m%10
    m=m//10
    rev=rev*10+mi
nn=(rev*10+r)+(f*pow(10,c))
print(nn)
