# Basic
basic python

#6組樂透好嗎
import random
again = 1
while again ==1:
    for i in range(1,7):
        lottonum = random.randint(1,49)
        print("%3d"%(lottonum), end = " ")
    print()
    again = eval(input("continue:1 or quit:0 ---->"))
    
#sum between a and b that %4==0 or %9==0
a = int(input())
b = int(input())
count = total_sum = 0
time = 10
for i in range(a,b+1):
    if i%4==0 or i%9==0:
        print("%-4d"%(i), end = " ")
        total_sum += i
        count += i
        if count % time == 0:
            print()
print("\n%d"%(count)) #bug
print(total_sum)
