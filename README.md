# Pands-problem-set

##### Problem Set 2019 for GMIT Data Analytics 

* Author: Slawomir Sowa
* Technologies: Python 3.7
* Launch Date: 03.02.2019
---

#### Problem No.1 

    Write a program that asks the user to input any positive integer and outputs the sum of all  
    numbers between one and that number.

#### Solution:
    File Name: sumupto.py 
To solve problem I used WHILE loop, But before that I decide to verify provided by user   number. I imported SYS module which 
allow me to use methode exit() to stop program when   needed. In case that user provide string I used TRY and EXCEPT block to 
change 'Bad looking Error' to delivered by me. When error ocured in TRY block, EXCEPT block will be executed. In Next step I 
checked is provided number positive or negative Integer. I used IF ELSE   Statement. If provided number lower than 0 program will 
stop with comment. I declared two variables, i'll need them to store data.  
While loop every time checks is variable 'sum' lower than provided by user number. Every time   variable 'sum' is incremented by 1.
Also every time sum is added to sum_total. Program will   end when condition sum < number is false.   
    
    ref.
    https://teamtreehouse.com/community/about-import-sys-and-sysexit
    https://realpython.com/python-exceptions/#the-try-and-except-block-handling-exceptions

#### Problem No.2 
    Write a program that outputs whether or not today is a day that begins with the letter T. An   example of running this 
    program on a Thursday is as follows.

#### Solution:
    File Name: begins-with-t.py  
    We need to get current date. To do that we can use DATETIME module. By %A directive we can get   today's weekday name 
    and save it to list 'a' . Now we need to compare first item on the list   with letter 'T'. To do that i can use IF ELSE 
    statement.    

    ref.
    https://stackoverflow.com/questions/415511/how-to-get-the-current-time-in-python 
    https://docs.python.org/3/library/datetime.html

#### Problem No.3
    File name: divisors.py
    Write a program that prints all numbers between 1,000 and 10,000 that are divisible by 6 but not 12.

#### Solution:
    We can use loop FOR. FOR statement iterates over the members of a sequence in order, executing the block each time.
    In block we have IF statement. Number is divided by 6 if remainder = 0 and is not divided by 12 if remainder != 0. 
    If this condition is TRUE number is printed, if FALSE nothing happend. 
    
    ref.
    https://www.w3schools.com/python/python_for_loops.asp

#### Problem No 4
    File name: collatz.py
    Write a program that asks the user to input any positive integer and outputs the successive values of the following 
    calculation. At each step calculate the next value by taking the current value and, if it is even, divide it by two,
    but if it is odd, multiply it by three and add one. Have the program end if the current value is one.

#### Solution:
    First we check is provided number positive integer (explained in Problem no. 1), To solve problem we can use WHILE loop, 
    with nested IF ELSE statement. Loop will be repeated untill number = 1. If number different IF ELSE statement will be 
    executed. IF statement checks is division remainder of number divided by 2 equal 0. If TRUE number is divided and printed. 
    If NOT TRUE number is multipiled, added 1 and printed. WHILE loop checks condition again.

#### Problem No 5
    Write a program that asks the user to input a positive integer and tells the user whether or not the number is a prime.

#### Solution:
    File name: primes.py
    First we check is provided number positive integer (explained in Problem no. 1) Prime number is a number which remainder 
    of division is equal 0 only if divided by 1 and by itself. It means that Prime number will give us only two resoults 
    where remainder of division is = 0. We will store resoults of division in list. If list length = 2 number is prime. 
    If list length more that two number is not prime. To do that I used FOR loop. (TO REMEMBER: The last integer generated 
    by range() is up to, but not including ) This is why I added Number + 1.
    
    ref.
    https://www.w3schools.com/python/ref_list_append.asp


#### Problem No 6
    Write a program that takes a user input string and outputs every second word.
        
#### Solution
    File name: secondstring.py
    To solve that problem we need to get a provided by user string as a list. To do that we can use split() function, 
    and use space ' ' as a separator. We will need also list length. To print every second item from list we can use FOR 
    loop with incrementation step = 2, in range from 0 to list length. When list length is even we were getting an error 
    "IndexError: list index out of range", to avoid that i Used TRY EXCEPT statement.
    

    ref.
    https://stackoverflow.com/questions/743806/how-to-split-a-string-into-a-list
    https://stackoverflow.com/questions/12032214/print-new-output-on-same-line

#### Problem No. 7
    Write a program that that takes a positive floating point number as input and outputs an approximation of its square 
    root.

#### Solution
    File name: squareroot.py 
    First part of program will check of data provided. If string, will print error message. 
    Statement IF will check is number negative. In math theory we can do square root of negative number only if we 
    transform it to a complex number. A real number 'a' can be regarded as a complex number 'a + 0i' whose imaginary part 
    is 0. To work with complex number we need to import module cmath. If negative number provided IF block will be executed 
    and resoult printed as imaginary part of complex number with 'j'. If positive number provided ELSE block will be 
    executed and resoult of rounding printed.   

    ref.
    https://bbolker.github.io/math1mp/notes/random/r3_sqrtminusone.html
    https://docs.python.org/2/library/cmath.html
    https://en.wikipedia.org/wiki/Complex_number
