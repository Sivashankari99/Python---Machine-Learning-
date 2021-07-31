# Python-Machine-Learning
1.	PYTHON INTRODUCTION 

AIM:
To write a python program to execute various basic commands of python.
DESCRIPTION:
In this first experiment we will go through the basic examples of python and understand different data types, operators, conditional statements, methods etc.

PROGRAMS WITH OUTPUT:
Data types:
Numbers:
1 + 1
Output: 2
1 * 3
Output: 3
1 / 2
Output: 0.5
2 ** 4
Output: 16
4 % 2
Output: 0
5 % 2
Output: 1
(2 + 3) * (5 + 5)
Output: 50


Variable Assignment:
# Can not start with number or special characters
name_of_var = 2
x = 2
y = 3
z = x + y
z
Output: 5

Strings:
'single quotes'
Output: 'single quotes'
"double quotes"
Output: 'double quotes'
" wrap lot's of other quotes"
Output: " wrap lot's of other quotes"

Printing:
x = 'hello'
x
Output: 'hello'
print(x)
Output: hello
num = 12
name = 'Sam'
print('My number is: {one}, and my name is: {two}'.format(one=num,two=name))
Output: My number is: 12, and my name is: Sam
print('My number is: {}, and my name is: {}'.format(num,name))
Output: My number is: 12, and my name is: Sam

Lists:
[1,2,3]
Output: [1, 2, 3]
['hi',1,[1,2]]
Output: ['hi', 1, [1, 2]]
my_list = ['a','b','c']
my_list.append('d')
my_list
Output: ['a', 'b', 'c', 'd']
my_list[0]
Output: 'a'
my_list[1]
Output: 'b'
my_list[1:]
Output: ['b', 'c', 'd']
my_list[:1]
Output: ['a']
my_list[0] = 'NEW'
my_list
Output: ['NEW', 'b', 'c', 'd']
nest = [1,2,3,[4,5,['target']]]
nest[3]
Output: [4, 5, ['target']]
nest[3][2]
Output: ['target']
nest[3][2][0]
Output: 'target'

Dictionaries:
d = {'key1':'item1','key2':'item2'}
d
Output: {'key1': 'item1', 'key2': 'item2'}
d['key1']
Output: 'item1'

Booleans:
True
Output: True
False
Output: False

Tuples:
t = (1,2,3)
t[0]
Output: 1
t[0] = 'NEW'
Output:
TypeError                                 Traceback (most recent call last)
TypeError: 'tuple' object does not support item assignment

Sets:
{1,2,3}
Output: {1, 2, 3}
{1,2,3,1,2,1,2,3,3,3,3,2,2,2,1,1,2}
Output: {1, 2, 3}

Comparison Operators:
1 > 2
Output: False
1 < 2
Output: True
1 >= 1
Output: True
1 <= 4
Output: True
1 == 1
Output: True
'hi' == 'bye'
Output: False

Logic Operators:
(1 > 2) and (2 < 3)
Output: False
(1 > 2) or (2 < 3)
Output: True
(1 == 2) or (2 == 3) or (4 == 4)
Output: True

if,elif, else Statements:
if 1 < 2:
    print('Yep!')
Output: Yep!
if 1 < 2:
    print('yep!')
Output: yep!
if 1 < 2:
    print('first')
else:
    print('last')
Output: first
if 1 > 2:
    print('first')
else:
    print('last')
Output: last
if 1 == 2:
    print('first')
elif 3 == 3:
    print('middle')
else:
    print('Last')
Output: middle

for Loops:
seq = [1,2,3,4,5]
for item in seq:
    print(item)
Output:
1
2
3
4
5
for item in seq:
    print('Yep')
Output:
Yep
Yep
Yep
Yep
Yep
for jelly in seq:
    print(jelly+jelly)
Output:
2
4
6
8
10

while Loops:
i = 1
while i < 5:
    print('i is: {}'.format(i))
    i = i+1
Output:
i is: 1
i is: 2
i is: 3
i is: 4

range():
range(5)
Output: range(0, 5)
for i in range(5):
    print(i)
Output:
0
1
2
3
4
list(range(5))
Output: [0, 1, 2, 3, 4]

list comprehension:
x = [1,2,3,4]
out = []
for item in x:
    out.append(item**2)
print(out)
Output: [1, 4, 9, 16]
[item**2 for item in x]
Output: [1, 4, 9, 16]

functions:
def my_func(param1='default'):
    """
    Docstring goes here.
    """
    print(param1)
my_func
Output: <function __main__.my_func(param1='default')>
my_func()
Output: default
my_func('new param')
Output: new param
my_func(param1='new param')
Output: new param
def square(x):
    return x**2
out = square(2)
print(out)
Output: 4

lambda expressions:
def times2(var):
    return var*2
times2(2)
Output: 4
x=lambda var: var*2
x(3)
Output: 6

map and filter:
seq = [1,2,3,4,5]
map(times2,seq)
Output: <map at 0x16b151364a8>
list(map(times2,seq))
Output: [2, 4, 6, 8, 10]
list(map(lambda var: var*2,seq))
Output: [2, 4, 6, 8, 10]
filter(lambda item: item%2 == 0,seq)
Output: <filter at 0x16b150b5908>
list(filter(lambda item: item%2 == 0,seq))
Output: [2, 4]

methods:
st = 'hello my name is Sam'
st.lower()
Output: 'hello my name is sam'
st.upper()
Output: 'HELLO MY NAME IS SAM'
st.split()
Output: ['hello', 'my', 'name', 'is', 'Sam']
tweet = 'Go Sports! #Sports'
tweet.split('#')
Output: ['Go Sports! ', 'Sports']
tweet.split('#')[1]
Output: 'Sports'
d
Output: {'key1': 'item1', 'key2': 'item2'}
d.keys()
Output: dict_keys(['key1', 'key2'])
d.items()
Output: dict_items([('key1', 'item1'), ('key2', 'item2')])
lst = [1,2,3]
lst.pop()
Output: 3
lst
Output: [1, 2]
'x' in [1,2,3]
Output: False
'x' in ['x','y','z']
Output: True


EXERCISES:
1.	What is 7 to the power of 4?

7**4

Output: 2401
2.	Split this string: s = "Hi there Sam!" into a list

s = "Hi there Sam!" 
s.split()

Output: ['Hi', 'there', 'Sam!']
3.	planet = "Earth", diameter = 12742
Use .format() to print the following string:
The diameter of Earth is 12742 kilometers.

planet = "Earth"
diameter = 12742  
print("The diameter of {} is {} kilometers.".format(planet,diameter))

Output: The diameter of Earth is 12742 kilometers.
4.	Given this nested list, use indexing to grab the word "hello"
lst = [1,2,[3,4],[5,[100,200,['hello']],23,11],1,7]

lst = [1,2,[3,4],[5,[100,200,['hello']],23,11],1,7]
lst[3][1][2][0]
#look for the index

Output: 'hello'
5.	Given this nest dictionary grab the word "hello".
d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}

d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}
d['k1'][3]['tricky'][3]['target'][3]

Output: 'hello'
6.	What is the main difference between a tuple and a list?

Output: Tuple is immutable
7.	Create a function that grabs the email website domain from a string in the form:
“user@domain.com”
Passing "user@domain.com" would return: domain.com

def a(x):
    return x.split('@')[1] #a split is formed at @
a('user@domain.com')

Output: 'domain.com'

def a(x):
    return x.split('@')[1]
a('user@domain.com@in')

Output: 'domain.com'
8.	Create a basic function that returns True if the word 'dog' is contained in the input string:
'Is there a dog here?'. Do account capitalization.

def a(x):
    return 'dog' in x.lower().split()
a('Is there a dog here?')

Output: True
9.	Create a function that counts the number of times the word "dog" occurs in a string:
'Is there a dog here?'

def countDog(st):
    count = 0
    for word in st.lower().split():
        if word == 'dog':
            count += 1
    return count
countDog('This dog runs faster than the other dog dude!')

Output: 2

def a(x):
    return x.count('dog')
a('Is there a dog dog here?')

Output: 2
10.	Use lambda expressions and the filter() function to filter out words from a list that don't start with the letter 's'. 
For example: seq = ['soup','dog','salad','cat','great'] 
Should be filtered down to:  ['soup','salad']

seq = ['soup','dog','salad','cat','great']
list(filter(lambda x: x[0]=='s',seq))

Output: ['soup', 'salad']
11.	You are driving a little too fast, and a police officer stops you. Write a function to return one of 3 possible results:
If speed is 60 or less, the result is "No Ticket".
If speed is between 61 and 80 inclusive, the result is "Small Ticket".
If speed is 81 or more, the result is "Big Ticket".
Unless it is your birthday (encoded as a boolean value in the parameters of the function), your speed can be 5 higher in all cases. 

def caught_speeding(speed, is_birthday):
    if is_birthday:
        speeding = speed + 5
    else:
        speeding = speed
     if speeding <= 60:
        return 'No Ticket'
    elif speeding > 61 and speeding <= 80:
        return 'Small Ticket'
    elif speeding >= 81:
        return 'Big Ticket'
caught_speeding(56,True)

caught_speeding(56,False)

Output: 'No Ticket'

caught_speeding(56,False)

Output: 'No Ticket'

CONCLUSION:
Hence, python programs to perform various basic commands have been written, executed and output has been verified.

2. INTRODUCTION TO NUMPY

AIM:
To write a program in python to execute the basics of Numpy. 

DESCRIPTION:
NumPy (or Numpy) is a Linear Algebra Library for Python, the reason it is so important for Data Science with Python is that almost all of the libraries in the PyData Ecosystem rely on NumPy as one of their main building blocks.

Built-in Methods:
There are lots of built-in ways to generate arrays.

arange:
Return evenly spaced values within a given interval.
zeros and ones:
Generate arrays of zeros or ones.
linspace:
Return evenly spaced numbers over a specified interval.
eye:
Creates an identity matrix.
Random:
Numpy also has lots of ways to create random number arrays.
rand:
Create an array of the given shape and populate it with random samples from a uniform distribution over [0, 1).
randn:
Return a sample (or samples) from the "standard normal" distribution. 
randint:
Return random integers from low (inclusive) to high (exclusive).

reshape:
Returns an array containing the same data with a new shape.
max,min,argmax,argmin:
These are useful methods for finding max or min values or to find their index locations using argmin or argmax.
shape:
Shape is an attribute that arrays have (not a method):
dtype:
Data type of the object in the array can be retrieved.
PROGRAMS WITH OUTPUT:
import numpy as np

Arrays:
x=[1, 2, 3, 4, 5]
np.array(x)
Output: array([1, 2, 3, 4, 5])
x=np.array(16)    
x
Output: array(16)
x=numpy.array([[1, 2, 3], [4, 5, 6]])
print(x)
Output:
[[1 2 3]
 [4 5 6]]

Array indexing:
x=np.array([1, 2, 3, 4, 5])    
x[1]
Output: 2

x=np.array([[1, 2, 3], [4, 5, 6]])
x[1,2]
Output: 6

Array Slicing:
x=np.array([1, 2, 3, 4, 5]) #includes start index 1(eg.2) but omits end index(eg.5)
x[1:3]
Output: array([2, 3])
x=np.array([1, 2, 3, 4, 5]) #starts from index 0 but omits end index(eg.5)
x[:3]
Output: array([1, 2, 3])
x=np.array([1, 2, 3, 4, 5]) #starts from index 1 and prints till last value
x[1:]
Output: array([2, 3, 4, 5])
x=np.array([1, 2, 3, 4, 5]) 
#-3 and -1 prints from reverse
#includes end index 1(eg.4) but omits start index(eg.2)
x[-3:-1]
Output: array([3, 4])
x=np.array([1, 2, 3, 4, 5])
x[0:4:2]
#prints from index0 to index4 with space of 2
Output: array([1, 3])

BUILT-IN METHODS:
arange:
np.arange(1,5,3)
#3 refers to gap between the first two numbers
Output: array([1, 4])
np.arange(0,10)
Output: array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])

np.arange(0,11,2)
Output: array([ 0,  2,  4,  6,  8, 10])

zeros and ones:
np.zeros(2)
Output: array([0., 0.])
np.zeros((2,2))
Output:
array([[0., 0.],
       [0., 0.]])
np.ones(2)
Output: array([1., 1.])
np.ones((2,2))
Output:
array([[1., 1.],
       [1., 1.]])

linspace:
np.linspace(1,7,4)
#linspace is done with eaual spacing(4 refers to number of integers to be printed with equal spacing)
Output: array([1., 3., 5., 7.])
np.linspace(0,10,3)
Output: array([ 0.,  5., 10.])






np.linspace(0,10,50)
Output: 
array([ 0.        ,  0.20408163,  0.40816327,  0.6122449 ,  0.81632653,
        1.02040816,  1.2244898 ,  1.42857143,  1.63265306,  1.83673469,
        2.04081633,  2.24489796,  2.44897959,  2.65306122,  2.85714286,
        3.06122449,  3.26530612,  3.46938776,  3.67346939,  3.87755102,
        4.08163265,  4.28571429,  4.48979592,  4.69387755,  4.89795918,
        5.10204082,  5.30612245,  5.51020408,  5.71428571,  5.91836735,
        6.12244898,  6.32653061,  6.53061224,  6.73469388,  6.93877551,
        7.14285714,  7.34693878,  7.55102041,  7.75510204,  7.95918367,
        8.16326531,  8.36734694,  8.57142857,  8.7755102 ,  8.97959184,
        9.18367347,  9.3877551 ,  9.59183673,  9.79591837, 10.        ])
eye:
np.eye(3) #identity matrix
Output:
array([[1., 0., 0.],
       [0., 1., 0.],
       [0., 0., 1.]])

Random:
rand:
np.random.rand(2) #gives uniform distribution
Output: array([0.59899436, 0.57500594])
np.random.rand(5,5)
Output:
array([[0.8532597 , 0.78513659, 0.36389639, 0.81208698, 0.27504804],
       [0.43572746, 0.29009358, 0.60207693, 0.30800814, 0.26021457],
       [0.90321102, 0.91925396, 0.13992916, 0.03292513, 0.93188869],
       [0.98898628, 0.09062172, 0.52095818, 0.34706827, 0.02027942],
       [0.99790924, 0.5957805 , 0.76999301, 0.05253998, 0.14099702]])

randn:
np.random.randn(2) #gives standard normal distribution
Output: array([ 0.3475921 , -0.89893673])
np.random.randn(5,5)
Output:
array([[ 7.88238894e-04,  1.98097952e+00, -1.34520834e+00,
        -1.42765648e+00,  8.78573621e-01],
       [-8.42102821e-01, -3.33368933e-02,  6.80767197e-02,
        -1.75352891e-01, -1.58288094e+00],
       [ 8.44616834e-01,  6.22000673e-01,  3.75869213e-01,
        -5.64942435e-01, -8.94084724e-01],
       [-7.18814278e-01,  1.02690101e+00,  7.64674021e-01,
        -3.34669840e-01,  7.08345840e-01],
       [ 3.84149740e-01, -3.09014613e-01,  1.07635099e+00,
        -9.26246979e-01, -8.81341808e-01]])

randint:
np.random.randint(100)
Output: 41
np.random.randint(1,100)
Output: 85
np.random.randint(1,100,10)
Output: array([35, 64, 63, 90, 47, 18, 21, 71,  9, 38])
np.random.randint(1,20,(5,5))
Output:
array([[19, 19, 19,  8,  5],
       [15,  4, 19, 11, 19],
       [ 5,  2,  5,  1, 14],
       [16, 10,  1, 17,  9],
       [19, 18,  5,  6,  1]])

shape:
arr=numpy.array([[1,2,3],[4,5,6]]) #specifies rows and columns
arr.shape
Output: (2, 3)
reshape:
arr=np.array([[1,2,3],[4,5,6]])
arr.reshape(6,1)
Output:
array([[1],
       [2],
       [3],
       [4],
       [5],
       [6]])
arr=np.array([[1,2,3,4],[4,5,6,7]])
arr.reshape (2,2,2)
Output:
array([[[1, 2],
        [3, 4]],

       [[4, 5],
        [6, 7]]])
arr=numpy.array([1,2,3,4,5,6])
print(arr.shape)
print('\n')
b=arr.reshape(2,3)
print(b)
print('\n')
print(b.shape)
Output:
(6,)

[[1 2 3]
 [4 5 6]]

(2, 3)

Flattening:
arr=numpy.array([[1,2,3],[4,5,6]]) #converts 2D array into 1D
print (arr.reshape(-1))
Output: [1 2 3 4 5 6]
max,min,argmax,argmin:
arr=np.array([1,2,3,4,5,6])
arr.max()
Output: 6
arr.min()
Output: 1
arr.argmax()
Output: 5
arr.argmin()
Output: 0

dtype:
arr=numpy.array([1,2,3,4,5,6])
arr.dtype
Output: dtype('int32')
arr=numpy.array(['a','b','c'])
arr.dtype
Output: dtype('<U1')
arr=numpy.array([1,2],dtype='S') #S refers to String
arr.dtype
Output: dtype('S1')

