# Word-Order-HackerRank-Solution
Hackerrank solution python WordOrder | word order solution hacker rank | hacker rank solution | python code for word order

````python

import collections

n = int(input())
st = []
for i in range(n):
    s = input()
    st.append(s)
sh = collections.Counter(st)
u = {}
c = []
count = 0
for i in st:
    u[i] = sh[i]
for x,y in u.items():
    count += 1
    c.append(y)
print(count)
print(*c)

