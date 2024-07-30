# first-5-prime-numbers
#input:n=5
#output:2 5 11 17 23
n=int(input())
c,i,rc=0,2,0
while True:
  flag=True
  for j in range(2,i//2+1):
    if i%j==0:
      flag=False
      break
  if flag:
      c+=1
      if c%2!=0:
        rc+=1
        print(i,end=' ')
        if rc==n:
          break
  i+=1