ASSIGNMENT:
import numpy as np
1.Create an array of 10 zeros
np.zeros(10)
Output: array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])
2.Create an array of 10 ones
np.ones(10)
Output: array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])
3.Create an array of 10 fives
np.ones(10) * 5
Output: array([5., 5., 5., 5., 5., 5., 5., 5., 5., 5.])
4.Create an array of the integers from 10 to 50
np.arange(10,51)
Output:
array([10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26,
       27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43,
       44, 45, 46, 47, 48, 49, 50])
5.Create an array of all the even integers from 10 to 50
np.arange(10,51,2)
Output:
array([10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42,
       44, 46, 48, 50])
6.Create a 3x3 matrix with values ranging from 0 to 8
np.arange(9).reshape(3,3)
Output:
array([[0, 1, 2],
       [3, 4, 5],
       [6, 7, 8]])





7.Create a 3x3 identity matrix
np.eye(3)
Output:
array([[1., 0., 0.],
       [0., 1., 0.],
       [0., 0., 1.]])
8.Use NumPy to generate a random number between 0 and 1
np.random.rand(1)
Output: array([0.6149836])
9.Use NumPy to generate an array of 25 random numbers sampled from a standard normal distribution
np.random.randn(25)
Output:
array([-1.04836744e+00, -2.97633916e+00, -3.82111702e-01, -1.93406555e-03,
        8.64101535e-01, -8.37096674e-01, -1.79030546e+00,  3.15415355e-01,
       -1.13173998e+00,  1.34093125e+00, -1.12248717e-01,  8.21505846e-01,
        1.20541731e+00, -7.98198623e-01,  5.92267250e-01, -4.88767801e-01,
        1.72576041e+00,  5.15198394e-01, -1.41620420e+00,  6.23389058e-02,
        4.39328639e-01,  5.47428877e-01, -1.43637000e+00,  4.52558065e-01,
        3.15599124e-01])
10.Create an array of 20 linearly spaced points between 0 and 1
np.linspace(0,1,20)
Output:
array([0.        , 0.05263158, 0.10526316, 0.15789474, 0.21052632,
       0.26315789, 0.31578947, 0.36842105, 0.42105263, 0.47368421,
       0.52631579, 0.57894737, 0.63157895, 0.68421053, 0.73684211,
       0.78947368, 0.84210526, 0.89473684, 0.94736842, 1.        ])

CONCLUSION:
Hence, various python programs to perform basics of  Numpy have been written, executed and output has been verified.

3.	NUMPY INDEXING AND SELECTION

AIM:
To write a python program to select elements or groups of elements from an array.
DESCRIPTION:
Bracket Indexing and Selection:
The simplest way to pick one or some elements of an array which looks similar to python lists.
Broadcasting:
Numpy arrays differ from a normal Python list because of their ability to broadcast. Broadcasting describes how numpy treats arrays with different shapes during arithmetic operations.
Indexing a 2D array (matrices):
The general format of a 2D array is arr_2d[row][col] or arr_2d[row,col]. 
Fancy Indexing:
Fancy indexing helps to select entire rows or columns out of order.
Selection:
Refers to the use of brackets for selection including comparison operators.
PROGRAMS WITH OUTPUT:
import numpy as np

#Creating sample array
arr = np.arange(0,11)
#Show
arr
Output: array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])



Bracket Indexing and Selection:
#Get a value at an index
arr[8]
Output: 8
#Get values in a range
arr[1:5]
Output: array([1, 2, 3, 4])
#Get values in a range
arr[0:5]
Output: array([0, 1, 2, 3, 4])
arr[4:]
Output: array([ 4,  5,  6,  7,  8,  9, 10])

Broadcasting:
#Setting a value with index range (Broadcasting)
arr[0:5]=100
#Show
arr
Output: array([100, 100, 100, 100, 100,   5,   6,   7,   8,   9,  10])
arr[4]=10
arr
Output: array([ 0,  1,  2,  3, 10,  5,  6,  7,  8,  9, 10])
arr[4:]=10
arr
Output: array([ 0,  1,  2,  3, 10, 10, 10, 10, 10, 10, 10])


# Reset array, we'll see why I had to reset in  a moment
arr = np.arange(0,11)
#Show
arr
Output: array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])
#Important notes on Slices
slice_of_arr = arr[0:6]
#Show slice
slice_of_arr
Output: array([0, 1, 2, 3, 4, 5])
#Change Slice
slice_of_arr[:]=99
#Show Slice again
slice_of_arr
Output: array([99, 99, 99, 99, 99, 99])
#The changes also occur in the original array
arr
Output: array([99, 99, 99, 99, 99, 99,  6,  7,  8,  9, 10])
#Data is not copied, it's a view of the original array
#To get a copy, need to be explicit
arr_copy = arr.copy()
arr_copy
Output: array([99, 99, 99, 99, 99, 99,  6,  7,  8,  9, 10])

Indexing a 2D array (matrices):
arr_2d = np.array(([5,10,15],[20,25,30],[35,40,45]))
#Show
arr_2d
Output:
array([[ 5, 10, 15],
       [20, 25, 30],
       [35, 40, 45]])
#Indexing row
arr_2d[1]
Output: array([20, 25, 30])
# Format is arr_2d[row][col] or arr_2d[row,col]
# Getting individual element value
arr_2d[1][0]
Output: 20
# Getting individual element value
arr_2d[1,0]
Output: 20
# 2D array slicing
#Shape (2,2) from top right corner
arr_2d[:2,1:]
Output:
array([[10, 15],
       [25, 30]])
#Shape bottom row
arr_2d[2]
Output: array([35, 40, 45])
#Shape bottom row
arr_2d[2,:]
Output: array([35, 40, 45])

Fancy Indexing:
#Fancy indexing allows you to select entire rows or columns out of order
#Set up matrix
arr2d = np.zeros((10,10))
#Length of array
arr_length = arr2d.shape[1]
#Set up array
for i in range(arr_length):
    arr2d[i] = i    
arr2d





Output:
array([[0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],
       [1., 1., 1., 1., 1., 1., 1., 1., 1., 1.],
       [2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],
       [3., 3., 3., 3., 3., 3., 3., 3., 3., 3.],
       [4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],
       [5., 5., 5., 5., 5., 5., 5., 5., 5., 5.],
       [6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],
       [7., 7., 7., 7., 7., 7., 7., 7., 7., 7.],
       [8., 8., 8., 8., 8., 8., 8., 8., 8., 8.],
       [9., 9., 9., 9., 9., 9., 9., 9., 9., 9.]])
arr2d[[2,4,6,8]]
Output: 
array([[2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],
       [4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],
       [6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],
       [8., 8., 8., 8., 8., 8., 8., 8., 8., 8.]])
#Allows in any order
arr2d[[6,4,2,7]]
Output:
array([[6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],
       [4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],
       [2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],
       [7., 7., 7., 7., 7., 7., 7., 7., 7., 7.]])

Selection:
arr = np.arange(1,11)
arr
Output: array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10])
arr > 4
Output: array([False, False, False, False,  True,  True,  True,  True,  True,  True])
bool_arr = arr>4
bool_arr
Output: array([False, False, False, False,  True,  True,  True,  True,  True,  True])

arr[bool_arr]
Output: array([ 5,  6,  7,  8,  9, 10])
arr[arr>2]
Output: array([ 3,  4,  5,  6,  7,  8,  9, 10])
x = 2
arr[arr>x]
Output: array([ 3,  4,  5,  6,  7,  8,  9, 10])














CONCLUSION:
Hence, various python programs to perform selection of elements or groups of elements from an array have been written, executed and output has been verified.

 
4.	NUMPY OPERATIONS
AIM:
To write a program in python to display various operations of arrays using NumPy.
DESCRIPTION:
Various operations between two arrays including array with array arithmetic, or scalar with array arithmetic will be performed along with few universal array functions which are commonly used in python.
Arithmetic:
Input arrays are used for performing arithmetic operations such as add(), subtract(), multiply(), and divide() etc.
Universal Array Functions:
Universal functions in Numpy are simple mathematical functions. It is a term given to mathematical functions in the Numpy library. Numpy provides various universal functions that cover a wide variety of operations. These functions include standard trigonometric functions, functions for arithmetic operations, handling complex numbers, statistical functions, etc.
PROGRAMS WITH OUTPUT:
import numpy as np
arr = np.arange(0,10)
arr + arr
Output: array([ 0,  2,  4,  6,  8, 10, 12, 14, 16, 18])
arr * arr
Output: array([ 0,  1,  4,  9, 16, 25, 36, 49, 64, 81])
arr - arr
Output: array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
# Warning on division by zero, but not an error!
# Just replaced with nan
arr/arr
C:\ProgramData\Anaconda3\lib\site-packages\ipykernel_launcher.py:3: RuntimeWarning: invalid value encountered in true_divide
  This is separate from the ipykernel package so we can avoid doing imports until

Output: array([nan,  1.,  1.,  1.,  1.,  1.,  1.,  1.,  1.,  1.])
# Warning, but not an error instead infinity
1/arr
C:\ProgramData\Anaconda3\lib\site-packages\ipykernel_launcher.py:2: RuntimeWarning: divide by zero encountered in true_divide
Output:

array([       inf, 1.        , 0.5       , 0.33333333, 0.25      ,
       0.2       , 0.16666667, 0.14285714, 0.125     , 0.11111111])
arr**3
Output: array([  0,   1,   8,  27,  64, 125, 216, 343, 512, 729], dtype=int32)

Universal Array Functions:
#Taking Square Roots
np.sqrt(arr)
Output:
array([0.        , 1.        , 1.41421356, 1.73205081, 2.        ,
       2.23606798, 2.44948974, 2.64575131, 2.82842712, 3.        ])
#Calcualting exponential (e^)
np.exp(arr)
Output:
array([1.00000000e+00, 2.71828183e+00, 7.38905610e+00, 2.00855369e+01,
       5.45981500e+01, 1.48413159e+02, 4.03428793e+02, 1.09663316e+03,
       2.98095799e+03, 8.10308393e+03])
np.max(arr) #same as arr.max()
Output: 9
np.sin(arr)
Output:
array([ 0.        ,  0.84147098,  0.90929743,  0.14112001, -0.7568025 ,
       -0.95892427, -0.2794155 ,  0.6569866 ,  0.98935825,  0.41211849])



np.log(arr)
Output:

array([      -inf, 0.        , 0.69314718, 1.09861229, 1.38629436,
       1.60943791, 1.79175947, 1.94591015, 2.07944154, 2.19722458])
















CONCLUSION:
Hence, python programs to perform various operations have been written, executed and output has been verified.



5. INTRODUCTION TO PANDAS - SERIES

AIM:
To write a program in python to display the function of series using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

Series:
The first main data type for pandas is the Series data type
A Series is very similar to a NumPy array (in fact it is built on top of the NumPy array object) but a Series can have axis labels, meaning it can be indexed by a label, instead of just a number location. It also doesn't need to hold numeric data, it can hold any arbitrary Python Object.
PROGRAMS WITH OUTPUT:
import numpy as np
import pandas as pd
Creating a Series:
#A list, numpy array, or dictionary can be converted into a Series
labels = ['a','b','c']
my_list = [10,20,30]
arr = np.array([10,20,30])
d = {'a':10,'b':20,'c':30}
Using Lists:

pd.Series(data=my_list)
Output:
0    10
1    20
2    30
dtype: int64

pd.Series(data=d)
Output:
a    10
b    20
c    30
dtype: int64
pd.Series(data=labels)
Output:
0    a
1    b
2    c
dtype: object
pd.Series(data=my_list,index=labels)
Output:
a    10
b    20
c    30
dtype: int64
pd.Series(index=labels,data=my_list)
Output:
a    10
b    20
c    30
dtype: int64
pd.Series(my_list,labels)
Output:
a    10
b    20
c    30
dtype: int64




Using NumPy Arrays: 
pd.Series(arr)
Output:
0    10
1    20
2    30
dtype: int32
pd.Series(arr,labels)
Output:
a    10
b    20
c    30
dtype: int32

Using Dictionary:
pd.Series(d)
Output:
a    10
b    20
c    30
dtype: int64
Data in a Series:
# A pandas Series can hold a variety of object types
pd.Series(data=labels)
Output:
0    a
1    b
2    c
dtype: object

Using an Index:
# The key to using a Series is understanding its index. Pandas makes use of these index names or numbers by allowing for fast look ups of information (works like a hash table or dictionary).
ser1 = pd.Series([1,2,3,4],index = ['USA', 'Germany','USSR', 'Japan'])                                   
ser1
Output:
USA        1
Germany    2
USSR       3
Japan      4
dtype: int64
ser2 = pd.Series([1,2,5,4],index = ['USA', 'Germany','Italy', 'Japan'])                                   
ser2
Output:
USA        1
Germany    2
Italy      5
Japan      4
dtype: int64
ser1[‘USA’]
Output: 1
# Operations are then also done based off of index:
ser1 + ser2
Output:
Germany    4.0
Italy      NaN
Japan      8.0
USA        2.0
USSR       NaN
dtype: float64

CONCLUSION:
Hence, various python programs to display the functions of series using pandas library have been written, executed and output has been verified. 
6. INTRODUCTION TO PANDAS - DATAFRAMES

AIM:
To write a program in python to display the functions of dataframes using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

Dataframes:
DataFrame is a bunch of Series objects put together to share the same index. 
Selection and Indexing:
Grabs data from Dataframe.
Conditional Selection:
An important feature of pandas is conditional selection using bracket notation, very similar to numpy.
Indexing:
Various features of indexing includes resetting the index ,setting it to something else, index hierarchy etc.

PROGRAMS WITH OUTPUT:
import pandas as pd
import numpy as np
from numpy.random import randn
np.random.seed(101)
df = pd.DataFrame(randn(5,4),index='A B C D E'.split(),columns='W X Y Z'.split())
df


Output:
 

Selection and Indexing:
df['W']
Output:
A    2.706850
B    0.651118
C   -2.018168
D    0.188695
E    0.190794
Name: W, dtype: float64

# Pass a list of column names
df[['W','Z']]
Output:
 
type(df['Z'])
Output: pandas.core.series.Series
Creating a new column:
df['new'] = df['W'] + df['Y']
df
Output:
 
#Removing columns
df.drop('new',axis=1)
Output:
 

# Not inplace unless specified
df
Output:
 
df.drop('new',axis=1,inplace=True)
df
Output:
 
df.drop('E',axis=0)
Output:
 
Selecting Rows:
df.loc['C']
Output:
W   -2.018168
X    0.740122
Y    0.528813
Z   -0.589001
Name: C, dtype: float64
df.iloc[2]
Output:
W   -2.018168
X    0.740122
Y    0.528813
Z   -0.589001
Name: C, dtype: float64
df.loc['B','Y']
Output: -0.8480769834036315
df.loc[['A','B'],['W','Y']]
Output:
 
Conditional Selection:
df
Output:
 
df>0
Output:
 



df[df>0]
Output:
 
df[df['W']>0]
Output:
 
df[df['W']>0]['Y']
Output:
A    0.907969
B   -0.848077
D   -0.933237
E    2.605967
Name: Y, dtype: float64
df[df['W']>0][['Y','X']]
Output:
 
df[(df['W']>0) & (df['Y'] > 1)]
Output:
 
More Index Details:

df
Output:
 

# Reset to default 0,1...n index
df.reset_index()
Output:
 


newind = 'CA NY WY OR CO'.split()
df['States'] = newind
df
Output:
 


df.set_index('States')
Output:
 




df.set_index('States',inplace=True)
df
Output:
 











CONCLUSION:
Hence, various python programs to display the functions of dataframes using pandas library have been written, executed and output has been verified. 



7. INTRODUCTION TO PANDAS – MISSING DATA

AIM:
To write a program in python to analyze the missing data of a dataset using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

Missing Data:
Missing Data can occur when no information is provided for one or more items or for a whole unit. Missing Data is a very big problem in real life scenario. Missing Data can also refer to as NA(Not Available) values in pandas. In DataFrame sometimes many datasets simply arrive with missing data, either because it exists and was not collected or it never existed.

PROGRAMS WITH OUTPUT:
import numpy as np
import pandas as pd
df = pd.DataFrame({'A':[1,2,np.nan],
                                 'B':[5,np.nan,np.nan],
                                 'C':[1,2,3]})
df
Output:
 


df.dropna()
Output:
 

df.dropna(axis=1)
Output:
 

df.dropna(thresh=1)
Output:
 

df.fillna(value='FILL VALUE')
Output:
 


df['A'].fillna(value=df['A'].mean())
Output:
0    1.0
1    2.0
2    1.5
Name: A, dtype: float64















CONCLUSION:
Hence, various python programs to analyze the missing data of a dataset using pandas library have been written, executed and output has been verified. 
	


