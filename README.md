# <p align="center"> Python Programming</p>


> Question 1

                Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5,
    between 2000 and 3200 (both included).
                The numbers obtained should be printed in a comma-separated sequence on a single line.

Solution:
              
    l=[]
    for i in range(2000, 3201):
        if (i%7==0) and (i%5!=0):
            l.append(str(i))
    print (','.join(l))

# <p align="center"> -X-X-X- </p>

> Question 2

Write a program which can compute the factorial of a given numbers.

Solution:

    def fact(x):
      if x==1:
        return 1
      return x*fact(x-1)

    y=int(input())
    print(fact(y))
    
# <p align="center"> -X-X-X- </p>

> Question 3

Write a program to generate a dictionary that contains (i, i*)

Solution:

    p={}
    n=int(input())
    for i in range (1,n+1):
      p[str(i)]=str(i*i)
    print(" ".join(p))
    pp=p.values()
    print(" ".join(pp))
    
Output

    10
    1 2 3 4 5 6 7 8 9 10
    1 4 9 16 25 36 49 64 81 100
    
# <p align="center"> -X-X-X- </p>    
    
> Question 4  

Write a program to check if two strings are anagram

Solution:

    def anagram(s1,s2):
      return sorted(s1)==sorted(s2)
      
    a="ababa" #string 1
    b="ababa" #string 2
 
    print(anagram(a,b))
    
# <p align="center"> -X-X-X- </p>    
    
> Question 5  

Write a program to check if given strings are palindrome

Solution:

    a="malayalam"

    def check_palindrome(s1,s2):
      return s1==s2

    print(check_palindrome(a,a[::-1]))


# <p align="center"> -X-X-X- </p>    
    
> Question 6 

Find the Missing Number

Solution:

    a = [1,2,3,5]


    #as we know (n)*(n+1)/2 gives sum of n numbers

    # "sum_if_series_were_completed" corresponds to sum of [1,2,3,4,5]
    # "sum_of_missing_series" corresponds to sum of [1,2,3,5]


    def find_miss_no(series):
      p = len(series)
      sum_if_series_were_completed = ((p+1)*(p+2))/2
      sum_of_missing_series = sum(series)
      return sum_if_series_were_completed-sum_of_missing_series

    print(find_miss_no(a))


# <p align="center"> -X-X-X- </p>   


> Question 7

How do you debug a Python program?

Solution:

    python -m pdb prg_name.py
    pdb -> python debugger


# <p align="center"> -X-X-X- </p>   


> Question 8

Print  space seperated integers on a line denoting first N squares in the ascending order

Solution:

    p=int(input())

    for i in range(p):
        pp=i+1
        cc=pp*pp
        print( cc, end=" ")
        
        
  Output

      10
      1 4 9 16 25 36 49 64 81 100 

# <p align="center"> -X-X-X- </p>   


> Question 9

Convert Celsius To Fahrenheit

Solution:

    celsius = 37.5

    # calculate fahrenheit
    fahren = (celsius * 1.8) + 32
    print('%0.1f degree Celsius is equal to %0.1f degree Fahrenheit' %(celsius,fahren))

        
        
  Output

      37.5 degree Celsius is equal to 99.5 degree Fahrenheit 

# <p align="center"> -X-X-X- </p>   
