# hm0914solutions
# 1.
# On the market, an old lady sells geese, each for 1860 HUF, which costs 260 HUF more than a hen.
# Yesterday she sold 6 hens and 11 geese. How much did she earn?
t=1860*11+(1860-260)*6
print(t)
# 2.
# 7 scarves cost 6860 HUF. How much does 140 scarves cost? How many scarves can I buy with 15 000 HUF?
t=6860*140
u=15000/6860
print (t,u)
# 3.
# John and James will be twice as old as now in 4 and 8 years, respectively. How old are they?
john=4
james=8
print("john: ", john)
print("james: ", james)
# 4.
# Write a program that prints the next 20 leap years.
for i in range(2018, 2039):
    print(i)
# 5.
# Write a program that asks the user for a number n and prints the sum of the numbers 1 to n.
number=int(input("enter number: "))
for sum in range(1, number+1):
    print(sum)
# 6.
# Write a program which merges two sorted lists into a new sorted list.
L1=['tom', 'jerry']
L2=['cat','mouse']
L2.append(L1)
print(L2)

# 7.
# Write a function that takes a number and returns a list of its digits.
# So for 8500 it should return [8, 5, 0, 0].
number=int(input("enter 4 digit number: "))
a=number/1000
b=(number-a*1000)/100
c=(number-a*1000-b*100)/10
d=(number-a*1000-b*100-c*10)
#a1=floor(a) i tried floor function to get first digit of decimal a, but it didnt work
print(a,b,c,d)


# 8.
# Write a function that combines two lists by alternatingly taking elements.
# e.g. [a,b,c], [1,2,3] → [a,1,b,2,c,3].
# i have googled this question a bit.
list1= [23,11,70]
list2= [1,2,3]
list3 = []
while True:
    try:
        list3.append(list1.pop(0))
        list3.append(list2.pop(0))
    except IndexError:
        break
print(list3)