8. INTRODUCTION TO PANDAS – GROUPBY

AIM:
To write a program in python to perform various operations related to groupby() function using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

Groupby:
Pandas groupby method is used to group rows of data together and call aggregate functions. The pandas objects can be split on any of their axes. The abstract definition of grouping is to provide a mapping of labels to group names.
PROGRAMS WITH OUTPUT:

Groupby:
import pandas as pd
# Create dataframe
data = {'Company':['GOOG','GOOG','MSFT','MSFT','FB','FB'],
             'Person':['Sam','Charlie','Amy','Vanessa','Carl','Sarah'],
             'Sales':[200,120,340,124,243,350]}
df = pd.DataFrame(data)
df
Output:
 
#.groupby() method to group rows together based off of a column name
df.groupby('Company')
Output:
 <pandas.core.groupby.generic.DataFrameGroupBy object at 0x0000017D9E1A74C0>
#This object can be saved as a new variable
by_comp = df.groupby("Company")

Aggregate methods:
by_comp.mean()
Output:
 
df.groupby('Company').mean()
Output:
 
by_comp.std()
Output:
 
by_comp.min()
Output:
 
by_comp.max()
Output:
 
by_comp.count()
Output:
 
by_comp.describe()
Output:
 
by_comp.describe().transpose()
Output:
 

by_comp.describe().transpose()['GOOG']
Output:
Sales  count     2.000000
          mean    160.000000
          std           56.568542
          min       120.000000
          25%      140.000000
          50%      160.000000
          75%      180.000000
          max       200.000000
Name: GOOG, dtype: float64



CONCLUSION:
Hence, python programs to perform various operations related to groupby() function using pandas library have been written, executed and output has been verified. 


9. INTRODUCTION TO PANDAS –
MERGING, JOINING, CONCATENATING

AIM:
To write a program in python to perform Merging, Joining and Concatenating among different dataframes using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.
Pandas provides various facilities for easily combining together Series or DataFrame with various kinds of set logic for the indexes and relational algebra functionality in the case of join / merge-type operations.
Concatenation:
Concatenation basically glues together DataFrames. The dimensions should match along the axis concatenating on. pd.concat can be used and passed in a list of DataFrames to concatenate together.
Merging:
The merge function allows you to merge DataFrames together using a similar logic as merging SQL Tables together. 
Joining:
Joining is a convenient method for combining the columns of two potentially differently-indexed DataFrames into a single result DataFrame.
PROGRAMS WITH OUTPUT:
Example DataFrames:
import pandas as pd
df1 = pd.DataFrame({'A': ['A0', 'A1', 'A2', 'A3'],
                                   'B': ['B0', 'B1', 'B2', 'B3'],
                                   'C': ['C0', 'C1', 'C2', 'C3'],
                                   'D': ['D0', 'D1', 'D2', 'D3']},
                                    index=[0, 1, 2, 3])
df2 = pd.DataFrame({'A': ['A4', 'A5', 'A6', 'A7'],
                                   'B': ['B4', 'B5', 'B6', 'B7'],
                                   'C': ['C4', 'C5', 'C6', 'C7'],
                                   'D': ['D4', 'D5', 'D6', 'D7']},
                                    index=[4, 5, 6, 7]) 
df3 = pd.DataFrame({'A': ['A8', 'A9', 'A10', 'A11'],
                                   'B': ['B8', 'B9', 'B10', 'B11'],
                                   'C': ['C8', 'C9', 'C10', 'C11'],
                                   'D': ['D8', 'D9', 'D10', 'D11']},
                                    index=[8, 9, 10, 11])
df1
Output:
 
df2
Output:
 
df3
Output:
 
Concatenation:
pd.concat([df1,df2,df3])
Output:
 
pd.concat([df1,df2,df3],axis=1)
Output:
 
Example DataFrames:
left = pd.DataFrame({'key': ['K0', 'K1', 'K2', 'K3'],
                                   'A': ['A0', 'A1', 'A2', 'A3'],
                                   'B': ['B0', 'B1', 'B2', 'B3']})
right = pd.DataFrame({'key': ['K0', 'K1', 'K2', 'K3'],
                                      'C': ['C0', 'C1', 'C2', 'C3'],
                                      'D': ['D0', 'D1', 'D2', 'D3']})    
left
Output:
 

Right
Output:
 
Merging:
pd.merge(left,right,how='inner',on='key')
Output:
 

left = pd.DataFrame({'key1': ['K0', 'K0', 'K1', 'K2'],
                                   'key2': ['K0', 'K1', 'K0', 'K1'],
                                   'A': ['A0', 'A1', 'A2', 'A3'],
                                   'B': ['B0', 'B1', 'B2', 'B3']})
    
right = pd.DataFrame({'key1': ['K0', 'K1', 'K1', 'K2'],
                                     'key2': ['K0', 'K0', 'K0', 'K0'],
                                     'C': ['C0', 'C1', 'C2', 'C3'],
                                     'D': ['D0', 'D1', 'D2', 'D3']})
pd.merge(left, right, on =['key1', 'key2'])
Output:
 
pd.merge(left, right, how='outer', on=['key1', 'key2'])
Output:
 
pd.merge(left, right, how='right', on=['key1', 'key2'])
Output:
 
pd.merge(left, right, how='left', on=['key1', 'key2'])
Output:
 
Joining:
left = pd.DataFrame({'A': ['A0', 'A1', 'A2'],
                                   'B': ['B0', 'B1', 'B2']},
                                   index=['K0', 'K1', 'K2']) 
right = pd.DataFrame({'C': ['C0', 'C2', 'C3'],
                                     'D': ['D0', 'D2', 'D3']},
                                     index=['K0', 'K2', 'K3'])
left.join(right)
Output:
 
left.join(right, how='outer')
Output:
 
CONCLUSION:
Hence, python programs to perform Merging, Joining and Concatenating among different dataframes using pandas library have been written, executed and output has been verified. 
10. INTRODUCTION TO PANDAS – DF OPERATIONS

AIM:
To write a program in python to perform various Dataframe operations using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

DF Operations:
Using pandas, functions like unique, selecting data, applying function to check the removing a column, sorting in ascending or descending order, null values, fill the null positions, and to find pivot are performed.
PROGRAMS WITH OUTPUT:

import pandas as pd

df = pd.DataFrame({'col1':[1,2,3,4],'col2':[444,555,666,444],'col3':['abc','def','ghi','xyz']})
df.head()
Output:
 

Info on Unique Values:
df['col2'].unique()
Output: array([444, 555, 666], dtype=int64)
df['col2'].nunique()
Output: 3
df['col2'].value_counts()
Output:
444    2
555    1
666    1
Name: col2, dtype: int64

Selecting Data:
#Select from DataFrame using criteria from multiple columns
newdf = df[(df['col1']>2) & (df['col2']==444)]
newdf
Output:
 
Applying Functions:
def times2(x):
    return x*2
df['col1'].apply(times2)
Output:
0    2
1    4
2    6
3    8
Name: col1, dtype: int64


df['col3'].apply(len)
Output:
0    3
1    3
2    3
3    3
Name: col3, dtype: int64
df['col1'].sum()
Output: 10


Permanently Removing a Column:
del df['col1']
df
Output:
 
#Get column and index names
df.columns
Output: Index(['col2', 'col3'], dtype='object')
df.index
Output: RangeIndex(start=0, stop=4, step=1)





Sorting and Ordering a DataFrame:
df
Output:
 
df.sort_values(by='col2') #inplace=False by default
Output:
 
Find or Check for Null Values:
df.isnull()
Output:
 
# Drop rows with NaN Values
df.dropna()
Output:
 
Filling in NaN values:
import numpy as np
df = pd.DataFrame({'col1':[1,2,3,np.nan],
                                 'col2':[np.nan,555,666,444],
                                 'col3':['abc','def','ghi','xyz']})
df.head()
Output:
 
df.fillna('FILL')
Output:
 
data = {'A':['foo','foo','foo','bar','bar','bar'],
            'B':['one','one','two','two','one','one'],
            'C':['x','y','x','y','x','y'],
            'D':[1,3,2,5,4,1]}
df = pd.DataFrame(data)
df
Output:
 
df.pivot_table(values='D',index=['A', 'B'],columns=['C'])
Output:
 















CONCLUSION:
Hence, python programs to perform various Dataframe operations using pandas library have been written, executed and output has been verified. 


11. INTRODUCTION TO PANDAS – 
DATA INPUT AND OUTPUT

AIM:
To write a program in python to get variety of file types using pandas library.
DESCRIPTION:

Introduction to Pandas:
Pandas for data analysis is an extremely powerful version of Excel, and is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.
Data Input and Output:
Pandas can read a variety of file types like csv, excel, html using its pd.read methods
CSV:

Read a comma-separated values (csv) file into DataFrame and also supports optionally iterating or breaking of the file into chunks.
Excel:
Pandas can read, write excel files and only imports data. Formulas or images, having images or macros may cause this read_excel method to crash.
HTML:
For HTML, htmllib5,lxml, and BeautifulSoup4 needs to be installed.
pip install can be used for Anaconda Distribution (or) 

#In your terminal/command prompt run
conda install lxml
conda install html5lib
conda install BeautifulSoup4
#Restart Jupyter Notebook



		
PROGRAMS WITH OUTPUT:
import numpy as np
import pandas as pd
CSV:
CSV Input:
df = pd.read_csv('example')
df
Output:
 
CSV Output:
df.to_csv('example',index=False)
Output:
 
EXCEL:
Excel Input:
pd.read_excel('Excel_Sample.xlsx',sheetname='Sheet1')
Output:
 
Excel Output:
df.to_excel('Excel_Sample.xlsx',sheet_name='Sheet1')
Output:
 
HTML:
HTML Input:
df = pd.read_html('http://www.fdic.gov/bank/individual/failed/banklist.html')
df[0]
Output:
 



ASSIGNMENT:
import pandas as pd
df=pd.read_csv("Salaries.csv - Salaries.csv.csv")
df
1.	Use the .info() method to find out how many entries there are.

df.info()

Output:

<class 'pandas.core.frame.DataFrame'>
RangeIndex: 148654 entries, 0 to 148653
Data columns (total 13 columns):
 #   Column            Non-Null Count   Dtype  
---  ------            --------------   -----  
 0   Id                148654 non-null  int64  
 1   EmployeeName      148654 non-null  object 
 2   JobTitle          148654 non-null  object 
 3   BasePay           148045 non-null  float64
 4   OvertimePay       148650 non-null  float64
 5   OtherPay          148650 non-null  float64
 6   Benefits          112491 non-null  float64
 7   TotalPay          148654 non-null  float64
 8   TotalPayBenefits  148654 non-null  float64
 9   Year              148654 non-null  int64  
 10  Notes             0 non-null       float64
 11  Agency            148654 non-null  object 
 12  Status            0 non-null       float64
dtypes: float64(8), int64(2), object(3)
memory usage: 14.7+ MB

2.	Find the Average Basepay.

df['BasePay'].mean()

Output: 66325.44884050643
3.	Find the highest amount of overtimepay.

df['OvertimePay'].max()

Output: 245131.88

4.	What is the job title of JOSEPH DRISCOLL? Note: Use all caps, otherwise you may get an answer that doesn't match up (there is also a lowercase Joseph Driscoll).

df[df['EmployeeName']=='JOSEPH DRISCOLL']['JobTitle']

Output:

24    CAPTAIN, FIRE SUPPRESSION
Name: JobTitle, dtype: object
5.	How much does JOSEPH DRISCOLL make (including benefits)?

df[df['EmployeeName']=='JOSEPH DRISCOLL']['TotalPayBenefits']

Output:

24    270324.91
Name: TotalPayBenefits, dtype: float64
6.	What is the name of highest paid person (including benefits)?

df[df['TotalPayBenefits']== df['TotalPayBenefits'].max()]['EmployeeName']

Output:

0    NATHANIEL FORD
Name: EmployeeName, dtype: object
7.	What is the name of lowest paid person (including benefits)? Do you notice something strange about how much he or she is paid?

df[df['TotalPayBenefits']== df['TotalPayBenefits'].min()]['EmployeeName']

Output:

148653    Joe Lopez
Name: EmployeeName, dtype: object
8.	What was the average (mean) BasePay of all employees per year? (2011-2014) ?

df.groupby('Year')['BasePay'].mean()
Output:
Year
2011    63595.956517
2012    65436.406857
2013    69630.030216
2014    66564.421924
Name: BasePay, dtype: float64
9.	How many unique job titles are there?[nunique operation]

df['JobTitle'].nunique()

Output: 2159
10.	How many people have the word Chief in their job title?

def chief(values):
    x=values.str.lower()
    count=x.str.contains('chief').value_counts()
    print(count)
chief(df['JobTitle'])

Output:

False    148027
True        627
Name: JobTitle, dtype: int64









CONCLUSION:
Hence, python programs to get variety of file types using pandas library have been written, executed and output has been verified. 



12. INTRODUCTION TO MATPLOTLIB

AIM:
To create and customize plots in python using matplotlib, including how to create different types of plots and customize plot colors and labels.
DESCRIPTION:
Matplotlib is an excellent 2D and 3D graphics library for generating scientific figures.
Some of the major Pros of Matplotlib are:
•	Generally easy to get started for simple plots
•	Support for custom labels and texts
•	Great control of every element in a figure
•	High-quality output in many formats
•	Very customizable in general
Matplotlib is used to create reproducible figures programmatically. 
Figure size, aspect ratio and DPI:
Matplotlib allows the aspect ratio, DPI and figure size to be specified when the Figure object is created. 
* figsize is a tuple of the width and height of the figure in inches 
* dpi is the dots-per-inch (pixel per inch).
Saving figures:
Matplotlib can generate high-quality output in a number formats, including PNG, JPG, EPS, SVG, PGF and PDF.
To save a figure to a file, savefig method is used in the Figure class.
Legends, labels and titles:
Figure titles:
A title can be added to each axis instance in a figure. To set the title, the set_title method in the axes instance is used.
Axis labels:
Similarly, with the methods set_xlabel and set_ylabel, we can set the labels of the X and Y axes.
Legends:
The label="label text" keyword argument is used when plots or other objects are added to the figure, and the legend method is used without arguments to add the legend to the figure.
The legend function takes an optional keyword argument loc that can be used to specify where in the figure the legend is to be drawn. The allowed values of loc are numerical codes for the various places the legend can be drawn. 
Setting colors, linewidths, linetypes:
Colors with MatLab like syntax:
With matplotlib, the colors of lines and other graphical elements can be explained in a number of ways. MATLAB-like syntax is used where 'b' means blue, 'g' means green, etc. 
The MATLAB API for selecting line styles are also supported: where, for example, 'b.-' means a blue line with dots.
Colors with the color= parameter:
Colors can be defined by their names or RGB hex codes and optionally provide an alpha value using the color and alpha keyword arguments. Alpha indicates opacity.
Line and marker styles:
To change the line width, the linewidth or lw keyword argument is used. The line style can be selected using the linestyle or ls keyword arguments.
Control over axis appearance:
Plot range:
The ranges of the axes can be configured using the set_ylim and set_xlim methods in the axis object, or axis('tight') for automatically getting "tightly fitted" axes ranges.
PROGRAMS WITH OUTPUT:
import matplotlib.pyplot as plt
#This line helps to see plots in the notebook
%matplotlib inline
Basic Example:
import numpy as np
x = np.linspace(0, 5, 11)
y = x ** 2
x
Output:
array([0. , 0.5, 1. , 1.5, 2. , 2.5, 3. , 3.5, 4. , 4.5, 5. ])
y
Output:
array([ 0.  ,  0.25,  1.  ,  2.25,  4.  ,  6.25,  9.  , 12.25, 16.  , 20.25, 25.  ])
Basic Matplotlib Commands:
#Basic Matplotlib Commands
plt.plot(x, y, 'r') # 'r' is the color red
plt.xlabel('X Axis Title Here')
plt.ylabel('Y Axis Title Here')
plt.title('String Title Here')
plt.show()
 

Creating Multiplots on Same Canvas:
# plt.subplot(nrows, ncols, plot_number)
plt.subplot(1,2,1)
plt.plot(x, y, 'r-') # More on color options later
plt.subplot(1,2,2)
plt.plot(y, x, 'g*-');
 
# Creates blank canvas
fig = plt.figure()

axes1 = fig.add_axes([0.1, 0.1, 0.8, 0.8]) # main axes
axes2 = fig.add_axes([0.2, 0.5, 0.4, 0.3]) # inset axes

# Larger Figure Axes 1
axes1.plot(x, y, 'b')
axes1.set_xlabel('X_label_axes2')
axes1.set_ylabel('Y_label_axes2')
axes1.set_title('Axes 2 Title')

# Insert Figure Axes 2
axes2.plot(y, x, 'r')
axes2.set_xlabel('X_label_axes2')
axes2.set_ylabel('Y_label_axes2')
axes2.set_title('Axes 2 Title');
 
