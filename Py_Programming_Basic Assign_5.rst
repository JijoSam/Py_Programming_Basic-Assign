1. Write a Python Program to Find LCM?
======================================

.. code:: ipython3

    x = 2
    y = 3
    
    if x>y:
        greater=x
    else:
        greater=y
    
    while(True):
        if (greater %x == 0 and greater %y == 0):
            print (f"lcm of {x} and {y} is {greater}")
            break
            maxNum = maxNum +1
    

2. Write a Python Program to Find HCF?
======================================

.. code:: ipython3

    num1 = int(input("Enter first number :  "))
    num2 = int(input("Enter second number :  "))
               
    if num1> num2:
               min = num1
    else:
               min = num2
               
    for i in range(1,min+1):
               if((num1 % i == 0) and (num2 % i == 0)):
                hcf = i 
        
    
    print("The H.C.F. is", compute_hcf(num1, num2))


.. parsed-literal::

    Enter first number :  24
    Enter second number :  36
    The H.C.F. is 12
    

3. Write a Python Program to Convert Decimal to Binary, Octal and Hexadecimal?
==============================================================================

.. code:: ipython3

    dec = 884
    
    print("The decimal value of", dec, "is:")
    print(bin(dec), "in binary.")
    print(oct(dec), "in octal.")
    print(hex(dec), "in hexadecimal.")


.. parsed-literal::

    The decimal value of 884 is:
    0b1101110100 in binary.
    0o1564 in octal.
    0x374 in hexadecimal.
    

4. Write a Python Program To Find ASCII value of a character?
=============================================================

.. code:: ipython3

    string = "INeuron"
    
    for i in string:
        print(f"ASCII value of '{i}' -- {ord(i)}")
     


.. parsed-literal::

    ASCII value of 'I' -- 73
    ASCII value of 'N' -- 78
    ASCII value of 'e' -- 101
    ASCII value of 'u' -- 117
    ASCII value of 'r' -- 114
    ASCII value of 'o' -- 111
    ASCII value of 'n' -- 110
    

5. Write a Python Program to Make a Simple Calculator with 4 basic mathematical operations?
===========================================================================================

.. code:: ipython3

    def add(a,b):
        return a+b
    
    def subtract(a,b):
        return a-b
    
    def mulitply(a,b):
        return a*b
    
    def divide(a,b):
        return a/b
    
    print("Select operation.")
    print("1.Add")
    print("2.Subtract")
    print("3.Multiply")
    print("4.Divide")
    
    while(True):
        choice = input("Enter your choice 1/2/3/4")
        
        if choice in ('1', '2', '3', '4'):
            
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            
            if choice == '1':
                print(num1, "+", num2, "=", add(num1, num2))
    
            elif choice == '2':
                print(num1, "-", num2, "=", subtract(num1, num2))
    
            elif choice == '3':
                print(num1, "*", num2, "=", multiply(num1, num2))
    
            elif choice == '4':
                print(num1, "/", num2, "=", divide(num1, num2))
            
            # check if user wants another calculation
            # break the while loop if answer is no
            next_calculation = input("Let's do next calculation? (yes/no): ")
            if next_calculation == "no":
              break
        
        else:
            print("Invalid Input")


.. parsed-literal::

    Select operation.
    1.Add
    2.Subtract
    3.Multiply
    4.Divide
    Enter your choice 1/2/3/44
    Enter first number: 4
    Enter second number: 5
    4.0 / 5.0 = 0.8
    
