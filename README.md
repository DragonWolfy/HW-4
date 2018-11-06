# HW-4
n=list(input('Input name: '))
a=len(n)
if a < 4:
    print('>Name too short')
elif a > 4:
    print('>Name too long')
else:
    n.reverse()
    w=[]
    q=[]
    for i in n:
        for j in range(a):
            q.insert(j,i)
        w.extend([q])
        q=[]
    for s in range(a):
        for b in range(a):
            print(w[s][b], end='')
        print()
m=[]
for i in range(a):
    m.extend(w[i])
u=10
while u < len(m):
    print(m[u])
    u+=1