subplots():
#The plt.subplots() object will act as a more automatic axis manager.
# Use similar to plt.figure() except use tuple unpacking to grab fig and axes
fig, axes = plt.subplots()

# Now use the axes object to add stuff to plot
axes.plot(x, y, 'r')
axes.set_xlabel('x')
axes.set_ylabel('y')
axes.set_title('title');
 
#Then you can specify the number of rows and columns when creating the subplots() object
# Empty canvas of 1 by 2 subplots
fig, axes = plt.subplots(nrows=1, ncols=2)
 

# Axes is an array of axes to plot on
axes
Output:
array([<matplotlib.axes._subplots.AxesSubplot object at 0x000001BDAE69A5C0>,
       <matplotlib.axes._subplots.AxesSubplot object at 0x000001BDAE6C1550>],
      dtype=object)




#We can iterate through this array:
for ax in axes:
    ax.plot(x, y, 'b')
    ax.set_xlabel('x')
    ax.set_ylabel('y')
    ax.set_title('title')
# Display the figure object    
fig
 
#A common issue with matplolib is overlapping subplots or figures. We can use fig.tight_layout() or plt.tight_layout() method, which automatically adjusts the positions of the axes on the figure canvas so that there is no overlapping content.
fig, axes = plt.subplots(nrows=1, ncols=2)
for ax in axes:
    ax.plot(x, y, 'g')
    ax.set_xlabel('x')
    ax.set_ylabel('y')
    ax.set_title('title')
fig    
plt.tight_layout()
 
Figure size, aspect ratio and DPI:
fig = plt.figure(figsize=(8,4), dpi=100)
Output:
<Figure size 800x400 with 0 Axes>
#The same arguments can also be passed to layout managers, such as the subplots function
fig, axes = plt.subplots(figsize=(12,3))

axes.plot(x, y, 'r')
axes.set_xlabel('x')
axes.set_ylabel('y')
axes.set_title('title');
 
Saving figures:
fig.savefig("filename.png")
#Here we can also optionally specify the DPI and choose between different output formats
fig.savefig("filename.png", dpi=200)
Legends, labels and titles:
Figure titles:
ax.set_title("title");
Axis labels:
ax.set_xlabel("x")
ax.set_ylabel("y");
Legends:
fig = plt.figure()
ax = fig.add_axes([0,0,1,1])
ax.plot(x, x**2, label="x**2")
ax.plot(x, x**3, label="x**3")
ax.legend()
 
# legend overlaps some of the actual plot.

ax.legend(loc=1) # upper right corner
ax.legend(loc=2) # upper left corner
ax.legend(loc=3) # lower left corner
ax.legend(loc=4) # lower right corner
ax.legend(loc=0) # let matplotlib decide the optimal location
fig
 
Setting colors, linewidths, linetypes:
Colors with MatLab like syntax:
# MATLAB style line color and style 
fig, ax = plt.subplots()
ax.plot(x, x**2, 'b.-') # blue line with dots
ax.plot(x, x**3, 'g--') # green dashed line
 
Colors with the color= parameter:
fig, ax = plt.subplots()
ax.plot(x, x+1, color="blue", alpha=0.5) # half-transparant
ax.plot(x, x+2, color="#8B008B")        # RGB hex code
ax.plot(x, x+3, color="#FF8C00")        # RGB hex code 
 


Line and marker styles:
fig, ax = plt.subplots(figsize=(12,6))

ax.plot(x, x+1, color="red", linewidth=0.25)
ax.plot(x, x+2, color="red", linewidth=0.50)
ax.plot(x, x+3, color="red", linewidth=1.00)
ax.plot(x, x+4, color="red", linewidth=2.00)

# possible linestype options ‘-‘, ‘–’, ‘-.’, ‘:’, ‘steps’
ax.plot(x, x+5, color="green", lw=3, linestyle='-')
ax.plot(x, x+6, color="green", lw=3, ls='-.')
ax.plot(x, x+7, color="green", lw=3, ls=':')

# custom dash
line, = ax.plot(x, x+8, color="black", lw=1.50)
line.set_dashes([5, 10, 15, 10]) # format: line length, space length, ...

# possible marker symbols: marker = '+', 'o', '*', 's', ',', '.', '1', '2', '3', '4', ...
ax.plot(x, x+ 9, color="blue", lw=3, ls='-', marker='+')
ax.plot(x, x+10, color="blue", lw=3, ls='--', marker='o')
ax.plot(x, x+11, color="blue", lw=3, ls='-', marker='s')
ax.plot(x, x+12, color="blue", lw=3, ls='--', marker='1')

# marker size and color
ax.plot(x, x+13, color="purple", lw=1, ls='-', marker='o', markersize=2)
ax.plot(x, x+14, color="purple", lw=1, ls='-', marker='o', markersize=4)
ax.plot(x, x+15, color="purple", lw=1, ls='-', marker='o', markersize=8, markerfacecolor="red")
ax.plot(x, x+16, color="purple", lw=1, ls='-', marker='s', markersize=8, 
        markerfacecolor="yellow", markeredgewidth=3, markeredgecolor="green");
 
Control over axis appearance:
Plot range:
fig, axes = plt.subplots(1, 3, figsize=(12, 4))

axes[0].plot(x, x**2, x, x**3)
axes[0].set_title("default axes ranges")

axes[1].plot(x, x**2, x, x**3)
axes[1].axis('tight')
axes[1].set_title("tight axes")

axes[2].plot(x, x**2, x, x**3)
axes[2].set_ylim([0, 60])
axes[2].set_xlim([2, 5])
axes[2].set_title("custom axes range");
 
Special Plot Types:
plt.scatter(x,y)
 
from random import sample
data = sample(range(1, 1000), 100)
plt.hist(data)
Output:
(array([12., 11.,  8., 10., 10.,  8., 12.,  8., 10., 11.]),
 array([  6. , 104.3, 202.6, 300.9, 399.2, 497.5, 595.8, 694.1, 792.4,
        890.7, 989. ]),
 <a list of 10 Patch objects>)
 

data = [np.random.normal(0, std, 100) for std in range(1, 4)]
# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=True);   
 


Exercise:Visualizing Titanic dataset
Step1:Import necessary libraries
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
Step2:Read the dataset
data=pd.read_csv("Titanic")
data.head()
 
Step3:Set Passengerid as the index
data.set_index("PassengerId").head()
 
Step4:Visualization
Line Graph-Age:
plt.figure(figsize=(14,6))
plt.title('Line Graph-age')
plt.plot(data['Age'])
 
Barchart-Survived:
data['Survived'].value_counts().plot(kind='bar')
plt.xlabel('Survived')
plt.ylabel('Frequency')
plt.title('Barchart-Survived')
plt.legend()
 
Histogram-Age:
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.title('Histogram of age')
plt.hist(data['Age'])
 
Scatterplot-Fare:
plt.scatter(data.Age,data.Fare)
plt.xlabel('Age')
plt.ylabel('Fare')
plt.title('Scatterplot-Fare')
 
Piechart for presenting male/female proportion:
Males=(data['Sex']=='male').sum()
Females=(data['Sex']=='female').sum()
Gender=[Males,Females]
plt.title("Sex Proportion")
plt.pie(Gender,colors=['blue','red'],labels=['Males','Females'],
        #with the start angle at 90%
        startangle=90,
        #with one slide exploded out
        explode=[0.15,0],
        #with the percent listed as fraction
        autopct='%1.1f%%')
 





CONCLUSION
Hence, various plots have been created and customized using matplotlib.


13. DATA VISUALIZATION USING SEABORN 

AIM:
To create and visualize various plots in python using seaborn.
DESCRIPTION:
Seaborn is a library for making statistical graphics in Python. It is built on top of matplotlib and closely integrated with pandas data structures.

Seaborn aims to make visualization a central part of exploring and understanding data. Its dataset-oriented plotting functions operate on dataframes and arrays containing whole datasets and internally perform the necessary semantic mapping and statistical aggregation to produce informative plots.
PLOT TYPES:
Lineplot:
A Line plot is a graph that shows frequency of data along a number line.
Distplot:
Flexibly plot a univariate distribution of observations.
Jointplot:
Seaborn’s  Jointplot displays a relationship between 2 variables (bivariate) as well as 1D profiles (univariate) in the margins.
Lmplot:
The Lmplot plot shows the line along with datapoints on the 2d space. By specifying x and y you can set the horizontal and vertical labels respectively.
Barplot:
These very similar plots allow you to get aggregate data off a categorical feature in your data. Barplot is a general plot that allows you to aggregate the categorical data based off some function, by default the mean.
Countplot:
This is essentially the same as Barplot except the estimator is explicitly counting the number of occurrences which is why we only pass the x value:



Boxplot and Violinplot:
Boxplots and Violinplots are used to show the distribution of categorical data. A Box plot (or Box-and-Whisker plot) shows the distribution of quantitative data in a way that facilitates comparisons between variables or across levels of a categorical variable. The box shows the quartiles of the dataset while the whiskers extend to show the rest of the distribution, except for points that are determined to be “outliers” using a method that is a function of the inter-quartile range.
A Violin plot plays a similar role as a box and whisker plot. It shows the distribution of quantitative data across several levels of one (or more) categorical variables such that those distributions can be compared. Unlike a Box plot, in which all of the plot components correspond to actual datapoints, the violin plot features a kernel density estimation of the underlying distribution.
Stripplot and Swarmplot:
The Stripplot will draw a scatterplot where one variable is categorical. A Strip plot can be drawn on its own, but it is also a good complement to a box or violin plot in cases where you want to show all observations along with some representation of the underlying distribution.
The Swarmplot is similar to Stripplot, but the points are adjusted (only along the categorical axis) so that they don’t overlap. This gives a better representation of the distribution of values, although it does not scale as well to large numbers of observations (both in terms of the ability to show all the points and in terms of the computation needed to arrange them).
Factorplot:
Factorplot is the most general form of a categorical plot. It can take in a kind parameter to adjust the plot type.
Pairplot:
Pair Plot ia a simple way to visualize relationships between each variable. It produces a matrix of relationships between each variable for instant examination of data. It can also be used for determining types of regression analysis to use.
Heatmap:
Heat maps display numeric tabular data where the cells are colored depending upon the contained value. Heat maps are great for making trends in this kind of data more readily apparent, particularly when the data is ordered and there is clustering.





PROGRAMS WITH OUTPUT:
#Import libraries and read the dataset
import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
tips = sns.load_dataset('tips')
tips.head()
 
Lineplot:
sns.lineplot(data=tips['size'],label='size')
 






Distplot:
sns.distplot(tips['size'],label="size")
 
Jointplot:
sns.jointplot(tips['total_bill'],tips['tip'])
 
Lmplot:
sns.lmplot(x='total_bill',y='tip',data=tips)
 
Barplot:
sns.barplot(x='sex',y='total_bill',data=tips)
 
#You can change the estimator object to your own function, that converts a vector to a scalar:
sns.barplot(x='sex',y='total_bill',data=tips,estimator=np.std)
 
Countplot:
sns.countplot(x='sex',data=tips)
 
Boxplot:
sns.boxplot(x="day", y="total_bill", data=tips,palette='rainbow')
 

# Can do entire dataframe with orient='h'
sns.boxplot(data=tips,palette='rainbow',orient='h')
 
sns.boxplot(x="day", y="total_bill", hue="smoker",data=tips, palette="coolwarm")
 
Violinplot:
sns.violinplot(x="day", y="total_bill", data=tips,palette='rainbow')
 
sns.violinplot(x="day", y="total_bill", data=tips,hue='sex',palette='Set1')
 
sns.violinplot(x="day", y="total_bill", data=tips,hue='sex',split=True,palette='Set1')
 
Stripplot: 
sns.stripplot(x="day", y="total_bill", data=tips)
 
sns.stripplot(x="day", y="total_bill", data=tips,jitter=True)
 
sns.stripplot(x="day", y="total_bill", data=tips,jitter=True,hue='sex',palette='Set1')
 
sns.stripplot(x="day", y="total_bill", data=tips,jitter=True,hue='sex',palette='Set1',split=True)
 
Swarmplot:
sns.swarmplot(x="day", y="total_bill", data=tips)
 

sns.swarmplot(x="day", y="total_bill",hue='sex',data=tips, palette="Set1", split=True)
 
Combining Categorical Plots:
sns.violinplot(x="tip", y="day", data=tips,palette='rainbow')
sns.swarmplot(x="tip", y="day", data=tips,color='black',size=3)
 
Factorplot:
sns.factorplot(x='sex',y='total_bill',data=tips,kind='bar')
 
Pairplot:
sns.pairplot(tips,hue='sex')
 







Heatmap:
plt.figure(figsize=(14,10))
sns.heatmap(tips[['tip','size']])
 

CONCLUSION
Hence, various plots have been created and visualized using seaborn.




14. PLOTLY AND CUFFLINKS

AIM:
To write a program in python to create an interactive visualization with plotly and Cufflinks.

DESCRIPTION:

Plotly is a library used to create interactive plots which can be used in dashboards or websites. They can be saved as html files or static images.

The plotly Python library is an interactive, open-source plotting library that supports over 40 unique chart types covering a wide range of statistical, financial, geographic, scientific, and 3-dimensional use-cases.

PROGRAMS WITH OUTPUT:

Import Libraries:
import plotly
import cufflinks as cf
import pandas as pd
import numpy as np
#To display the plots
%matplotlib inline
#Enabling the offline mode for interactive plotting locally
from plotly.offline import download_plotlyjs,init_notebook_mode,plot,iplot
init_notebook_mode(connected=True)
cf.go_offline()






Read data:
df=pd.read_csv("PRICE.csv")
df
Output:
 
Simple Plot:
#The plots are marked in the manner of dataset(based on the index)
df.iplot()
Output:
 

Scatter Plot:
#The plots are marked in the manner of dataset(based on the index)
#Markers need to be specified else line will be taken as default
df[['carlength','carwidth','carheight','price']].iplot(kind = 'scatter' , mode = 'markers')
Output:
 

#x and y are specified
df.iplot(kind='scatter',x='carlength',y='price',mode='markers',size=10)
Output:
 
Bar Plots:
df.iplot(kind='bar',x='Affordable',y='price')
Output:
 
#Gives the count of each data
df.count().iplot(kind='bar')
Output:
 
#Gives horizontal view
df.count().iplot(kind='barh')
Output:
 
Boxplots:
df.iplot(kind='box')
Output:
 
3d Surfaceplot:
#gives 3d view of x, y and z axis
df[['carlength','price','carheight']].iplot(kind = 'surface', colorscale = 'rdylbu')
Output:
 
Spreadplot:
#Shows the spread between two or more than numerical columns at any particular point.
#Gives the difference between the two values (i.e) spread
df[['carlength','carheight']].iplot(kind='spread')
Output:
 
Histogram:
#Bins to specify the quantity of distribution buckets.
df['price'].iplot(kind='hist',bins=25)
Output:
 
Bubbleplot:
df.iplot(kind='bubble',x='carlength',y='carheight',size='price')
Output:
 
scatter_matrix():
#Similar to sns.pairplot()
df.scatter_matrix()
Output:
 
CONCLUSION:
Hence, python programs to create an interactive visualization with plotly and Cufflinks have been executed and output has been verified. 

15. FOLIUM

AIM:
To write a program in python to create a map leaflet using folium.
DESCRIPTION:

Folium helps to visualize the coordinates of a area along with measures.
It makes it easy to visualize data that’s been manipulated in Python on an interactive Leaflet map. It enables both the binding of data to a map for choropleth visualizations as well as passing Vincent/Vega visualizations as markers on the map.
PROGRAMS WITH OUTPUT:

import numpy as np
import pandas as pd
import folium
district_wise_census = pd.read_csv("districtwise_population_and_centroids")
district_wise_census.head()
Output:
 
surat_city_long = district_wise_census[district_wise_census["District"] == "Surat"].Longitude.values[0]
surat_city_lat = district_wise_census[district_wise_census["District"] == "Surat"].Latitude.values[0]
m = folium.Map(location=[surat_city_lat, surat_city_long])
m



Output:
 
state_wise_centroid = pd.read_csv("statewise_centroids_2011")
state_wise_centroid.head()
Output:
 
state_wise_census = district_wise_census.groupby(by="State").sum()[["Population in 2001","Population in 2011"]].reset_index()
state_wise_census.head()
Output:
 
state_wise_centroid.head()
Output:
 
state_wise_census = state_wise_centroid.merge(state_wise_census, left_on="State", right_on="State")
state_wise_census
Output:
 
center_lat = state_wise_census.mean().Latitude
center_long = state_wise_census.mean().Longitude
m = folium.Map(location=[center_lat, center_long], zoom_start=4.5)
for state in state_wise_census["State"].unique():
    state_census = state_wise_census[state_wise_census["State"]==state]
    folium.CircleMarker(
        location=[state_census.Latitude.values[0], state_census.Longitude.values[0]],       
        radius = float(state_census["Population in 2011"].values[0]/1e7),
        popup="Population 2011 : %s"%state_census["Population in 2011"].values[0],
        tooltip = state_census.State.values[0],
        color="black",
        fill_color="black"
    ).add_to(m)

