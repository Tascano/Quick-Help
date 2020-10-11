# Quick-Help
quick codes for frequent needs


# Take a string of integers and break to list of integers 
//numbers = str
//string = list

string = list(map(int, numbers.split()))

or

nums = sorted(numbers.split(), key=int)


# hackerrank maintain dictionary of values based on two array, taking one array as the key

a = [2,0,1,2] #bidid
b = [8,7,6,9] #bidcost
c = set(a)    

dis = {}
l = list
for i in range(len(a)):
    if a[i] in c:
      if b[i]<b[i-1]:
        dis[a[i]] = b[i]

print(dis)
sum = 0
for i in dis.keys():
  sum = sum+dis[i]
print(sum)
