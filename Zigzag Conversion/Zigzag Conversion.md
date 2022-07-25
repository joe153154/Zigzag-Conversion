strs = "PAYPALISHIRING"
numRows = 5
x = numRows-2
d = ""
r1 = []
r2 = []
r3 = []
r4 = []
r5 = []
for i in range(len(strs)):
    m = numRows + x
    n = i % m
    print(n)
    if n == 0:
        a = strs[i]
        r1.append(a)
    elif n == 1 or n == 7:
        a = strs[i]
        r2.append(a)
    elif n == 2 or n == 6:
        a = strs[i]
        r3.append(a)
    elif n == 3 or n == 5:
        a = strs[i]
        r4.append(a)
    elif n == 8:
        a = strs[i]
        r5.append(a)
    r = r1 + r2 + r3 + r4 + r5
for i in range(len(r)):
    d += r[i]

print(d)