m
Output:
 



CONCLUSION:
Hence, python program to create a map leaflet using folium has been executed and output has been verified. 


16. INSTALLATION OF PYSPARK

AIM: 
To install PySpark and to run PySpark on jupyter notebook.

DESCRIPTION:
PySpark has been released in order to support the collaboration of Apache Spark(written in Scala programming language) and Python, it actually is a Python API for Spark. PySpark also helps to  interface with Resilient Distributed Datasets (RDDs) in Apache Spark and Python programming language. 
PySparkSQL:
A PySpark library used to apply SQL-like analysis on a huge amount of structured or semi-structured data. SQL queries can also be used along with PySparkSQL. It can also be connected to Apache Hive. HiveQL can be also be applied. PySparkSQL is a wrapper over the PySpark core. PySparkSQL introduced the DataFrame, a tabular representation of structured data that is similar to that of a table from a relational database management system.
PROGRAMS WITH OUTPUT:

A.	Needed resources:

1.	Spark distribution from spark.apache.org
 

2.	 Python and Jupyter Notebook - by installing the Python 3.x version of Anaconda distribution.

3.	winutils.exe — a Hadoop binary for Windows — from Steve Loughran’s GitHub repo. 
From the corresponding Hadoop version in the Spark distribution, from winutils.exe under /bin. https://github.com/steveloughran/winutils/blob/master/hadoop-2.7.1/bin/winutils.exe 
 

4.	The findspark Python module, which can be installed by running python -m pip install findspark either in Windows command prompt or Git bash if Python is installed. Command prompt is searched by typing cmd in the search box.

 

5.	If Java is not available or if Java version is 7.x or less, the latest JDK (current version 9.0.1) can be downloaded and installed from Oracle. 
 

6.	To unpack the .tgz file on Windows 7-zip can be by downloaded and installed on Windows
      To unpack the .tgz file from Spark distribution, right-click on the file icon and   
      select 7-zip > Extract Here.
 
B.	Installing PySpark:
1.	Unpack the .tgz file put under D:\spark\spark-2.2.1-bin-hadoop2.7
 
2.	Move the winutils.exe downloaded from step A3 to the \bin folder of Spark distribution. D:\spark\spark-2.2.1-bin-hadoop2.7\bin\winutils.exe
3.	Add environment variables: Enables Windows to find where the files are when we PySpark kernel gets started. It can be done by finding the environment variable settings by putting “environ…” in the search box.
Name	Value
SPARK_HOME	D:\spark\spark-2.2.1-bin-hadoop2.7
HADOOP_HOME	D:\spark\spark-2.2.1-bin-hadoop2.7
PYSPARK_DRIVER_PYTHON	jupyter
PYSPARK_DRIVER_PYTHON_OPTS	notebook

 

4.	In the same environment variable settings window, under the Path or PATH variable, edit is clicked and D:\spark\spark-2.2.1-bin-hadoop2.7\bin is added  to it.
      In Path  semicolon ; is used to separate the values.
 



5.	Add  the installed Java JDK folder from step A5, 
D:\Program Files\Java\jdk1.8.0_121

Name	Value
JAVA_HOME	D:\Progra~1\Java\jdk1.8.0_121
               
                   If JDK is installed under \Program Files (x86), Progra~1 part is replaced  
                   by Progra~2 instead. 

C.	Running PySpark in Jupyter Notebook:

Open a Python 3 notebook from Jupyter.
 

#Following code is run:
import findspark 
findspark.init()
# only run after findspark.init()
import pyspark
from pyspark.sql import SparkSession 
spark = SparkSession.builder.getOrCreate()
df = spark.sql('''select 'spark' as hello ''')
df.show()

When run, a Windows firewall pop-up will appear which can be cancelled.  

Output:
 

CONCLUSION:
Hence, PySpark has been installed successfully and has been tested using Jupyter notebook.



17. INTRODUCTION TO HDF5_PYTABLE

AIM: 
To define own records in Python and save collections of them (i.e. a table) into a file.

DESCRIPTION:

Hierarchical Data Format (HDF) is a specification and technology for the storage of big numerical data. HDF was created in the supercomputing community and is now an open standard. The latest version of HDF is HDF5. HDF5 structures data in groups and datasets. Datasets are multidimensional homogeneous arrays. Groups can contain other groups or datasets. Groups are like directories in a hierarchical filesystem.
The two main HDF5 Python libraries are:
1.	h5y
2.	PyTables
PyTables has a number of dependencies:
1.	NumPy
2.	Numexpr - This package claims that it evaluates multiple-operator array expressions  
                    many times faster than NumPy can.
3.	HDF5
The HDFStore class is the pandas abstraction responsible for dealing with HDF5 data. 

Importing tables objects:
Public objects in the tables package needs to be imported first. However, PyTables has a contained set of first-level primitives, which can be considered as an alternative. If NumPy arrays are used, functions from the numpy package needs to be imported.
Declaring a Column Descriptor:
If a particle detector is available and in order to create a table object for saving data retrieved from it, a table needs to be defined along with number of columns and the kind of object is contained in each column. 
Particle detector has a TDC (Time to Digital Converter) counter with a dynamic range of 8 bits and an ADC (Analogical to Digital Converter) with a range of 16 bits. For these values, 2 fields are defined in the record object called TDCcount and ADCcount. To save the grid position in which the particle has been detected, two new fields called grid_i and grid_j are added. Instrumentation can also obtain pressure and energy of the particle. 
The resolution of the pressure-gauge uses a single-precision float to store pressure readings, while the energy value will need a double-precision float. Finally, to track the particle, a name is assigned to identify the kind of the particle it is along with a unique numeric identifier is given. Hence, two more fields are added:
1.	name           -    string of up to 16 characters
2.	idnumber  -   an integer of 64 bits (which allows to store records for extremely large   
                         numbers of particles). 
A new Particle class that will contain all the above information is declared for each field which is needed along with its value to which an instance of the appropriate Col subclass is assigned, according to the kind of column defined (the data type, the length, the shape, etc). Hence, this Particle instance can be used as a descriptor for the detector data table. 
Creating a PyTables file: 
The top-level open_file() function is used to create a PyTables file. open_file() is one of the objects imported by the `from tables import *` statement. This function attempts to open the file, and if successful, returns the File object instance h5file. The root of the object tree is specified in the instance’s root attribute. 
Creating a new group:
A group called detector is created that branches from the root node. The particle data table is saved in the group. This function creates a new Group object instance that will be assigned to the variable group.
Creating a new table: 
A Table object is created as a branch off the newly-created group using File.create_table() method of the h5file object. Hence, a new Table instance is created and assigned to the variable table. 
More detailed information can be displayed about the objects and their children by just printing them leading to that introspection capability to be very useful. 
The row attribute of table points to the Row instance that will be used to write data rows into the table. A data is written simply by assigning the Row instance, the values for each row as if it were a dictionary (although it is actually an extension class), using the column names as keys. 
Flushing:
After all data have been processed, the table’s I/O buffer needs to flushed if all this data needs to be written to disk which is achieved by calling the table.flush() method. Flushing is a very important step as it will not only help to maintain the integrity of file, but also will free valuable memory resources (i.e. internal buffers) that the program may need for other things.



Reading (and selecting) data in a table:
This task helps to access the data and select from specific columns the values needed. The first line creates a “shortcut” to the readout table deeper on the object tree. The natural naming schema is used to access it. 
PyTables do offer other, more powerful ways of performing selections which may be more suitable for very large tables or if a very high query speed is needed. They are called inkernel and indexed queries, which can be used through Table.where() and other related methods. 
In-kernel and indexed queries are not only faster, but also, they look more compact, and are among the greatest features for PyTables.
Closing the file:
The close method of the h5file File object is used to close the file before exiting Python. Hence, a PyTables file with a table and two arrays have been created which can be examined with any generic HDF5 tool, such as h5dump or h5ls. 
PROGRAMS WITH OUTPUT:

Importing tables objects:
#Import packages
conda install -c anaconda hdf5
pip install numexpr
pip install tables
import numpy as np
import h5pymatrix1 = np.random.random(size=(1000,1000))
matrix2 = np.random.random(size=(1000,100))
with h5py.File("I:\\hdf5_data.h5","w") as hdf:
     hdf.create_dataset('dataset1',data=matrix1)
     hdf.create_dataset('dataset2',data=matrix2)
#Reading the hdf5
with h5py.File("I:\\hdf5_data.h5","r") as hdf:
      ls=list(hdf.keys())
      print("List of datasets in this file ",ls)
      data = hdf.get('dataset1')
      dataset1=np.array(data)
      print("Shape of dataset ",dataset1.shape)
Output:
List of datasets in this file  ['dataset1', 'dataset2']
Shape of dataset  (1000, 1000)
 

Declaring a Column Descriptor:
from tables import *

class Particle(IsDescription):
    name      = StringCol(16)  	  # 16-character String
    idnumber  = Int64Col()    	  # Signed 64-bit integer
    ADCcount  = UInt16Col()    # Unsigned short integer
    TDCcount  = UInt8Col()      # unsigned byte
    grid_i    = Int32Col()    	  # 32-bit integer
    grid_j    = Int32Col()     	  # 32-bit integer
    pressure  = Float32Col()  	  # float  (single-precision)
    energy    = Float64Col()    	  # double (double-precision)
Creating a PyTables file: 
# Tto create a new file in the current working directory called “tutorial2.h5” in “w”rite mode and with a descriptive title string (“Test file”). 
h5file = open_file("tutorial2.h5", mode="w", title="Test file")
Creating a new group:
#The File instance h5fileis taken and invoked its File.create_group() method to create a new group called detector branching from ”/” .
group = h5file.create_group("/", 'detector', 'Detector information')
Creating a new table: 
# Node name “readout” is assigned to this table. 
# The Particle class declared before is the description parameter (to define the columns of the table) 
#  “Readout example” is set as the Table title. 
table = h5file.create_table(group, 'readout',Particle, "Readout example")
#  To examine the object tree, print the File instance variable h5file
# Dump of the object tree would be displayed and the Group and Table objects which are created can be easily seen
print(h5file)
Output:
tutorial2.h5 (File) 'Test file'
Last modif.: 'Wed Dec  2 10:46:38 2020'
Object Tree: 
/ (RootGroup) 'Test file'
/detector (Group) 'Detector information'
/detector/readout (Table(0,)) 'Readout example'
# For more information
h5file
Output:
File(filename=tutorial2.h5, title='Test file', mode='w', root_uep='/', filters=Filters(complevel=0, shuffle=False, bitshuffle=False, fletcher32=False, least_significant_digit=None))
/ (RootGroup) 'Test file'
/detector (Group) 'Detector information'
/detector/readout (Table(0,)) 'Readout example'
  description := {
  "ADCcount": UInt16Col(shape=(), dflt=0, pos=0),
  "TDCcount": UInt8Col(shape=(), dflt=0, pos=1),
  "energy": Float64Col(shape=(), dflt=0.0, pos=2),
  "grid_i": Int32Col(shape=(), dflt=0, pos=3),
  "grid_j": Int32Col(shape=(), dflt=0, pos=4),
  "idnumber": Int64Col(shape=(), dflt=0, pos=5),
  "name": StringCol(itemsize=16, shape=(), dflt=b'', pos=6),
  "pressure": Float32Col(shape=(), dflt=0.0, pos=7)}
  byteorder := 'little'
  chunkshape := (1394,)

# To get  pointer to the Row instance of this table instance
particle = table.row
# To write rows
for i in range(10):
    particle['name']  = 'Particle: %6d' % (i)
    particle['TDCcount'] = i % 256
    particle['ADCcount'] = (i * 256) % (1 << 16)
    particle['grid_i'] = i
    particle['grid_j'] = 10 - i
    particle['pressure'] = float(i*i)
    particle['energy'] = float(particle['pressure'] ** 4)
    particle['idnumber'] = i * (2 ** 34)
    # Insert a new particle record
    particle.append()


Flushing:
table.flush()

Reading (and selecting) data in a table:
# Creates a “shortcut” to the readout table deeper on the object tree
table = h5file.root.detector.readout

# Loops over the rows in table as they are provided by the Table.iterrows() iterator
# The iterator returns values until all the data in table is exhausted.
pressure = [x['pressure'] for x in table.iterrows() if x['TDCcount'] > 3 and 20 <= x['pressure'] < 50]
pressure
Output:
[25.0, 36.0, 49.0]

# Using an in-kernel selection to query the name column for the same set of cuts
names = [ x['name'] for x in table.where("""(TDCcount > 3) & (20 <= pressure) & (pressure < 50)""") ]
names
Output:
[b'Particle:      5', b'Particle:      6', b'Particle:      7']


Closing the file:
h5file.close()
h5file_Emp.close()





EXAMPLE:
class Employee(IsDescription):
    name      = StringCol(16)   # 16-character String
    idnumber  = Int64Col()      # Signed 64-bit integer
  
# h5file_Emp = tables.open_file("Emp4.h5", mode="w", title="Emp file")
h5file_Emp = open_file("Emp5.h5", mode="w", title="Emp file")
 


group1 = h5file_Emp.create_group("/", 'GV', 'SRM')
#table = h5file.create_table(group, 'readout',Particle, "Readout example")
table_Emp = h5file_Emp.create_table(group1, 'Emp5',Employee, "EmployeeData")

print(h5file_Emp)
Output:
Emp5.h5 (File) 'Emp file'
Last modif.: 'Wed Dec  2 10:53:55 2020'
Object Tree: 
/ (RootGroup) 'Emp file'
/GV (Group) 'SRM'
/GV/Emp5 (Table(0,)) 'EmployeeData'
h5file_Emp
Output:
File(filename=Emp5.h5, title='Emp file', mode='w', root_uep='/', filters=Filters(complevel=0, shuffle=False, bitshuffle=False, fletcher32=False, least_significant_digit=None))
/ (RootGroup) 'Emp file'
/GV (Group) 'SRM'
/GV/Emp5 (Table(0,)) 'EmployeeData'
  description := {
  "idnumber": Int64Col(shape=(), dflt=0, pos=0),
  "name": StringCol(itemsize=16, shape=(), dflt=b'', pos=1)}
  byteorder := 'little'
  chunkshape := (2730,)




emprow = table_Emp.row
for i in range(10):
    emprow['name']  = i
    emprow['idnumber'] = i
    emprow.append()
table_Emp.flush()
table_Emp = h5file_Emp.root.GV.Emp5
table_Emp
Output:
/GV/Emp5 (Table(10,)) 'EmployeeData'
  description := {
  "idnumber": Int64Col(shape=(), dflt=0, pos=0),
  "name": StringCol(itemsize=16, shape=(), dflt=b'', pos=1)}
  byteorder := 'little'
  chunkshape := (2730,)

names = [ x['name'] for x in table_Emp.where("""(idnumber > 3) """) ]
names
Output:
[b'4', b'5', b'6', b'7', b'8', b'9']
h5file_Emp.close()




CONCLUSION:
Hence, records in Python have been defined and saved into a file using PyTable.


18. INTRODUCTION TO PYSTORE

AIM: 
To understand and execute the basics of PyStore.

DESCRIPTION:

PyStore, a fast data store for Pandas timeseries data, is a simple (yet powerful) datastore for Pandas dataframes, and while it can store any Pandas object, it was designed with storing timeseries data in mind.
It’s built on top of Pandas, Numpy, Dask, and Parquet (via Fastparquet) in a hierarchical directory structure, to provide an easy to use, fast, powerful, and pythonic datastore for Pandas dataframes that can easily query millions of rows in sub-second speed. Files are compressed using Snappy, a fast and efficient compression/decompression library from Google.
 Dask can create DataFrames from various data storage formats like CSV, HDF, Apache Parquet, and others. For most formats, this data can live on various storage systems including local disk, network file systems (NFS), the Hadoop File System (HDFS), and Amazon’s S3 (excepting HDF, which is only available on POSIX like file systems).
Snappy (previously known as Zippy) is a fast data compression and decompression library written in C++ by Google based on ideas from LZ77 and open-sourced in 2011.It does not aim for maximum compression, or compatibility with any other compression library; instead, it aims for very high speeds and reasonable compression. Compression speed is 250 MB/s and decompression speed is 500 MB/s using a single core.

PROGRAMS WITH OUTPUT:

Setting storage path
Defaults to ~/pystore or PYSTORE_PATH environment variable (if set)
pystore.set_path("~/pystore")

List stores
pystore.list_stores()

Connect to datastore (create it if not exist)
store = pystore.store('mydatastore')

List existing collections
store.list_collections()


Access a collection (create it if not exist)
collection = store.collection('NASDAQ')

List items in collection
collection.list_items()

Load some data from Quandl
aapl = quandl.get("WIKI/AAPL", authtoken="your token here")

