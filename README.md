# sudip-demo
This is my first git.
<br>
Author-Trisha




#Write a Python Program to check whether a year is leap year or not.

year=int(input("Enter a year:"))

if((year%4==0 and year%100!=0) or (year%400==0)):

    print("The ",year,"is a leap year")

else:

    print("The",year,"is not a leap year")





'''

Write a program to input Percentage.Calculate percentage and grade according to the following conditions:

Percentage>=90%: Grade A

Percentage>=80%: Grade B

Percentage>=70%: Grade C

Percentage>=60%: Grade D

Percentage>=40%: Grade E

Percentage<40%: Grade F

'''

Percentage=int(input("Enter the Percentage:"))

if(Percentage>90 or Percentage==90):

    print("Grade A")

elif(Percentage>80 or Percentage==80):

    print("Grade B")

elif(Percentage>70 or Percentage==70):

    print("Grade C")

elif(Percentage>60 or Percentage==60):

    print("Grade D")

elif(Percentage>40 or Percentage==40):

    print("Grade E")

else:

    print("Grade F")



'''

Write a Python Program to determine whether a 3-digit number is Armstrong or not.

'''

num=int(input("Enter a number:"))

sum=0

n=num

while(n>0):

    r=n%10

    sum=sum+(r**3)

    n=n//10

if(sum==num):

    print("It is an Armstrong number")

else:

    print("It is not an Armstrong number")



#Write a Python Program to calculate the sum of digits of a given N -digit number.

n=int(input("Enter a number:"))

sum=0

while(n>0):

    r=n%10

    sum=sum+r

    n=n//10

print("The sum of the digits is:",sum)



#Write a Python Program to check whether a number is palindrome or not

def palindrome(num):

    sum=0

    n=num

    while(n>0):

        r=n%10

        sum=(sum*10)+r

        n=n//10

    if(sum==num):

        print("It is a palindrome number")

    else:

        print("It is not a palindrome number")

no=int(input("Enter a number: "))

palindrome(no)

    

'''Write a Python Program to calculate the following :1+3+5+7+.....+ upto n terms

Take the numbder of terms as user input.

'''

n=int(input("Enter the no. of terms:"))

sum=0

num=1

for i in range(0,n):

        sum=sum+num

        num+=2

print("The value is:",sum)



#Write a Python function that takes a number as input and checks if it is a prime number

def prime(num):

    count=0

    for i in range(1,num+1):

        if(num%i==0):

            count+=1

    if(count==2):

        return True

    else:

        return False

n=int(input("Enter a number:"))

if(prime(n)==True):

    print("It is a prime number")

else:

    print("It is not a prime number")





#Write a Python programk that takes the input string from the user and calculate the no. of vowels.

str=input("Enter the string:")

count=0

for i in str:

    if(i=='a' or i=='e' or i=='i' or i=='o' or i=='u' or i=='A' or i=='E' or i=='I' or i=='O' or i=='U'):

        count+=1

print("The total no. of vowels in the string:",count)



#Define a function that takes the list of integers as input and returns the sum of all even numbers in the list

def sum_even(n):

    l=[]

    for i in range(0,n):

        num=int(input("Enter the number:"))

        l.append(num)

    print("The list is:",l)

    sum=0

    for i in range(0,n):

        if(l[i]%2==0):

            sum=sum+l[i]

    print("The sum of all the even numbers in the list:",sum)

n=int(input("Enter the no. of elements in the list:"))

sum_even(n)

            

'''Write a Python Program that takes a set of integers as input and returns a new set that contains only the even numbers from the original set

'''

n=int(input("Enter the no. of elements in the set:"))

s1=set()

for i in range(0,n):

    num=int(input("Enter the element:"))

    s1.add(num)

print("The original set is:",s1)

l=list(s1)

l1=[]

for i in range(0,n):

    if(l[i]%2==0):

        l1.append(l[i])

s2=set(l1)

print("The set of only even numbers is:",s2)





'''

Write a Program in Python that takes a dictionary as input and returns a new dictionary that contains only the key-value

pairs where the key is an odd number.'''

d1={1:"a",2:"e",3:"i",4:"o",5:"u"}

print("The original dictionary is:",d1)

d2={}

for key in d1:

    if(key%2!=0):

        d2[key]=d1[key]

print(d2)

        

#Write a Program in Python to calculate the Hcf of two numbers using recursive function

def HCF(a,b):

    if(b==0):

        return a

    else:

        return HCF(b,a%b)

x=int(input("Enter the 1st number:"))

y=int(input("Enter the 2nd number:"))

result=HCF(x,y)

print("The HCF value is:",result)





#Write a Python Program to find the factorial of a given number using recursion

def fibo(n):

    if(n<=0):

        return False

    elif(n==1):

        return 0

    elif (n==2):

        return 1

    else:

        return fibo(n-1)+fibo(n-2)

n=int(input("Enter ther no. of terms:"))

print("The fibonacci series is:")

for i in range(0,n):

    print(fibo(i))

    



    

