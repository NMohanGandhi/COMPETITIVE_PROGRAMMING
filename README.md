# Competitive_programs
** Given a number N followed by N numbers(negative or positive) print the maximum sum of any subarray of the array.**
Input Size : 1 <= N <= 100000

**INPUT**
7
1 2 3 4 5 6 7
**OUTPUT**
28

```python

N=int(input())
numbers = list(map(int,input().split()))[:N]
positive_num = []
negative_num=[]
for i in numbers:
    #print(i)
    if i>0:
        positive_num.append(i)
        #print(total)
    else:
        negative_num.append(i)
result = sum(positive_num)
if len(positive_num)==len(numbers):
    print(result)
else:
    print(result+negative_num[0])
```