Store the first 100 rows of the data in the collection under "AAPL"
collection.write('AAPL', aapl[:100], metadata={'source': 'Quandl'})

Reading the item's data
item = collection.item('AAPL') data = item.data # <-- Dask dataframe (see dask.pydata.org) metadata = item.metadata df = item.to_pandas()

Append the rest of the rows to the "AAPL" item
collection.append('AAPL', aapl[100:])

Reading the item's data
item = collection.item('AAPL') data = item.data metadata = item.metadata df = item.to_pandas()
PROGRAMS WITH OUTPUT:
# Install package
pip install quandl
conda install -c conda-forge snappy
conda install -c ranaroussi pystore
# Import libraries
import quandl
import pystore
# Using Quandl's API to download 37+ years worth of historical data for Apple's stock.
aapl = quandl.get('WIKI/AAPL')
aapl.head()
Output: 
# Storage path 
pystore.get_path()
Output:
WindowsPath('C:/Users/HP/pystore')
# Path can be changed by calling set_path() mathod 
# Set storage path
 pystore.set_path('./pystore_demo')
 # show the new storage path
 pystore.get_path()
Output:
' WindowsPath('C:/pystore_demo')
# Get list of datastores found in this location
# Since this is a start, output is an empty list
# List stores
 pystore.list_stores()
Output:
[]

Creating / connecting to datastore: 
# When connecting to a datastore, if it doesn't exist, it will be automatically created
store = pystore.store('mydatastore')
store 
Output:
PyStore.datastore <C:\pystore_demo\mydatastore>
# To get a list with the new datastore listed
pystore.list_stores() 
Output:
['mydatastore']



Creating / connecting to a Collection:
# To create a Collection (or namespace) that maps to a directory containing partitioned parquet files for each item (e.g. symbol)
# When connecting to a collection, if it doesn't exist, it will be automatically created
# Access a collection (create it if not exist)
 collection = store.collection('NASDAQ.EOD')
 collection
Output:
PyStore.collection <NASDAQ.EOD>
# List can show all the newly created collection
store.list_collections()
Output:
['NASDAQ.EOD']
Working with collection items:
 # To see if there are any existing items in the collection
 collection.list_items()
Output:
set()
# To store data
collection.write('AAPL', aapl[:-1], metadata={'source': 'Quandl'},overwrite=True) 
# To list all items in the collections, to see newly created item
collection.list_items()
Output:
{'AAPL'}

# Read the item's data
item = collection.item('AAPL') 
item 
Output:
PyStore.item <NASDAQ.EOD/AAPL>


# data returns a Dask datafram
# metadata returns the metadata attached to the item, along with an "updated" timestamp
data = item.data 
data

Output:
 
item.metadata

Output:
{'source': 'Quandl', '_updated': '2020-12-09 13:01:11.380157'}
# To load the item's data as a Pandas dataframe
df = item.to_pandas() 
df.tail()

Output:
 
# To append the last day (row) to item
 collection.append('AAPL', aapl[-1:])

 df = collection.item('AAPL').to_pandas()
 df.tail()

Output:
 
Querying Collections:
 # To look some items up by metadata by adding metadata key to the list_items method
collection.list_items(source='Quandl') 

Output:
{'AAPL'}
Working with Snapshots:
# PyStore allows to create snapshots - a point-in-time, named reference for all current items in a collection.
# To see if there are any existing snapshots
collection.list_snapshots() 

Output:
[]
# Creating a snapshot using the create_snapshot method
collection.create_snapshot('snapshot_name') 
collection.list_snapshots() 
Output:
['snapshot_name']
# To see how snapshots work, original AAPL is changed to only include the Close and Volume columns
collection.write('AAPL', aapl[['Close', 'Volume']], metadata={'source': 'Quandl'}, overwrite=True) 
# Load the "new" item 
df = collection.item('AAPL').to_pandas() 
df.tail() 
Output:
 


# To load the item from a previous snapshot
snap_df = collection.item('AAPL', snapshot='snapshot_name') 
snap_df.to_pandas().tail()
Output:

 

# To restore data from snapshot
collection.write('AAPL', snap_df,metadata={'source': 'Quandl'},overwrite=True)
df = collection.item('AAPL').to_pandas()
df.tail()
Output:

 

# Delete a collection snapshot
collection.delete_snapshot('snapshot_name')
# To delete all snapshots
# collection.delete_snapshots()
Output:
True
Deleting items, collections and stores:
# Delete the item from the current version
collection.delete_item('AAPL')
Output:
True
# Delete the collection
store.delete_collection('NASDAQ.EOD')
Output:
True
# Delete the datastore
pystore.delete_store('mydatastore')

# to delete all datastores in the path
# pystore.delete_stores()
Output:
True







CONCLUSION:
Hence, the basics in PyStore has been understood and code has been written, executed and output has been verified. 



19. INTRODUCTION TO JSON

AIM: 
To understand, read and write JSON files using Python and Pandas.

DESCRIPTION:

JavaScript Object Notation (JSON) is a data format that stores data in a human-readable form. While it can be technically be used for storage, JSON files are primarily used for serialization and information exchange between a client and server. Although it was derived from JavaScript, it's platform-agnostic and is a widely-spread and used format - most prevalently in REST APIs.

Creating a JSON File:

To create JSON files via Python, data has to be stored in a certain way. There are multiple ways of storing this data using Python. 
Creating JSON Data via a Nested Dictionaries:
In Python, nested dictionaries can be used to create JSON data. Each item inside the outer dictionary corresponds to a column in the JSON file. The key of each item is the column header and the value is another dictionary consisting of rows in that particular column. 

Creating JSON Data via Lists of Dictionaries:
Another way to create JSON data is via a list of dictionaries. Each item in the list consists of a dictionary and each dictionary represents a row. This approach is a lot more readable than using nested dictionaries.

Writing Data to a JSON File via Python:
With nested dictionary and a list of dictionaries, data can be stored in a JSON file. For this, JSON module and dump() method are used. 

Reading JSON Files with Pandas from Local Files:
To read a JSON file via Pandas, the read_json() method is used and the path to the file to be read is applied to it. The method returns a Pandas Dataframe that stores data in the form of columns and rows.
Reading JSON from Remote Files:
The read_json() method isn't limited to only reading local files but also used to read JSON files located on remote servers by passing the path of the remote JSON file to the function call.
Converting Pandas to JSON Data Files:
To convert a Pandas dataframe to a JSON file, to_json() function is used on the dataframe, and the path is passed to the soon-to-be file as a parameter.
PROGRAMS WITH OUTPUT:

Creating JSON Data via a Nested Dictionaries:
# First item represents Name column. 
# Item value consists of a dictionary where dictionary items represent rows
# Keys of the inner dictionary items represents index numbers of rows
patients = {
         "Name":{"0":"John","1":"Nick","2":"Ali","3":"Joseph"},             
         "Gender":{"0":"Male","1":"Male","2":"Female","3":"Male"},          
         "Nationality":{"0":"UK","1":"French","2":"USA","3":"Brazil"},
         "Age" :{"0":10,"1":25,"2":35,"3":29}
                 }
Creating JSON Data via Lists of Dictionaries:
# Each dictionary items represents a row in a JSON file
cars = [
    {"Name":"Honda", "Price": 10000, "Model":2005, "Power": 1300},
    {"Name":"Toyota", "Price": 12000, "Model":2010, "Power": 1600},
    {"Name":"Audi", "Price": 25000, "Model":2017, "Power": 1800},
    {"Name":"Ford", "Price": 28000, "Model":2009, "Power": 1200},
           ]

Writing Data to a JSON File via Python:
import json
with open('H:\\patients.json', 'w') as f:
    json.dump(patients, f) 
with open('H:\\cars.json', 'w') as f:
    json.dump(cars, f) 

Output:
 

Reading JSON Files with Pandas from Local Files:
import pandas as pd
patients_df = pd.read_json('H:\\patients.json')
patients_df.head()

Output:
 
import pandas as pd
cars_df = pd.read_json('H:\\cars.json')
cars_df.head()
Output:
 


Reading JSON from Remote Files:

import pandas as pd
iris_data=pd.read_json("https://raw.githubusercontent.com/domoritz/maps/master/data/iris.json")iris_data.head()
Output:
 

Converting Pandas to JSON Data Files:
#Load a dataset (seaborn tips dataset)
import seaborn as sns
dataset = sns.load_dataset('tips')
dataset.head()

Output:
 
# Convert the dataset to json file
dataset.to_json('H:\\tips.json')
Output:
 




CONCLUSION:
Hence, reading and writing of JSON files has been understood and programs have been written and output has been verified. 



20. INTRODUCTION TO RSS_BEAUTIFULSOUP

AIM: 
To understand the data and to do operations of fetching and parsing using Beautifulsoup.
DESCRIPTION:

It is possible to extract data from Web and this is called Web Scraping. Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.

Beautiful Soup is a Python library for pulling data (scrape data from the web) out of HTML and XML files. 
It works to provide idiomatic ways of navigating, searching, and modifying the parse tree. It commonly saves hours or days of work.

PROGRAMS WITH OUTPUT:
# Install the Essential Python Libraries
pip install requests beautifulsoup4
# Import "requests" library to fetch the page content 
# Import bs4 (Beautiful Soup) for parsing the HTML page content
from bs4 import BeautifulSoup
import requests
url = “https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(nominal)”
# Make a GET request to fetch the raw HTML content
html_content = requests.get(url).text
# Parse the html content
soup = BeautifulSoup(html_content, "lxml")
# print the parsed data of html
print(soup.prettify())

Output:
 
# Print title of the webpage
print(soup.title)
Output:
<title>List of countries by GDP (nominal) - Wikipedia</title>
# To get the text without the HTML tags
print(soup.title.text)
Output:
List of countries by GDP (nominal) – Wikipedia

# To get all links in the page with attributes (href, title,inner Text)
for link in soup.find_all("a"):
    print("Inner Text: {}".format(link.text))
    print("Title: {}".format(link.get("title")))
    print("href: {}".format(link.get("href")))

Output:
 

# First tr tag is for headings of all three tables
# Next tr tag is for table data for all three inner tables.

# To get all three table headings
gdp_table = soup.find("table", attrs={"class": "wikitable"})
# contains 2 rows
gdp_table_data = gdp_table.tbody.find_all("tr") 
# Get all the headings of Lists
headings = []
for td in gdp_table_data[0].find_all("td"):
    # remove any newlines and extra spaces from left and right
    headings.append(td.b.text.replace('\n', ' ').strip())
print(headings)

Output:
['Per the International Monetary Fund (2020 estimates)', 'Per the World Bank (2019)', 'Per the United Nations (2019)']

# To get content of all three tables by iterating over each table and its rows
data = {}
for table, heading in zip(gdp_table_data[1].find_all("table"), headings):
    # Get headers of table i.e., Rank, Country, GDP
    t_headers = []
    for th in table.find_all("th"):
        # remove any newlines and extra spaces from left and right
        t_headers.append(th.text.replace('\n', ' ').strip())
    # Get all the rows of table
    table_data = []
    # find all tr's from table's tbody
    for tr in table.tbody.find_all("tr"): 
        t_row = {}
        # Each table row is stored in the form of
        # t_row = {'Rank': '', 'Country/Territory': '', 'GDP(US$million)': ''}

        # find all td's(3) in tr and zip it with t_header
        for td, th in zip(tr.find_all("td"), t_headers): 
            t_row[th] = td.text.replace('\n', '').strip()
        table_data.append(t_row)

    # Put the data for the table with his heading
    data[heading] = table_data

print(data)
Output:
 


# Export to CSV file by iterating over it
import csv

for topic, table in data.items():
    # Create csv file for each table
    with open(f"{topic}.csv", 'w') as out_file:
        # Each 3 table has headers as following
        headers = [ 
            "Country/Territory",
            "GDP(US$million)",
            "Rank"
        ] 
        # == t_headers
        writer = csv.DictWriter(out_file, headers)
        # write the header
        writer.writeheader()
        for row in table:
            if row:
                writer.writerow(row)


Output:
 

Example:
Importing the libraries:
from bs4 import BeautifulSoup
import requests
import csv
Sending a HTTP request to a URL:
url = https://www.srmist.edu.in/department-of-information-technology/faculty
# Make a GET request to fetch the raw HTML content
html_content = requests.get(url).text
Parse the html content:
soup = BeautifulSoup(html_content, "lxml")

Analyze the HTML tag:
my_table = soup.find("table", attrs={"class": "table table-striped hostel-fee"})
my_table_data = my_table.tbody.find_all("tr")

Getting the headers:
headings = []
for td in my_table_data[0].find_all("td"):
    headings.append(td.b.text.replace('\n', ' ').strip())
headings
Output:
['FACULTY', 'DESIGNATION', 'RESEARCH INTEREST']

Getting the Data:
from bs4 import BeautifulSoup
name_data =[]
research_data=[]
# find all tr's from table's tbody
for tr in my_table.tbody.find_all("tr"): 
    if(tr.a==None):
        name_data.append(headings[0])
        research_data.append(headings[2])
    else:
        name_data.append(tr.a.text)
        t1=tr.text.replace('\n', '')
        t2=t1.split('\t')
        research_data.append(t2[-1])
#print(research_data)

Converting the data into csv format:
import csv
with open('file.csv', 'w') as f:
    writer = csv.writer(f)
    writer.writerows(zip(name_data, research_data))



Displaying the table data:
import pandas as pd
df=pd.read_csv('file.csv',encoding= 'unicode_escape')
df
Output:
 




CONCLUSION:
Hence, operations of fetching and parsing using Beautifulsoup has been understood and programs have been written and output has been verified. 




21. INTRODUCTION TO SCRAPY

AIM: 
To understand the data and use Scrapy library to scrape data from a website.

DESCRIPTION:

It is possible to extract data from Web and this is called Web Scraping. Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.

Scrapy is an open source and collaborative framework for extracting data from websites in a fast, simple, yet extensible way. It is a framework which allows to focus on the data extraction using CSS selectors and choosing XPath expressions and less on the intricate internals of how spiders are supposed to work. Spiders are classes that are defined and that Scrapy uses to scrape information from a website (or a group of websites). 
They must subclass Spider and define the initial requests to make, optionally how to follow links in the pages, and how to parse the downloaded page content to extract data.

PROGRAMS WITH OUTPUT:
# Settings for notebook
from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"
# Show Python version
import platform
platform.python_version()
Import Scrapy:

try:
    import scrapy
except:
    !pip install scrapy
    import scrapy
from scrapy.crawler import CrawlerProcess



Setup a Pipeline:

# This class creates a simple pipeline that writes all found items to a JSON file, where each line contains one JSON element
import json
class JsonWriterPipeline(object):

    def open_spider(self, spider):
        self.file = open('quoteresult.jl', 'w')

    def close_spider(self, spider):
        self.file.close()

    def process_item(self, item, spider):
        line = json.dumps(dict(item)) + "\n"
        self.file.write(line)
        return item

Define the Spider:

# QuotesSpider class defines from which URLs to start crawling and which values to retrieve
# Logging level of the crawler is set to warning to avoid DEBUG messages
import logging

class QuotesSpider(scrapy.Spider):
    name = "quotes"
    start_urls = [
        'http://quotes.toscrape.com/page/1/',
        'http://quotes.toscrape.com/page/2/',
    ]
    custom_settings = {
        'LOG_LEVEL': logging.WARNING,
        'ITEM_PIPELINES': {'__main__.JsonWriterPipeline': 1}, # Used for pipeline 1
        'FEED_FORMAT':'json',                                                      # Used for pipeline 2
        'FEED_URI': 'quoteresult.json'                                             # Used for pipeline 2
    }
    
    def parse(self, response):
        for quote in response.css('div.quote'):
            yield {
                'text': quote.css('span.text::text').extract_first(),
                'author': quote.css('span small::text').extract_first(),
                'tags': quote.css('div.tags a.tag::text').extract(),
            }


Start the crawler:

process = CrawlerProcess({
    'USER_AGENT': 'Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 5.1)'
})

process.crawl(QuotesSpider)
process.start()


Create dataframes:

import pandas as pd
df = pd.read_json('quoteresult.jl', lines=True)
df.head(10)

Output:
 




CONCLUSION:
Hence, scraping of data from website using Scrapy library has been understood and programs have been written and output has been verified. 


22. INTRODUCTION TO WORDCLOUD

