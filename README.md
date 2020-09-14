# Hackerrank-solution
# my solutions of hackerrank problems in python
# Electronic shop solution


def electricshop(k,u,b):
    maxi=-1
    for i in range(len(k)):
        for j in range(len(u)):
            if((k[i]+u[j])<=b  and (k[i]+u[j])>maxi):
                maxi=k[i]+u[j]
    return maxi
b,n1,n2=list(map(int,input().rstrip().split()))
k=list(map(int,input().rstrip().split()))[:n1]
u=list(map(int,input().rstrip().split()))[:n2]
print(electricshop(k,u,b))

