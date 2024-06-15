1.
def differenceSum(n):
    n=str(n)
    d=0
    c=0
    for i in range(len(n)):
        if (i%2==0):
            c=c+int(n[i]) 
        else:
            d=d+int(n[i]) 
    return (d-c)

2.
def coinChange(n):
  a=n//4
  b=n%4
  return a+b
 
3.
def productDigits(n):
    k=1
    p=0
    n=str(n)
    for i in range(len(n)):
        if(i%2!=0):
            k=k*int(n[i]) 
        else:
            p=p+int(n[i])
    if(k%p==0):
        return "True"
    else:
        return "False"

4.
def automorphic(n):
    b=n*n
    if(b%10==n):
        return "Automorphic" 
    else:
        return "Not Automorphic"

5.
def checkUgly(n):
    if(n>=2):
        if(n%2==0):
            return "ugly"
        else:
            return "not ugly"
    elif(n>=3):
        if(n%3==0):
            return "ugly"
        else:
            return "not ugly"
    elif(n>=5):
        if(n%5==0):
            return "ugly"
        else:
            return "not ugly"