AIM: 
To understand wordcloud and visualize words in a text using wordcloud.
DESCRIPTION:
Word cloud is a technique for visualising frequent words in a text where the size of the words represents their frequency. Various arguments for WordCloud function:
1)	width/height: The word cloud dimension can be changed to preferred width and height
2)	random_state:  By setting this parameter, reproducibility of the exact same word cloud can be ensured. 
3)	background_colour: ‘white’ and ‘black’ are common background colours. 
4)	colormap: To set up colour theme that the words are displayed in. (eg) ‘rainbow’, ‘seismic’, ‘Pastel1’ and Pastel2’.
5)	collocations: This is set as False to ensure that the word cloud doesn’t appear as if it contains any duplicate words. Otherwise, ‘web’, ‘scraping’ and ‘web scraping’ is seen as a collocation in the word cloud, giving an impression that words have been duplicated.
6)	stopwords: Stopwords are common words which provide little to no value to the meaning of the text. (eg)‘We’, ‘are’ and ‘the’. 
PROGRAMS WITH OUTPUT:
Data:
# To use text from Wikipedia
pip install Wikipedia
# Import packages
import Wikipedia
import re
# Specify the title of the Wikipedia page
wiki = wikipedia.page('List_of_political_parties_in_India')
# Extract the plain text content of the page
text = wiki.content
# Clean text
text = re.sub(r'==.*?==+', '', text)
text = text.replace('\n', '')
text
Output:
 


Wordcloud:
import matplotlib.pyplot as plt
# Define a function to plot word cloud
def plot_cloud(wordcloud):
    # Set figure size
    plt.figure(figsize=(10, 5))
    # Display image
    plt.imshow(wordcloud)
    # No axis details
    # plt.axis("off")

# Import package
from wordcloud import WordCloud, STOPWORDS
# Generate word cloud
wordcloud = WordCloud(width = 500, height = 500, random_state=1, background_color='white', colormap='Set2', collocations=False, stopwords = STOPWORDS).generate(text)
# Plot
plot_cloud(wordcloud)
Output:
 
Example:
# Using beautifulsoup
import requests
from bs4 import BeautifulSoup

# url = "https://timesofindia.indiatimes.com/politics/news"
# page_request = requests.get(url)
# data = page_request.content
# soup = BeautifulSoup(data,"html.parser")

soup = BeautifulSoup(requests.get("https://timesofindia.indiatimes.com/topic/Tamil-Nadu-Election/news").content,"html.parser")
reviews = soup.find(name="div", attrs={'class': 'tab_content'}).ul
for a in reviews(href = True):
    temp = str("https://timesofindia.indiatimes.com"+str(a['href']))
    print(temp)
results = ["https://timesofindia.indiatimes.com"+a['href'] for a in reviews(href=True)]

Output:
 

# To derive the content from links
import pandas as pd
import numpy as np
from newspaper import Article
for i in results:
    art = Article(i)
    art.download()
    art.parse()
    print(art.text)

Output:
 


# To tokenize text
import nltk
raw = art.text
tokens = nltk.word_tokenize(raw)
tokens
Output:
 
# To convert tokens to lowercase
tokens = [item.lower() for item in tokens]
tokens
Output:
 

#To display poltical parties and their members
list1=['dhinakaran','jayalalithaa','kamal','rajinikanth','haasan','edappadi','palanisamy','panneerselvam','amma']
list2=['aiadmk','bjp','dmk','ammk']
Members = [i for i in tokens if i in list1]
Parties = [i for i in tokens if i in list2]


# Wordcloud
import matplotlib.pyplot as plt
# Define a function to plot word cloud
def plot_cloud(wordcloud):
    # Set figure size
    plt.figure(figsize=(8, 8))
    # Display image
    plt.imshow(wordcloud)
    # No axis details
    # plt.axis("off")
# Import package
from wordcloud import WordCloud, STOPWORDS
# Import packages
import numpy as np
# PIL used from importing image
from PIL import Image
# Import image to np.array
mask = np.array(Image.open('tamilnadu.jpg'))
# Generate wordcloud
wordcloud = WordCloud( background_color='WHITE', collocations=False, stopwords = STOPWORDS, mask=mask).generate(str(tokens))
# Plot
plot_cloud(wordcloud)
plt.title("TAMIL NADU LATEST POLITIC NEWS", fontdict = {'fontsize' : 10})
Output:
 
# Display Politic Members
# Import package
from wordcloud import WordCloud, STOPWORDS
# Generate word cloud
wordcloud = WordCloud(width = 300, height = 300, random_state=1, background_color='black', colormap='Set2', collocations=False, stopwords = STOPWORDS).generate(str(Members))
# Plot
plot_cloud(wordcloud)
plt.title("TAMIL NADU POLITIC MEMBERS", fontdict = {'fontsize' : 10})

Output:
 


# Display Political Parties
# Import package
from wordcloud import WordCloud, STOPWORDS
# Generate word cloud
wordcloud = WordCloud(width = 200, height = 100, random_state=1, background_color='black', colormap='Set2', collocations=False, stopwords = STOPWORDS).generate(str(Parties))
# Plot
plot_cloud(wordcloud)
plt.title("TAMIL NADU POLITIC PARTIES", fontdict = {'fontsize' : 10})



Output:
 










CONCLUSION:
Hence, forming wordcloud has been understood and words in a text have been visualized and output has been verified. 

23. INTRODUCTION TO SQLITE

AIM: 
To understand SQLite and to do basic operations with it.
DESCRIPTION:

SQL (Structured Query Language) is a domain-specific language used in programming and designed for managing data held in a relational database management system (RDBMS), or for stream processing in a relational data stream management system (RDSMS). It is particularly useful in handling structured data where there are relations between different entities/variables of the data. 
SQLite is an in-process library that implements a self contained, serverless, zero configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private. 
SQLite is an embedded SQL database engine. Unlike most other SQL databases, SQLite does not have a separate server process. SQLite reads and writes directly to ordinary disk files. A complete SQL database with multiple tables, indices, triggers, and views, is contained in a single disk file. It is a compact library and is very carefully tested prior to every release and has a reputation for being very reliable. Most of the SQLite source code is devoted purely to testing and verification. 

PROGRAMS WITH OUTPUT:
Import SQLite:

# Import to use SQLite3 module
import sqlite3
Create a SQLite Database:
db = sqlite3.connect('test.db')


Create table:
cursor = db.cursor()

cursor.execute("CREATE TABLE writer(FirstName VARCHAR(50) NOT NULL, LastName VARCHAR(50) NOT NULL, USERID int PRIMARY KEY)")
cursor.execute("SELECT name FROM sqlite_master WHERE type = 'table'").fetchall()
Output:
[('books',), ('writer',)]

Insert data:

cursor.execute("INSERT INTO writer VALUES ('William', 'Shakespeare', 1618)")
cursor.execute("INSERT INTO writer VALUES ('Lin', 'Han', 1997)")
cursor.execute("INSERT INTO writer VALUES ('Peter', 'Brecht', 1979)")
cursor.execute("commit")
Write query:
rows=cursor.execute("SELECT * from writer").fetchall()
rows
Output:
[('William', 'Shakespeare', 1618),
 ('Lin', 'Han', 1997),
 ('Peter', 'Brecht', 1979)]
Close connection:
db.close()

CONCLUSION:
Hence, basics of SQLite has been understood and programs have been written, executed and output has been verified. 

24. LINEAR REGRESSION

AIM: 
To predict and summarize relationships between dependent and independent variable using Linear Regression model. 

DESCRIPTION:

Creating a model and predicting housing prices for regions in the USA. 
Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.
Attributes:
•	'Avg. Area Income': Avg. Income of residents of the city house is located in.
•	'Avg. Area House Age': Avg Age of Houses in same city
•	'Avg. Area Number of Rooms': Avg Number of Rooms for Houses in same city
•	'Avg. Area Number of Bedrooms': Avg Number of Bedrooms for Houses in same city
•	'Area Population': Population of city house is located in
•	'Price': Price that the house sold at
•	'Address': Address for the house
Regression Evaluation Metrics:
Here are three common evaluation metrics for regression problems:
Mean Absolute Error (MAE) is the mean of the absolute value of the errors:
1𝑛∑𝑖=1𝑛|𝑦𝑖−𝑦̂ 𝑖|1n∑i=1n|yi−y^i|
Mean Squared Error (MSE) is the mean of the squared errors:
1𝑛∑𝑖=1(𝑦𝑖−𝑦̂ 𝑖)21n∑i=1n(yi−y^i)2
Root Mean Squared Error (RMSE) is the square root of the mean of the squared errors:
1𝑛∑𝑖=1(𝑦𝑖−𝑦̂ 𝑖)21n∑i=1n(yi−y^i)2
Comparing these metrics:
•	MAE is the easiest to understand, because it's the average error.
•	MSE is more popular than MAE, because MSE "punishes" larger errors, which tends to be useful in the real world.
•	RMSE is even more popular than MSE, because RMSE is interpretable in the "y" units.
All of these are loss functions, because we want to minimize them.


PROGRAMS WITH OUTPUT:

Import libraries:

# Data preprocessing/numerical calculations
import numpy as np 
# Read data/import data
import pandas as pd 
# Mathematic plotting library/plotting data/visualization
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
# Machine Learning model
from sklearn.linear_model import LinearRegression
# For Train/Test operations
from sklearn.model_selection import train_test_split


Read dataset:
USAhousing = pd.read_csv('USA_Housing.csv')
USAhousing.head()

Output:
 




USAhousing.info()

Output:
 



USAhousing.describe()

Output:
 

Exploratory Data Analysis:
Pairplot:
sns.pairplot(USAhousing)
Output:
 




Distplot:
sns.distplot(USAhousing['Price'])
Output:
 
Heatmap:
Heatmap - sns.heatmap(USAhousing.corr())
Output:
 





Model Building:
Step1: Determine Input and Output
X = USAhousing[['Avg. Area Income', 'Avg. Area House Age', 'Avg. Area Number of Rooms',    'Avg. Area Number of Bedrooms', 'Area Population']]
y = USAhousing['Price']
Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.4, random_state=101)
Step3: Fit training data into model
lm = LinearRegression()
lm.fit(X_train,y_train)
Output: 

LinearRegression(copy_X=True, fit_intercept=True, n_jobs=None, normalize=False)

Step4: Model Evaluation
print(lm.intercept_)
coeff_df = pd.DataFrame(lm.coef_,X.columns,columns=['Coefficient'])
coeff_df
Output:
 
Step5: Model Interpretation
•	Holding all other features fixed, a 1 unit increase in Avg. Area Income is associated with an *increase of $21.52 *.
•	Holding all other features fixed, a 1 unit increase in Avg. Area House Age is associated with an *increase of $164883.28 *.
•	Holding all other features fixed, a 1 unit increase in Avg. Area Number of Rooms is associated with an *increase of $122368.67 *.
•	Holding all other features fixed, a 1 unit increase in Avg. Area Number of Bedrooms is associated with an *increase of $2233.80 *.
•	Holding all other features fixed, a 1 unit increase in Area Population is associated with an *increase of $15.15 *.
Step6: Model Predictions
predictions = lm.predict(X_test)
plt.scatter(y_test,predictions)
Output:
 
sns.distplot((y_test-predictions),bins=50)
Output: Residual Histogram
 
Regression Evaluation Metrics:

print('MAE:', metrics.mean_absolute_error(y_test, predictions))
print('MSE:', metrics.mean_squared_error(y_test, predictions))
print('RMSE:', np.sqrt(metrics.mean_squared_error(y_test, predictions)))
Output:
MAE: 82288.22251914957
MSE: 10460958907.209501
RMSE: 102278.82922291153













CONCLUSION:
Hence, a simple linear regression model to predict and summarize relationships between dependent and independent variable has been created and output has been verified.



25. LOGISTIC REGRESSION

AIM: 
To predict and summarize relationships between dependent and independent variable using Logistic Regression model. 
Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

DESCRIPTION:

Creating a model and predicting the presence or absence of diabetes(outcome) using various attributes.
Attributes:
•	'Pregnancies': Total number of pregnancies of patients
•	'Glucose': Glucose level of patients
•	'Blood Pressure': Blood Pressure level of patients
•	'Skin Thickness': Skin Thickness of patients
•	'Insulin': Insulin level of patients
•	'BMI': BMI value of patients
•	'DiabetesPedigreeFunction': DiabetesPedigreeFunction of patients
•	'Age': Age of patients
•	'Outcome': Outcome (0 for diabetes and 1 fro non-diabetes) of patients
PROGRAMS WITH OUTPUT:

Import libraries:

# Data preprocessing/numerical calculations
import numpy as np 
# Read data/import data
import pandas as pd 
import warnings
warnings.filterwarnings('ignore')
# Mathematic plotting library/plotting data/visualization
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
# Machine Learning model
from sklearn.linear_model import LogisticRegression
# For Train/Test operations
from sklearn.model_selection import train_test_split


# calculating metrics, confusion matrix and classification report and accuracy score
from sklearn import metrics
from sklearn.metrics import confusion_matrix
from sklearn.metrics import classification_report
from sklearn.metrics import accuracy_score


Read dataset:

df = pd.read_csv('diabetes.csv')
df.head()

Output:
 

df.info()

Output:
 

df.describe()
Output:

 


df.isnull().sum()
Output:
 



Exploratory Data Analysis:
Heatmap: 
plt.figure(figsize=[15,10])
sns.heatmap(df.corr(), annot=True)
Output:
 
Barplot:
plt.figure(figsize=[15,10])
df['Pregnancies'].value_counts().plot(kind='bar')
Output:
 

Piechart:
plt.figure(figsize=[10,7])
df['Outcome'].value_counts().plot(kind="pie")
Output:
 
Histogram:
df.plot(x='BMI',y=['Pregnancies','Glucose','BloodPressure','SkinThickness'],kind='hist')
plt.show()
Output:
 

Boxplot:
plt.figure(figsize=[15,10])
plt.subplot(3,3,1)
sns.boxplot(df['BMI'])
plt.subplot(3,3,2)
sns.boxplot(df['Pregnancies'])
plt.subplot(3,3,3)
sns.boxplot(df['SkinThickness'])
plt.subplot(3,3,4)
sns.boxplot(df['Glucose'])
plt.subplot(3,3,5)
sns.boxplot(df['BloodPressure'])
plt.subplot(3,3,6)
sns.boxplot(df['Insulin'])
plt.subplot(3,3,7)
sns.boxplot(df['DiabetesPedigreeFunction'])
plt.subplot(3,3,8)
sns.boxplot(df['Age'])
plt.subplot(3,3,9)
sns.boxplot(df['Outcome'])
Output:

 


Histogram:
df.plot(kind='hist')
Output:
 
Scatterplot:
plt.figure(figsize=[15,10])
plt.scatter(df['BMI'],df['SkinThickness'])
Output:
 

Pairplot:
sns.pairplot(df)
Output:
 

Model Building:
Step1: Determine Input and Output
X = df.drop('Outcome',axis=1)
y = df['Outcome']

Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, y_train, y_test = train_test_split(X,y, test_size=0.30, random_state=101)

Step3: Fit training data into model

logmodel = LogisticRegression(max_iter=5000)
logmodel.fit(X_train,y_train)
Output: 

LogisticRegression(max_iter=5000)


Step4: Model Evaluation
predictions = logmodel.predict(X_test)
print(classification_report(y_test,predictions)
Output:
 




confusion_matrix(y_test,predictions)
Output:
 


accuracy_score(y_test,predictions)
Output:
0.7835497835497836
















CONCLUSION:
Hence, a logistic regression model to predict and summarize relationships between dependent and independent variable has been created and output has been verified.
26. KNN

AIM: 
To create a model to classify target class for classified data, depending on different independent variables.

DESCRIPTION:

K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions).
Creating a model and classifying target class for classified data, depending on different independent variables.
Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

PROGRAMS WITH OUTPUT:


Import libraries:

# Data preprocessing/numerical calculations
import numpy as np 
# Read data/import data
import pandas as pd 
import warnings
warnings.filterwarnings('ignore')
# Mathematic plotting library/plotting data/visualization
import matplotlib.pyplot as plt
%matplotlib inline
# Machine Learning model
from sklearn.neighbors import KNeighborsClassifier
# For Train/Test operations
from sklearn.model_selection import train_test_split


# calculating metrics, confusion matrix, classification report and accuracy score
from sklearn import metrics
from sklearn.metrics import confusion_matrix
from sklearn.metrics import classification_report
from sklearn.metrics import accuracy_score





Read dataset:

df = pd.read_csv('Classified Data')
df.head()

Output:
 

Model Building:
Step1: Determine Input and Output
X = df.drop('TARGET CLASS',axis=1)
y = df['TARGET CLASS']

Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, y_train, y_test = train_test_split(X,y, test_size=0.30, random_state=101)

Step3: Fit training data into model

knn = KNeighborsClassifier(n_neighbors=1)
knn.fit(X_train, y_train)
Output: 

KNeighborsClassifier(n_neighbors=1)
Step4: Model Evaluation
pred = knn.predict(X_test)
print(classification_report(y_test, pred))
Output:
 

confusion_matrix(y_test, pred)
Output:
 

accuracy_score(y_test, pred)
Output:
0.54

The KNN model varies with different K values thus figuring out the optimum K value will give us better results for our model. 
Two ways to find out the K values is as follows:





