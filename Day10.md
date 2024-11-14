# Python
## Keywords and Identifiers
- Keywords are reserved words in Python
- Keywords cannot be used as a variable name, function name or any other identifier
- For identifiers we need to follow some rules while creating them
  Comments - # , '''text with more than one lines'''
  Variables and Data types
  Numeric
  - Integer
  - Float
  - Complex
  type() - to know the data type
  len() - No of Characters
  print() - to print values

  ## Sequence Type
- **List** - a collection of elements grouped together
  - mix of data types is possible
  - Syntax :
    - digits = [0,1,2,3,4]
    - alpha = ['a','e','b']
    - grocery = ['Apple',5,'Grapes']
  - list within a list
      -1. List = [[1,3,5,7], [2,4,6,8,10]] 
      -2. odd =[1,3,5]
        even =[2,4,6]
        List = [odd,even]

   ### Indexing of a list
  Lists are Mutable  ie, we can change the elements
  we cannot be add items to List (IndexError: list assignment index out of range)

  - **Tuple**
   - immutable, once we create a tuple, we cannot change, add or remove items
   - This immutability can help protect data from accidental modification and also makes tuple more memory efficient.
   - my_tuple = (1,2,3)
     
  - **Range** -the range datatype in py represents an immutable sequence of numbers
      - range(start,stop,skip)
      - range(5) = 0,1,2,3,4
      - a= list(range (1,5))
        print(a)
      - z= list(range(10,1,-2))
        print(z)

 ### Dictionary - derived datatype
 - an unordered mutable collection that stores data in any key-value pairs.
 - Each key in a dictionary must be unique, while values can be duplicated.
 - Syntax :  data ={
 -                     "name" : "Merlin",
                        "Place" : "tvm"
                   }

### Set - unordered collection of unique items
 syntax : my_set = {1,2,3,4}

Boolean Type
None Type -represents an absence of value or a null value

## Operators
1- Arthematic Operations (Addition, Subtraction, Multiplication, Division, Modulus, Exponentiation)
    integer division "//" will eliminate decimal numbers
    a=13
    b= 2
    c=a//b
    print(c)
    Exponentiation
    a=2
    b= 2
    c=a**b
    print(c)
2. Comparision Operators( == ,!=,<,>,<=,>=)
3. Logical Operators (AND, OR, NOT)
4. Membership Operators( IN,NOTIN)
      print('a' in 'apple') 
      True
5. Identity Operator (IS ,ISNOT)
     a=10
     b=10
     print (a is b)
     a= a+1
     b=10
     c=10
     print (c is b)
      true
### Conditional Statements
Syntax : 
         x=11
        if (x%2==0):
              print(x," is even")
        else:
             print(x, "is odd")

 nested if else(browse)

  ## slice notation
 a="water"
 a[0:3]
 a[: :-1]
 syntax : a= "watermelon"
          a[::-1] 
          result = 'nolemretaw'
