**USE OF HIGHER ORDER FUNCTIONS**
numbers = "2,4,6,8,10"
Your task:
1. Convert the string into individual numbers.
   
n = "2,4,5,6"  
r = n.split(",")  
d = list(map(int,r))  
print(type(d))

3. Use map() and lambda to double every number.
n = "2,3,5,6"
r = n.split(",")
d = list(map(int,r))
db = lambda x: x*2
result = list(map(db,d))
print(result)


4. Convert the result back into a comma-separated string.
n = [2,3,4,5]
r = list(map(str,n))  
d = ",".join(r)  
print(type(d))


2.>Question:
Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5,between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line.

l = []  
for i in range(2000,3200):  
    if i%7==0 and i%5!=0:  
        l.append(str(i))   
print(",".join((l)))   


# list only of odd nos
list = []  
for i in range(1,11):  
    if i%2 != 0:  
        list.append((i))  
print(list)             

**LIST COMPRESHION**
list = []   
numbers = [i for i in range(1,11) if i%2 != 0]  
print(numbers) 


list only of odd nos
list = []
for i in range(1,11):
    if i%2 != 0:
        list.append((i*i))
print(list)        


list = []
numbers = [i*i for i in range(1,11) if i%2 != 0]
print(numbers) 