Graphical Representation of the accuracy’s method:
accuracy = []
for i in range(1,40):

    knn = KNeighborsClassifier(n_neighbors=i)
    knn.fit(X_train, y_train)
    pred_i = knn.predict(X_test)
    accuracy.append(accuracy_score(y_test, pred_i))

# Plotting graph
plt.figure(figsize=(10,6))
plt.plot(range(1,40), accuracy, color='blue', linestyle='dashed',marker='o', markerfacecolor='red', markersize=10)
plt.title('Error rate vs K value')
plt.xlabel('K')
plt.ylabel('Error rate')
Output:
 




Confusion matrix method:
#Calculating the sensitivity, specificity, accuracy for different K values
df_threshold = pd.DataFrame( columns = ['K-Value','accuracy','sensitivity','specificity'])
num = []
for i in range(1,25):
    num.append(i)
for i in num:
    knn = KNeighborsClassifier(n_neighbors=i)
    knn.fit(X_train, y_train)
    pred_i = knn.predict(X_test)
    cm1 =confusion_matrix(y_test, pred_i)
    acc = accuracy_score(y_test,pred_i)
    speci = cm1[0,0]/(cm1[0,0]+cm1[0,1])
    sensi = cm1[1,1]/(cm1[1,0]+cm1[1,1])
    df_threshold.loc[i] =[ i ,acc,sensi,speci]
print(df_threshold)
df_threshold.plot(x='K-Value', y=['accuracy','sensitivity','specificity'])
plt.show()
Output:
 
CONCLUSION:
Hence, a KNN model to classify target class for classified data, depending on different independent variables has been created and output has been verified.
27. DECISION TREES AND VISUALIZATION

AIM: 
To predict and summarize relationships between dependent and independent variable using decision tree model and visualize it.

DESCRIPTION:

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, decision tress and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

Decision trees are a popular supervised learning method for a variety of reasons. Benefits of decision trees include that they can be used for both regression and classification, they don’t require feature scaling, and they are relatively easy to interpret as decision trees can be visualized. This is not only a powerful way to understand model, but also to communicate how model works. Consequently, it would help to know how to make a visualization based on the model.

PROGRAMS WITH OUTPUT:

Import libraries:

# Data preprocessing/numerical calculations
import numpy as np 
# Read data/import data
import pandas as pd 
import warnings
warnings.filterwarnings('ignore')
# Mathematic plotting library/plotting data/visualization
import matplotlib.pyplot as plt
%matplotlib inline
# from sklearn.datasets import load_iris
from sklearn.datasets import load_iris
# Machine Learning model
from sklearn import tree
from sklearn.tree import DecisionTreeClassifier
# For Train/Test operations
from sklearn.model_selection import train_test_split



Read dataset:

from sklearn.datasets import load_iris
data = load_iris()
df = pd.DataFrame(data.data, columns=data.feature_names)
df['target'] = data.target
df.head()
Output:
 
Model Building:
Step1: Determine Input and Output
X = df[data.feature_names]
Y = df['target']
Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, Y_train, Y_test = train_test_split(X, Y, random_state=0)

Step3: Fit training data into model

# Import the model you want to use
from sklearn.tree import DecisionTreeClassifier
# Make an instance of the Model
clf = DecisionTreeClassifier(max_depth = 2,random_state = 0)
# Train the model on the data
clf.fit(X_train, Y_train)
Output: 

DecisionTreeClassifier(max_depth=2, random_state=0)



Step4: Model Evaluation
# Predict labels of unseen (test) data
clf.predict(X_test)
Output:
array([2, 1, 0, 2, 0, 2, 0, 1, 1, 1, 2, 1, 1, 1, 1, 0, 1, 1, 0, 0, 1, 1,
       0, 0, 1, 0, 0, 1, 1, 0, 2, 1, 0, 1, 2, 1, 0, 2])


Visualization:
# Entropy is a measure of disorder or uncertainty
# Goal of machine learning models  is to reduce uncertainty
tree.plot_tree(clf);
Output:
 
fn=['sepal length (cm)','sepal width (cm)','petal length (cm)','petal width (cm)']
cn=['setosa', 'versicolor', 'virginica']
fig, axes = plt.subplots(nrows = 1,ncols = 1,figsize = (2,2), dpi=300)
tree.plot_tree(clf,
               feature_names = fn, 
               class_names=cn,
               filled = True);
#fig.savefig('dt1.png')

Output:
 
Example:
Import libraries:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
from sklearn.model_selection import train_test_split





Read dataset:

df = pd.read_csv('kyphosis.csv')
df.head()
Output:
 
Exploratory Data Analysis:
sns.pairplot(df,hue='Kyphosis',palette='Set1')
Output:
 


Model Building:
Step1: Determine Input and Output
X = df.drop('Kyphosis',axis=1)
y = df['Kyphosis']
Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30)

Step3: Fit training data into model

# Import the model you want to use
from sklearn.tree import DecisionTreeClassifier
# Make an instance of the Model
dtree = DecisionTreeClassifier()
# Train the model on the data
dtree.fit(X_train,y_train)
Output: 

DecisionTreeClassifier()

Step4: Model Evaluation
# Predict labels of unseen (test) data
predictions = dtree.predict(X_test)
from sklearn.metrics import classification_report,confusion_matrix
print(classification_report(y_test,predictions))
Output:
 
print(confusion_matrix(y_test,predictions))
Output:
[[19  4]
 [ 0  2]]
Tree Visualization:
from sklearn import tree
tree.plot_tree(dtree)
Output:
 
fn=['Age','Number','Start']
cn=['absent', 'present']
fig, axes = plt.subplots(nrows = 1,ncols = 1,figsize = (4,4), dpi=300)
tree.plot_tree(dtree,
               feature_names = fn,
               class_names=cn,
               filled = True);
fig.savefig('dt1.png')
Output:
 
CONCLUSION:
Hence, decision tree model to predict and summarize relationships between dependent and independent variable has been created and output has been visualized and verified.
28. RANDOM FOREST

AIM: 
To predict and summarize relationships between dependent and independent variable using random forest and visualize it.

DESCRIPTION:

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, decision tress and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

A random forest randomly selects observations/rows and specific features/variables to build multiple decision trees from and then averages the results. After a large number of trees are built using this method, each tree "votes" or chooses the class, and the class receiving the most votes by a simple majority is the "winner" or predicted class.
PROGRAMS WITH OUTPUT:

Import libraries:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
from sklearn.model_selection import train_test_split

Read dataset:

df = pd.read_csv('kyphosis.csv')
df.head() 
Output:
 
Exploratory Data Analysis:
sns.pairplot(df,hue='Kyphosis',palette='Set1')
Output:
 

Model Building:
Step1: Determine Input and Output
X = df.drop('Kyphosis',axis=1)
y = df['Kyphosis']
Step2: Splitting data
#Data is split into a training set and a testing set. 
#Train set to train out model
#Test set to evaluate the model.
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30)

Step3: Fit training data into model

# Import the model you want to use
from sklearn.ensemble import RandomForestClassifier
# Make an instance of the Model
rfc = RandomForestClassifier(n_estimators=100)
# Train the model on the data
rfc.fit(X_train, y_train)
Output: 

RandomForestClassifier(bootstrap=True, class_weight=None, criterion='gini',
                       max_depth=None, max_features='auto', max_leaf_nodes=None,
                       min_impurity_decrease=0.0, min_impurity_split=None,
                       min_samples_leaf=1, min_samples_split=2,
                       min_weight_fraction_leaf=0.0, n_estimators=100,
                       n_jobs=None, oob_score=False, random_state=None,
                       verbose=0, warm_start=False)

Step4: Model Evaluation
# Predict labels of unseen (test) data
rfc_pred = rfc.predict(X_test)
from sklearn.metrics import classification_report,confusion_matrix
print(classification_report(y_test,rfc_pred))
Output:
 

print(confusion_matrix(y_test,rfc_pred))
Output:
[[19  3]
 [ 2  1]]
 
Tree Visualization:
1)	 from sklearn import tree
fn=['Age','Number','Start']
cn=['absent', 'present']
fig, axes = plt.subplots(nrows = 1,
                                     ncols = 1,
                                     figsize = (4,4), 
                                     dpi=300)
tree.plot_tree(rfc.estimators_[0],
               feature_names = fn, 
               class_names=cn,
               filled = True);
fig.savefig('dt2.png')


Output:
 




2)	fn=['Age','Number','Start']
cn=['absent', 'present']
fig, axes = plt.subplots(nrows = 1,
                                     ncols = 1,
                                     figsize = (4,4), 
                                     dpi=300)
tree.plot_tree(rfc.estimators_[1],
               feature_names = fn,
               class_names=cn,
               filled = True);
fig.savefig('dt3.png')






3)	fn=['Age','Number','Start']
cn=['absent', 'present']
fig, axes = plt.subplots(nrows = 1,
                                      ncols = 1,
                                      figsize = (4,4), 
                                      dpi=300)
tree.plot_tree(rfc.estimators_[2],
               feature_names = fn, 
               class_names=cn,
               filled = True);
fig.savefig('dt4.png')


Output: 

Output:
 









4)	fn=['Age','Number','Start']
cn=['absent', 'present']
fig, axes = plt.subplots(nrows = 1,
                                      ncols = 1,
                                      figsize = (4,4), 
                                      dpi=300)
tree.plot_tree(rfc.estimators_[3],
               feature_names = fn, 
               class_names=cn,
               filled = True);
fig.savefig('dt5.png')













Output: 


 





CONCLUSION:
Hence, random forest model to predict and summarize relationships between dependent and independent variable has been created and output has been visualized and verified.


29. K-MEANS CLUSTERING

AIM: 
To identify clusters in the data, understand, predict model using K-Means and to visualize it.

DESCRIPTION:

K-means clustering is one of the simplest and popular unsupervised machine learning algorithms. Typically, unsupervised algorithms make inferences from datasets using only input vectors without referring to known, or labelled, outcomes. 

The objective of K-means is to group similar data points together and discover underlying patterns. To achieve this, K-means looks for a fixed number (k) of clusters in a dataset. A cluster refers to a collection of data points aggregated together because of certain similarities.

A target number k is defined, which refers to the number of centroids needed in the dataset. A centroid is the imaginary or real location representing the center of the cluster. Every data point is allocated to each of the clusters through reducing the in-cluster sum of squares. In other words, the K-means algorithm identifies k number of centroids, and then allocates every data point to the nearest cluster, while keeping the centroids as small as possible. The ‘means’ in the K-means refers to averaging of the data; that is, finding the centroid.

PROGRAMS WITH OUTPUT:

Import libraries:
import seaborn as sns
import matplotlib.pyplot as plt
%matplotlib inline
Read dataset:
from sklearn.datasets import make_blobs
data = make_blobs(n_samples=200, n_features=2,
                          centers=4, cluster_std=1.8,random_state=101)
data[0][:10,0]
Output:
array([ -6.42884095,   5.86867888,  -0.37610937,   2.16679181,
         5.0950857 , -10.87888819,   2.03405554,  -1.71798771,
         1.16911341,  -1.35185444])
Visualization:

plt.scatter(data[0][:,0],data[0][:,1])
Output:
 

plt.scatter(data[0][:,0],data[0][:,1],c=data[1],cmap='rainbow')
Output:
 
Cluster Creation:
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=4)
kmeans.fit(data[0])
Output:
KMeans(n_clusters=4)

kmeans.cluster_centers_
Output:
array([[ 3.71749226,  7.01388735],
       [-9.46941837, -6.56081545],
       [-4.13591321,  7.95389851],
       [-0.0123077 ,  2.13407664]])

kmeans.labels_
Output:
array([2, 0, 3, 0, 0, 1, 0, 3, 0, 3, 2, 3, 0, 0, 2, 3, 0, 3, 1, 2, 1, 3,
       3, 1, 2, 1, 1, 3, 0, 0, 2, 1, 0, 3, 3, 2, 1, 1, 1, 3, 1, 2, 2, 2,
       3, 0, 2, 3, 1, 3, 3, 2, 0, 3, 1, 2, 3, 3, 2, 0, 1, 0, 1, 2, 0, 3,
       1, 0, 0, 1, 0, 3, 1, 3, 1, 0, 0, 3, 2, 3, 3, 1, 0, 1, 3, 3, 3, 2,
       3, 1, 1, 1, 1, 3, 3, 1, 0, 2, 1, 0, 3, 1, 3, 3, 0, 3, 1, 0, 1, 1,
       0, 2, 2, 0, 1, 0, 2, 2, 0, 2, 3, 2, 3, 2, 3, 0, 2, 3, 1, 2, 2, 2,
       3, 1, 1, 2, 0, 2, 0, 3, 1, 0, 1, 2, 2, 0, 3, 1, 2, 2, 2, 2, 3, 0,
       3, 2, 0, 0, 0, 3, 0, 3, 3, 2, 1, 2, 3, 0, 2, 3, 0, 3, 2, 0, 3, 2,
       0, 0, 1, 0, 2, 1, 1, 2, 1, 1, 1, 1, 1, 3, 1, 0, 0, 2, 1, 3, 0, 0,
       1, 3])


f, (ax1, ax2) = plt.subplots(1, 2, sharey=True,figsize=(10,6))
ax1.set_title('K Means')
ax1.scatter(data[0][:,0],data[0][:,1],c=kmeans.labels_,cmap='rainbow')
ax2.set_title("Original")
ax2.scatter(data[0][:,0],data[0][:,1],c=data[1],cmap='rainbow')



Output:
 









CONCLUSION:
Hence, clusters in the data has been identified, model has been understood and output has been visualized and verified.



30. PRINCIPAL COMPONENT ANALYSIS

AIM: 
To reduce set of variables and to analyze and interpret the data using Principal Component Analysis(PCA).
DESCRIPTION:

Principal Component Analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets, by transforming a large set of variables into a smaller one that still contains most of the information in the large set.
Reducing the number of variables of a data set naturally comes at the expense of accuracy, but the trick in dimensionality reduction is to trade a little accuracy for simplicity. Because smaller data sets are easier to explore and visualize and make analyzing data much easier and faster for machine learning algorithms without extraneous variables to process.
Main idea of PCA is to reduce the number of variables of a data set, while preserving as much information as possible.
STANDARDIZATION:
The aim is to standardize the range of the continuous initial variables so that each one of them contributes equally to the analysis.
More specifically, the reason why it is critical to perform standardization prior to PCA, is that the latter is quite sensitive regarding the variances of the initial variables. That is, if there are large differences between the ranges of initial variables, those variables with larger ranges will dominate over those with small ranges (For example, a variable that ranges between 0 and 100 will dominate over a variable that ranges between 0 and 1), which will lead to biased results. So, transforming the data to comparable scales can prevent this problem.
Mathematically, this can be done by subtracting the mean and dividing by the standard deviation for each value of each variable.
 
Once the standardization is done, all the variables will be transformed to the same scale.
 
PROGRAMS WITH OUTPUT:

Import libraries:

import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
import seaborn as sns
%matplotlib inline

Read dataset:

# Cancer data
from sklearn.datasets import load_breast_cancer
cancer = load_breast_cancer()
cancer.keys()

Output:
dict_keys(['data', 'target', 'frame', 'target_names', 'DESCR', 'feature_names', 'filename'])

print(cancer['DESCR'])
Output:
 

df = pd.DataFrame(cancer['data'],columns=cancer['feature_names'])
df.head()

Output:
 
Standardization:
from sklearn.preprocessing import StandardScaler
scaler = StandardScaler()
scaler.fit(df)
scaled_data = scaler.transform(df)
scaled_data
Output:
array([[ 1.09706398, -2.07333501,  1.26993369, ...,  2.29607613,
         2.75062224,  1.93701461],
       [ 1.82982061, -0.35363241,  1.68595471, ...,  1.0870843 ,
        -0.24388967,  0.28118999],
       [ 1.57988811,  0.45618695,  1.56650313, ...,  1.95500035,
         1.152255  ,  0.20139121],
       ...,
       [ 0.70228425,  2.0455738 ,  0.67267578, ...,  0.41406869,
        -1.10454895, -0.31840916],
       [ 1.83834103,  2.33645719,  1.98252415, ...,  2.28998549,
         1.91908301,  2.21963528],
       [-1.80840125,  1.22179204, -1.81438851, ..., -1.74506282,
        -0.04813821, -0.75120669]])

PCA Model:
from sklearn.decomposition import PCA
pca = PCA(n_components=2)
pca.fit(scaled_data)
Output:
PCA(n_components=2)
scaled_data.shape
Output:
(569, 30)
# Transform to first 2 principal components
x_pca = pca.transform(scaled_data)
x_pca.shape
Output:
(569, 2)

Visualization:
plt.figure(figsize=(8,6))
plt.scatter(x_pca[:,0],x_pca[:,1],c=cancer['target'],cmap='plasma')
plt.xlabel('First principal component')
plt.ylabel('Second Principal Component')
Output:
 



CONCLUSION:
Hence, reduction of variables has been done and the data has been analyzed and interpreted using Principal Component Analysis (PCA).

