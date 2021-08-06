1. Write a Python program to convert kilometers to miles?
=========================================================

.. code:: ipython3

    kilometers = float(input("Enter Kilometer value  "))
    
    conv_fac = 0.621371
    
    miles = conv_fac * kilometers
    
    print('%0.2f kilometers is equal to %0.2f miles' %(kilometers,miles))     #%0.2f takes in how many decimal values the output wants


.. parsed-literal::

    Enter Kilometer value  35
    35.00 kilometers is equal to 21.75 miles
    

2. Write a Python program to convert Celsius to Fahrenheit?
===========================================================

.. code:: ipython3

    celsius = float(input("Enter celsius value   "))
    fahrenheit = (celsius * 1.8) + 32
    
    print('%0.1f celsius is equal to %0.1f fahrenheit' % (celsius,fahrenheit))


.. parsed-literal::

    Enter celsius value   36
    36.0 celsius is equal to 96.8 fahrenheit
    

3. Write a Python program to display calendar?
==============================================

.. code:: ipython3

    # importing calendar module
    
    import calendar
    
    year = int(input("Enter year:  ")) 
    month = int(input("Enter month:  "))  
    
    mycal = calendar.month(year,month)
    
    print(mycal)


.. parsed-literal::

    Enter year:  2020
    Enter month:  2
       February 2020
    Mo Tu We Th Fr Sa Su
                    1  2
     3  4  5  6  7  8  9
    10 11 12 13 14 15 16
    17 18 19 20 21 22 23
    24 25 26 27 28 29
    
    

4. Write a Python program to solve quadratic equation?
======================================================

.. code:: ipython3

    import cmath
    
    print("General quadratic equation is ax**2+bx+c = 0")
    
    a = int(input("Enter value for a where (a!=0) is  "))
    b = int(input("Enter value for b  "))
    c = int(input("Enter value for c  "))
    
    d = (b**2 - 4*a*c)
            
    sol1 = (-b + cmath.sqrt(d))/(2*a)
    sol2 = (-b - cmath.sqrt(d))/(2*a)
    
    print("\n")
    print(f"Results for equation {a}x**2 + {b}x + {c} = 0 are:\n" )
            
    if d>0:
            print("Type of roots: Two Distinct real root")
    elif d==0:
            print("Type of roots: Two equal real roots")
    elif d<0:
            print("Type of roots: Two complex roots")
            
            
    print(f"The solutions are {sol1} and {sol2}")


.. parsed-literal::

    General quadratic equation is ax**2+bx+c = 0
    Enter value for a where (a!=0) is  64
    Enter value for b  12
    Enter value for c  22
    
    
    Results for equation 64x**2 + 12x + 22 = 0 are:
    
    Type of roots: Two complex roots
    The solutions are (-0.09375+0.5787580992953792j) and (-0.09375-0.5787580992953792j)
    

5. Write a Python program to swap two variables without temp variable?
======================================================================

.. code:: ipython3

    X = 10
    Y = 20
    
    #values are swaped as below
    X = 20
    Y = 10
        
    print(f"The swapped solutions of X is {X} and Y is {Y}")
    


.. parsed-literal::

    The swapped solutions of X is 20 and Y is 10
    
