# Python---Machine-Learning-
This includes basics of python programming along with basics for machine learning.
1. **PYTHON**  **INTRODUCTION**

**AIM:**

To write a python program to execute various basic commands of python.

**DESCRIPTION:**

In this first experiment we will go through the basic examples of python and understand different data types, operators, conditional statements, methods etc.

**PROGRAMS WITH OUTPUT:**

## Data types:

### Numbers:

1 + 1

**Output: 2**

1 \* 3

**Output: 3**

1 / 2

**Output: 0.5**

2 \*\* 4

**Output: 16**

4 % 2

**Output: 0**

5 % 2

**Output: 1**

(2 + 3) \* (5 + 5)

**Output: 50**

### Variable Assignment:

_# Can not start with number or special characters_
name\_of\_var = 2
x = 2
y = 3
z = x + y
 z

**Output: 5**

### Strings:

_&#39;single quotes&#39;_

**Output: &#39;single quotes&#39;**

_&quot;double quotes&quot;_

**Output: &#39;double quotes&#39;**

_&quot; wrap lot&#39;s of other quotes&quot;_

**Output: &quot; wrap lot&#39;s of other quotes&quot;**

### Printing:

x = &#39;hello&#39;
x

**Output: &#39;hello&#39;**

print(x)

**Output: hello**

num = 12
name = &#39;Sam&#39;
print(&#39;My number is: {one}, and my name is: {two}&#39;.format(one=num,two=name))

**Output: My number is: 12, and my name is: Sam**

print(&#39;My number is: {}, and my name is: {}&#39;.format(num,name))

**Output: My number is: 12, and my name is: Sam**

### Lists:

[1,2,3]

**Output: [1, 2, 3]**

[&#39;hi&#39;,1,[1,2]]

**Output: [&#39;hi&#39;, 1, [1, 2]]**

my\_list = [&#39;a&#39;,&#39;b&#39;,&#39;c&#39;]
 my\_list.append(&#39;d&#39;)
 my\_list

**Output: [&#39;a&#39;, &#39;b&#39;, &#39;c&#39;, &#39;d&#39;]**

my\_list[0]

**Output: &#39;a&#39;**

my\_list[1]

**Output: &#39;b&#39;**

my\_list[1:]

**Output: [&#39;b&#39;, &#39;c&#39;, &#39;d&#39;]**

my\_list[:1]

**Output: [&#39;a&#39;]**

my\_list[0] = &#39;NEW&#39;
my\_list

**Output: [&#39;NEW&#39;, &#39;b&#39;, &#39;c&#39;, &#39;d&#39;]**

nest = [1,2,3,[4,5,[&#39;target&#39;]]]
 nest[3]

**Output: [4, 5, [&#39;target&#39;]]**

nest[3][2]

**Output: [&#39;target&#39;]**

nest[3][2][0]

**Output: &#39;target&#39;**

### Dictionaries:

d = {&#39;key1&#39;:&#39;item1&#39;,&#39;key2&#39;:&#39;item2&#39;}
 d

**Output: {&#39;key1&#39;: &#39;item1&#39;, &#39;key2&#39;: &#39;item2&#39;}**

d[&#39;key1&#39;]

**Output: &#39;item1&#39;**

### Booleans:

True

**Output: True**

False

**Output: False**

### Tuples:

t = (1,2,3)
 t[0]

**Output: 1**

t[0] = &#39;NEW&#39;

**Output:**

**TypeError Traceback (most recent call last)**
**TypeError: &#39;tuple&#39; object does not support item assignment**

### Sets:

{1,2,3}

**Output: {1, 2, 3}**

{1,2,3,1,2,1,2,3,3,3,3,2,2,2,1,1,2}

**Output: {1, 2, 3}**

## Comparison Operators:

1 \&gt; 2

**Output: False**

1 \&lt; 2

**Output: True**

1 \&gt;= 1

**Output: True**

1 \&lt;= 4

**Output: True**

1 == 1

**Output: True**

_&#39;hi&#39;_ == &#39;bye&#39;

**Output: False**

## Logic Operators:

(1 \&gt; 2) and (2 \&lt; 3)

**Output: False**

(1 \&gt; 2) or (2 \&lt; 3)

**Output: True**

(1 == 2) or (2 == 3) or (4 == 4)

**Output: True**

## if,elif, else Statements:

**if** 1 \&lt; 2:
print(&#39;Yep!&#39;)

**Output: Yep!**

**if** 1 \&lt; 2:
print(&#39;yep!&#39;)

**Output: yep!**

**if** 1 \&lt; 2:
print(&#39;first&#39;)
**else** :
print(&#39;last&#39;)

**Output: first**

**if** 1 \&gt; 2:
print(&#39;first&#39;)
**else** :
print(&#39;last&#39;)

**Output: last**

**if** 1 == 2:
print(&#39;first&#39;)
**elif** 3 == 3:
print(&#39;middle&#39;)
**else** :
print(&#39;Last&#39;)

**Output: middle**

## for Loops:

seq = [1,2,3,4,5]
**for** item in seq:
print(item)

**Output:**

**1**
**2**
**3**
**4**
**5**

**for** item in seq:
print(&#39;Yep&#39;)

**Output:**

**Yep**
**Yep**
**Yep**
**Yep**
**Yep**

**for** jelly in seq:
print(jelly+jelly)

**Output:**

**2**
**4**
**6**
**8**
**10**

## while Loops:

i = 1
**while** i \&lt; 5:
print(&#39;i is: {}&#39;.format(i))
 i = i+1

**Output:**

**i is: 1**
**i is: 2**
**i is: 3**
**i is: 4**

**range():**

range(5)

**Output: range(0, 5)**

**for** i in range(5):
print(i)

**Output:**

**0**
**1**
**2**
**3**
**4**

list(range(5))

**Output: [0, 1, 2, 3, 4]**

## list comprehension:

x = [1,2,3,4]
 out = []
**for** item in x:
 out.append(item\*\*2)
print(out)

**Output: [1, 4, 9, 16]**

[item\*\*2 **for** item in x]

**Output: [1, 4, 9, 16**]

## functions:

**def** my\_func(param1=&#39;default&#39;):
_&quot;&quot;&quot;_
 _Docstring goes here._
 _&quot;&quot;&quot;_
print(param1)
 my\_func

**Output: \&lt;function \_\_main\_\_.my\_func(param1=&#39;default&#39;)\&gt;**

my\_func()

**Output: default**

my\_func(&#39;new param&#39;)

**Output: new param**

my\_func(param1=&#39;new param&#39;)

**Output: new param**

**def** square(x):
**return** x\*\*2
out = square(2)
print(out)

**Output: 4**

## lambda expressions:

**def** times2(var):
**return** var\*2
times2(2)

**Output: 4**

x= **lambda** var: var\*2
x(3)

**Output: 6**

## map and filter:

seq = [1,2,3,4,5]
map(times2,seq)

**Output: \&lt;map at 0x16b151364a8\&gt;**

list(map(times2,seq))

**Output: [2, 4, 6, 8, 10]**

list(map( **lambda** var: var\*2,seq))

**Output: [2, 4, 6, 8, 10]**

filter( **lambda** item: item%2 == 0,seq)

**Output: \&lt;filter at 0x16b150b5908\&gt;**

list(filter( **lambda** item: item%2 == 0,seq))

**Output: [2, 4]**

## methods:

st = &#39;hello my name is Sam&#39;
st.lower()

**Output: &#39;hello my name is sam&#39;**

st.upper()

**Output: &#39;HELLO MY NAME IS SAM&#39;**

st.split()

**Output: [&#39;hello&#39;, &#39;my&#39;, &#39;name&#39;, &#39;is&#39;, &#39;Sam&#39;]**

tweet = &#39;Go Sports! #Sports&#39;
tweet.split(&#39;#&#39;)

**Output: [&#39;Go Sports! &#39;, &#39;Sports&#39;]**

tweet.split(&#39;#&#39;)[1]

**Output: &#39;Sports&#39;**

d

**Output: {&#39;key1&#39;: &#39;item1&#39;, &#39;key2&#39;: &#39;item2&#39;}**

d.keys()

**Output: dict\_keys([&#39;key1&#39;, &#39;key2&#39;])**

d.items()

**Output: dict\_items([(&#39;key1&#39;, &#39;item1&#39;), (&#39;key2&#39;, &#39;item2&#39;)])**

lst = [1,2,3]
 lst.pop()

**Output: 3**

lst

**Output: [1, 2]**

_&#39;x&#39;_ in [1,2,3]

**Output: False**

_&#39;x&#39;_ in [&#39;x&#39;,&#39;y&#39;,&#39;z&#39;]

**Output: True**

## EXERCISES:

1.
## What is 7 to the power of 4?

7\*\*4

Output: 2401
2.
## Split this string: s = &quot;Hi there Sam!&quot; into a list

s = &quot;Hi there Sam!&quot;
split()

Output: [&#39;Hi&#39;, &#39;there&#39;, &#39;Sam!&#39;]
3.
## planet = &quot;Earth&quot;, diameter = 12742
 Use .format() to print the following string:
 The diameter of Earth is 12742 kilometers.

planet = &quot;Earth&quot;
diameter = 12742
print(&quot;The diameter of {} is {} kilometers.&quot;.format(planet,diameter))

Output: The diameter of Earth is 12742 kilometers.
4.
## Given this nested list, use indexing to grab the word &quot;hello&quot;
lst = [1,2,[3,4],[5,[100,200,[&#39;hello&#39;]],23,11],1,7]

lst = [1,2,[3,4],[5,[100,200,[&#39;hello&#39;]],23,11],1,7]
lst[3][1][2][0]
_#look for the index_

Output: &#39;hello&#39;
5.
## Given this nest dictionary grab the word &quot;hello&quot;.
d = {&#39;k1&#39;:[1,2,3,{&#39;tricky&#39;:[&#39;oh&#39;,&#39;man&#39;,&#39;inception&#39;,{&#39;target&#39;:[1,2,3,&#39;hello&#39;]}]}]}

d = {&#39;k1&#39;:[1,2,3,{&#39;tricky&#39;:[&#39;oh&#39;,&#39;man&#39;,&#39;inception&#39;,{&#39;target&#39;:[1,2,3,&#39;hello&#39;]}]}]}
d[&#39;k1&#39;][3][&#39;tricky&#39;][3][&#39;target&#39;][3]

Output: &#39;hello&#39;
6.
## What is the main difference between a tuple and a list?

Output: _Tuple is immutable_
7.
## Create a function that grabs the email website domain from a string in the form:
&quot;user@domain.com&quot;
Passing &quot;user@domain.com&quot; would return: domain.com

**def** a(x):
**return** x.split(&#39;@&#39;)[1] _#a split is formed at @_
a(&#39;user@domain.com&#39;)

Output: &#39;domain.com&#39;

**def** a(x):
**return** x.split(&#39;@&#39;)[1]
a(&#39;user@domain.com@in&#39;)

Output: &#39;domain.com&#39;
8.
## Create a basic function that returns True if the word &#39;dog&#39; is contained in the input string:
&#39;Is there a dog here?&#39;. Do account capitalization.

**def** a(x):
**return**&#39;dog&#39; in x.lower().split()
a(&#39;Is there a dog here?&#39;)

Output: True
9.
## Create a function that counts the number of times the word &quot;dog&quot; occurs in a string:
&#39;Is there a dog here?&#39;

**def** countDog(st):
 count = 0
**for** word in st.lower().split():
**if** word == &#39;dog&#39;:
 count += 1
**return** count
countDog(&#39;This dog runs faster than the other dog dude!&#39;)

 Output: 2

**def** a(x):
**return** x.count(&#39;dog&#39;)
a(&#39;Is there a dog dog here?&#39;)

Output: 2
10.
## Use lambda expressions and the filter() function to filter out words from a list that don&#39;t start with the letter &#39;s&#39;.
 For example: seq = [&#39;soup&#39;,&#39;dog&#39;,&#39;salad&#39;,&#39;cat&#39;,&#39;great&#39;]
 Should be filtered down to: [&#39;soup&#39;,&#39;salad&#39;]

seq = [&#39;soup&#39;,&#39;dog&#39;,&#39;salad&#39;,&#39;cat&#39;,&#39;great&#39;]
list(filter( **lambda** x: x[0]==&#39;s&#39;,seq))

Output: [&#39;soup&#39;, &#39;salad&#39;]
11.
## You are driving a little too fast, and a police officer stops you.Write a function to return one of 3 possible results:
If speed is 60 or less, the result is &quot;No Ticket&quot;.
If speed is between 61 and 80 inclusive, the result is &quot;Small Ticket&quot;.
If speed is 81 or more, the result is &quot;Big Ticket&quot;.
Unless it is your birthday (encoded as a boolean value in the parameters of the function), your speed can be 5 higher in all cases.

**def** caught\_speeding(speed, is\_birthday):
**if** is\_birthday:
 speeding = speed + 5
**else** :
 speeding = speed
**if** speeding \&lt;= 60:
**return**&#39;No Ticket&#39;
**elif** speeding \&gt; 61 and speeding \&lt;= 80:
**return**&#39;Small Ticket&#39;
**elif** speeding \&gt;= 81:
**return**&#39;Big Ticket&#39;
caught\_speeding(56,True)

 caught\_speeding(56,False)

Output: &#39;No Ticket&#39;

caught\_speeding(56,False)

Output: &#39;No Ticket&#39;

**CONCLUSION:**

Hence, python programs to perform various basic commands have been written, executed and output has been verified.

**2. INTRODUCTION TO NUMPY**

**AIM:**

To write a program in python to execute the basics of Numpy.

**DESCRIPTION:**

NumPy (or Numpy) is a Linear Algebra Library for Python, the reason it is so important for Data Science with Python is that almost all of the libraries in the PyData Ecosystem rely on NumPy as one of their main building blocks.

 **Built-in Methods:**

There are lots of built-in ways to generate arrays.

**arange:**

Return evenly spaced values within a given interval.

**zeros and ones:**

Generate arrays of zeros or ones.

**linspace:**

Return evenly spaced numbers over a specified interval.

**eye:**

Creates an identity matrix.

**Random:**

Numpy also has lots of ways to create random number arrays.

### rand:

Create an array of the given shape and populate it with random samples from a uniform distribution over [0, 1).

**randn:**

Return a sample (or samples) from the &quot;standard normal&quot; distribution.

**randint:**

Return random integers from low (inclusive) to high (exclusive).

**reshape:**

Returns an array containing the same data with a new shape.

**max,min,argmax,argmin:**

These are useful methods for finding max or min values or to find their index locations using argmin or argmax.

**shape:**

Shape is an attribute that arrays have (not a method):

**dtype:**

Data type of the object in the array can be retrieved.

**PROGRAMS WITH OUTPUT:**

import numpy as np

## Arrays:

x=[1, 2, 3, 4, 5]
np.array(x)

**Output: array([1, 2, 3, 4, 5])**

x=np.array(16)
x

**Output: array(16)**

x=numpy.array([[1, 2, 3], [4, 5, 6]])
print(x)

**Output:**

**[[1 2 3]**
 **[4 5 6]]**

## Array indexing:

x=np.array([1, 2, 3, 4, 5])
x[1]

**Output: 2**

x=np.array([[1, 2, 3], [4, 5, 6]])
x[1,2]

**Output: 6**

## Array Slicing:

x=np.array([1, 2, 3, 4, 5]) _#includes start index 1(eg.2) but omits end index(eg.5)_
x[1:3]

**Output: array([2, 3])**

x=np.array([1, 2, 3, 4, 5]) _#starts from index 0 but omits end index(eg.5)_
x[:3]

**Output: array([1, 2, 3])**

x=np.array([1, 2, 3, 4, 5]) _#starts from index 1 and prints till last value_
x[1:]

**Output: array([2, 3, 4, 5])**

x=np.array([1, 2, 3, 4, 5])
_#-3 and -1 prints from reverse_
_#includes end index 1(eg.4) but omits start index(eg.2)_
x[-3:-1]

**Output: array([3, 4])**

x=np.array([1, 2, 3, 4, 5])
x[0:4:2]
_#prints from index0 to index4 with space of 2_

**Output: array([1, 3])**

## BUILT-IN METHODS:

## arange:

np.arange(1,5,3)
_#3 refers to gap between the first two numbers_

**Output: array([1, 4])**

np.arange(0,10)

**Output: array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])**

np.arange(0,11,2)

**Output: array([0, 2, 4, 6, 8, 10])**

## zeros and ones:

np.zeros(2)

**Output: array([0., 0.])**

np.zeros((2,2))

**Output:**

**array([[0., 0.],**
 **[0., 0.]])**

np.ones(2)

**Output: array([1., 1.])**

np.ones((2,2))

**Output:**

**array([[1., 1.],**
 **[1., 1.]])**

## linspace:

np.linspace(1,7,4)
_#linspace is done with eaual spacing(4 refers to number of integers to be printed with equal spacing)_

**Output: array([1., 3., 5., 7.])**

np.linspace(0,10,3)

**Output: array([0., 5., 10.])**

np.linspace(0,10,50)

**Output:**

**array([ 0. , 0.20408163, 0.40816327, 0.6122449 , 0.81632653,**
 **1.02040816, 1.2244898 , 1.42857143, 1.63265306, 1.83673469,**
 **2.04081633, 2.24489796, 2.44897959, 2.65306122, 2.85714286,**
 **3.06122449, 3.26530612, 3.46938776, 3.67346939, 3.87755102,**
 **4.08163265, 4.28571429, 4.48979592, 4.69387755, 4.89795918,**
 **5.10204082, 5.30612245, 5.51020408, 5.71428571, 5.91836735,**
 **6.12244898, 6.32653061, 6.53061224, 6.73469388, 6.93877551,**
 **7.14285714, 7.34693878, 7.55102041, 7.75510204, 7.95918367,**
 **8.16326531, 8.36734694, 8.57142857, 8.7755102 , 8.97959184,**
 **9.18367347, 9.3877551 , 9.59183673, 9.79591837, 10. ])**

## eye:

np.eye(3) _#identity matrix_

**Output:**

**array([[1., 0., 0.],**
 **[0., 1., 0.],**
 **[0., 0., 1.]])**

## Random:

## rand:

np.random.rand(2) _#gives uniform distribution_

**Output: array([0.59899436, 0.57500594])**

np.random.rand(5,5)

**Output:**

**array([[0.8532597 , 0.78513659, 0.36389639, 0.81208698, 0.27504804],**
 **[0.43572746, 0.29009358, 0.60207693, 0.30800814, 0.26021457],**
 **[0.90321102, 0.91925396, 0.13992916, 0.03292513, 0.93188869],**
 **[0.98898628, 0.09062172, 0.52095818, 0.34706827, 0.02027942],**
 **[0.99790924, 0.5957805 , 0.76999301, 0.05253998, 0.14099702]])**

## randn:

np.random.randn(2) _#gives standard normal distribution_

**Output: array([0.3475921 , -0.89893673])**

np.random.randn(5,5)

**Output:**

**array([[ 7.88238894e-04, 1.98097952e+00, -1.34520834e+00,**
 **-1.42765648e+00, 8.78573621e-01],**
 **[-8.42102821e-01, -3.33368933e-02, 6.80767197e-02,**
 **-1.75352891e-01, -1.58288094e+00],**
 **[ 8.44616834e-01, 6.22000673e-01, 3.75869213e-01,**
 **-5.64942435e-01, -8.94084724e-01],**
 **[-7.18814278e-01, 1.02690101e+00, 7.64674021e-01,**
 **-3.34669840e-01, 7.08345840e-01],**
 **[ 3.84149740e-01, -3.09014613e-01, 1.07635099e+00,**
 **-9.26246979e-01, -8.81341808e-01]])**

## randint:

np.random.randint(100)

**Output: 41**

np.random.randint(1,100)

**Output: 85**

np.random.randint(1,100,10)

**Output: array([35, 64, 63, 90, 47, 18, 21, 71, 9, 38])**

np.random.randint(1,20,(5,5))

**Output:**

**array([[19, 19, 19, 8, 5],**
 **[15, 4, 19, 11, 19],**
 **[5, 2, 5, 1, 14],**
 **[16, 10, 1, 17, 9],**
 **[19, 18, 5, 6, 1]])**

## shape:

arr=numpy.array([[1,2,3],[4,5,6]]) _#specifies rows and columns_
arr.shape

**Output: (2, 3)**

## reshape:

arr=np.array([[1,2,3],[4,5,6]])
arr.reshape(6,1)

**Output:**

**array([[1],**
 **[2],**
 **[3],**
 **[4],**
 **[5],**
 **[6]])**

arr=np.array([[1,2,3,4],[4,5,6,7]])
arr.reshape (2,2,2)

**Output:**

**array([[[1, 2],**
 **[3, 4]],**

 **[[4, 5],**
 **[6, 7]]])**

arr=numpy.array([1,2,3,4,5,6])
print(arr.shape)
print(&#39;\n&#39;)
b=arr.reshape(2,3)
print(b)
print(&#39;\n&#39;)
print(b.shape)

**Output:**

**(6,)**

**[[1 2 3]**
 **[4 5 6]]**

**(2, 3)**

## Flattening:

arr=numpy.array([[1,2,3],[4,5,6]]) _#converts 2D array into 1D_
print (arr.reshape(-1))

**Output: [1 2 3 4 5 6]**

# max,min,argmax,argmin:

arr=np.array([1,2,3,4,5,6])
arr.max()

**Output: 6**

arr.min()

**Output: 1**

arr.argmax()

**Output: 5**

arr.argmin()

**Output: 0**

## dtype:

arr=numpy.array([1,2,3,4,5,6])
arr.dtype

**Output: dtype(&#39;int32&#39;)**

arr=numpy.array([&#39;a&#39;,&#39;b&#39;,&#39;c&#39;])
arr.dtype

**Output: dtype(&#39;\&lt;U1&#39;)**

arr=numpy.array([1,2],dtype=&#39;S&#39;) _#S refers to String_
arr.dtype

**Output: dtype(&#39;S1&#39;)**

**ASSIGNMENT:**

import numpy as np

# 1.Create an array of 10 zeros

np.zeros(10)

**Output: array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])**

# 2.Create an array of 10 ones

np.ones(10)

**Output: array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])**

# 3.Create an array of 10 fives

np.ones(10) \* 5

**Output: array([5., 5., 5., 5., 5., 5., 5., 5., 5., 5.])**

# 4.Create an array of the integers from 10 to 50

np.arange(10,51)

**Output:**

**array([10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26,**
 **27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43,**
 **44, 45, 46, 47, 48, 49, 50])**

# 5.Create an array of all the even integers from 10 to 50

np.arange(10,51,2)

**Output:**

**array([10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42,**
 **44, 46, 48, 50])**

# 6.Create a 3x3 matrix with values ranging from 0 to 8

np.arange(9).reshape(3,3)

**Output:**

**array([[0, 1, 2],**
 **[3, 4, 5],**
 **[6, 7, 8]])**

**7.Create a 3x3 identity matrix**

np.eye(3)

**Output:**

**array([[1., 0., 0.],**
 **[0., 1., 0.],**
 **[0., 0., 1.]])**

# 8.Use NumPy to generate a random number between 0 and 1

np.random.rand(1)

**Output: array([0.6149836])**

# 9.Use NumPy to generate an array of 25 random numbers sampled from a standard normal distribution

np.random.randn(25)

**Output:**

**array([-1.04836744e+00, -2.97633916e+00, -3.82111702e-01, -1.93406555e-03,**
 **8.64101535e-01, -8.37096674e-01, -1.79030546e+00, 3.15415355e-01,**
 **-1.13173998e+00, 1.34093125e+00, -1.12248717e-01, 8.21505846e-01,**
 **1.20541731e+00, -7.98198623e-01, 5.92267250e-01, -4.88767801e-01,**
 **1.72576041e+00, 5.15198394e-01, -1.41620420e+00, 6.23389058e-02,**
 **4.39328639e-01, 5.47428877e-01, -1.43637000e+00, 4.52558065e-01,**
 **3.15599124e-01])**

# 10.Create an array of 20 linearly spaced points between 0 and 1

np.linspace(0,1,20)

**Output:**

**array([0. , 0.05263158, 0.10526316, 0.15789474, 0.21052632,**
 **0.26315789, 0.31578947, 0.36842105, 0.42105263, 0.47368421,**
 **0.52631579, 0.57894737, 0.63157895, 0.68421053, 0.73684211,**
 **0.78947368, 0.84210526, 0.89473684, 0.94736842, 1. ])**

**CONCLUSION:**

Hence, various python programs to perform basics of Numpy have been written, executed and output has been verified.

1. **NUMPY INDEXING AND SELECTION**

**AIM:**

To write a python program to select elements or groups of elements from an array.

**DESCRIPTION:**

## Bracket Indexing and Selection:

The simplest way to pick one or some elements of an array which looks similar to python lists.

## Broadcasting:

Numpy arrays differ from a normal Python list because of their ability to broadcast.Broadcasting describes how numpy treats arrays with different shapes during arithmetic operations.

## Indexing a 2D array (matrices):

The general format of a 2D array is arr\_2d[row][col] or arr\_2d[row,col].

### Fancy Indexing:

Fancy indexing helps to select entire rows or columns out of order.

## Selection:

Refers to the use of brackets for selection including comparison operators.

**PROGRAMS WITH OUTPUT:**

import numpy as np

_#Creating sample array_
arr = np.arange(0,11)
_#Show_
arr

**Output: array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])**

##

##

##

## Bracket Indexing and Selection:

_#Get a value at an index_
arr[8]

**Output: 8**

_#Get values in a range_
arr[1:5]

**Output: array([1, 2, 3, 4])**

_#Get values in a range_
arr[0:5]

**Output: array([0, 1, 2, 3, 4])**

arr[4:]

**Output: array([4, 5, 6, 7, 8, 9, 10])**

## Broadcasting:

_#Setting a value with index range (Broadcasting)_
arr[0:5]=100
_#Show_
arr

**Output: array([100, 100, 100, 100, 100, 5, 6, 7, 8, 9, 10])**

arr[4]=10
arr

**Output: array([0, 1, 2, 3, 10, 5, 6, 7, 8, 9, 10])**

arr[4:]=10
arr

**Output: array([0, 1, 2, 3, 10, 10, 10, 10, 10, 10, 10])**

_# Reset array, we&#39;ll see why I had to reset in a moment_
arr = np.arange(0,11)
_#Show_
arr

**Output: array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])**

_#Important notes on Slices_
slice\_of\_arr = arr[0:6]
_#Show slice_
slice\_of\_arr

**Output: array([0, 1, 2, 3, 4, 5])**

_#Change Slice_
slice\_of\_arr[:]=99
_#Show Slice again_
slice\_of\_arr

**Output: array([99, 99, 99, 99, 99, 99])**

_#The changes also occur in the original array_
arr

**Output: array([99, 99, 99, 99, 99, 99, 6, 7, 8, 9, 10])**

#Data is not copied, it&#39;s a view of the original array
_#To get a copy, need to be explicit_
arr\_copy = arr.copy()
arr\_copy

**Output: array([99, 99, 99, 99, 99, 99, 6, 7, 8, 9, 10])**

## Indexing a 2D array (matrices):

arr\_2d = np.array(([5,10,15],[20,25,30],[35,40,45]))
_#Show_
arr\_2d

**Output:**

**array([[5, 10, 15],**
 **[20, 25, 30],**
 **[35, 40, 45]])**

_#Indexing row_
arr\_2d[1]

**Output: array([20, 25, 30])**

_# Format is arr\_2d[row][col] or arr\_2d[row,col]_
_# Getting individual element value_
arr\_2d[1][0]

**Output: 20**

_# Getting individual element value_
arr\_2d[1,0]

**Output: 20**

_# 2D array slicing_
_#Shape (2,2) from top right corner_
arr\_2d[:2,1:]

**Output:**

**array([[10, 15],**
 **[25, 30]])**

_#Shape bottom row_
arr\_2d[2]

**Output: array([35, 40, 45])**

_#Shape bottom row_
arr\_2d[2,:]

**Output: array([35, 40, 45])**

### Fancy Indexing:

_#Fancy indexing allows you to select entire rows or columns out of order_
_#Set up matrix_
arr2d = np.zeros((10,10))
_#Length of array_
arr\_length = arr2d.shape[1]
_#Set up array_
**for** i in range(arr\_length):
 arr2d[i] = i
arr2d

**Output:**

**array([[0., 0., 0., 0., 0., 0., 0., 0., 0., 0.],**
 **[1., 1., 1., 1., 1., 1., 1., 1., 1., 1.],**
 **[2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],**
 **[3., 3., 3., 3., 3., 3., 3., 3., 3., 3.],**
 **[4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],**
 **[5., 5., 5., 5., 5., 5., 5., 5., 5., 5.],**
 **[6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],**
 **[7., 7., 7., 7., 7., 7., 7., 7., 7., 7.],**
 **[8., 8., 8., 8., 8., 8., 8., 8., 8., 8.],**
 **[9., 9., 9., 9., 9., 9., 9., 9., 9., 9.]])**

arr2d[[2,4,6,8]]

**Output:**

**array([[2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],**
 **[4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],**
 **[6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],**
 **[8., 8., 8., 8., 8., 8., 8., 8., 8., 8.]])**

_#Allows in any order_
arr2d[[6,4,2,7]]

**Output:**

**array([[6., 6., 6., 6., 6., 6., 6., 6., 6., 6.],**
 **[4., 4., 4., 4., 4., 4., 4., 4., 4., 4.],**
 **[2., 2., 2., 2., 2., 2., 2., 2., 2., 2.],**
 **[7., 7., 7., 7., 7., 7., 7., 7., 7., 7.]])**

##

## Selection:

arr = np.arange(1,11)
arr

**Output: array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])**

arr \&gt; 4

**Output: array([False, False, False, False, True, True, True, True, True,****True])**

bool\_arr = arr\&gt;4
bool\_arr

**Output: array([False, False, False, False, True, True, True, True, True, True])**

arr[bool\_arr]

**Output: array([5, 6, 7, 8, 9, 10])**

arr[arr\&gt;2]

**Output: array([3, 4, 5, 6, 7, 8, 9, 10])**

x = 2
arr[arr\&gt;x]

**Output: array([3, 4, 5, 6, 7, 8, 9, 10])**

**CONCLUSION:**

Hence, various python programs to perform selection of elements or groups of elements from an array have been written, executed and output has been verified.

**4. NUMPY OPERATIONS**

# AIM:

To write a program in python to display various operations of arrays using NumPy.

**DESCRIPTION:**

Various operations between two arrays including array with array arithmetic, or scalar with array arithmetic will be performed along with few universal array functions which are commonly used in python.

**Arithmetic:**

Input arrays are used for performing arithmetic operations such as add(), subtract(), multiply(), and divide() etc.

**Universal Array Functions:**

Universal functions in Numpy are simple mathematical functions. It is a term given to mathematical functions in the Numpy library. Numpy provides various universal functions that cover a wide variety of operations. These functions include standard trigonometric functions, functions for arithmetic operations, handling complex numbers, statistical functions, etc.

**PROGRAMS WITH OUTPUT:**

import numpy as np
arr = np.arange(0,10)

arr + arr

**Output: array([0, 2, 4, 6, 8, 10, 12, 14, 16, 18])**

arr \* arr

**Output: array([0, 1, 4, 9, 16, 25, 36, 49, 64, 81])**

arr - arr

**Output: array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])**

_# Warning on division by zero, but not an error!_
_# Just replaced with nan_
arr/arr

C:\ProgramData\Anaconda3\lib\site-packages\ipykernel\_launcher.py:3: RuntimeWarning: invalid value encountered in true\_divide
 This is separate from the ipykernel package so we can avoid doing imports until

**Output: array([nan, 1., 1., 1., 1., 1., 1., 1., 1., 1.])**

_# Warning, but not an error instead infinity_
1/arr

C:\ProgramData\Anaconda3\lib\site-packages\ipykernel\_launcher.py:2: RuntimeWarning: divide by zero encountered in true\_divide

**Output:

 array([ inf, 1. , 0.5 , 0.33333333, 0.25 ,**

 **0.2 , 0.16666667, 0.14285714, 0.125 , 0.11111111])**

arr\*\*3

**Output: array([0, 1, 8, 27, 64, 125, 216, 343, 512, 729], dtype=int32)**

# Universal Array Functions:

_#Taking Square Roots_
np.sqrt(arr)

**Output:**

**array([0. , 1. , 1.41421356, 1.73205081, 2. ,**
 **2.23606798, 2.44948974, 2.64575131, 2.82842712, 3. ])**

_#Calcualting exponential (e^)_
np.exp(arr)

**Output:**

**array([1.00000000e+00, 2.71828183e+00, 7.38905610e+00, 2.00855369e+01,**
 **5.45981500e+01, 1.48413159e+02, 4.03428793e+02, 1.09663316e+03,**
 **2.98095799e+03, 8.10308393e+03])**

np.max(arr) _#same as arr.max()_

**Output: 9**

np.sin(arr)

**Output:**

**array([ 0. , 0.84147098, 0.90929743, 0.14112001, -0.7568025 ,**
 **-0.95892427, -0.2794155 , 0.6569866 , 0.98935825, 0.41211849])**

np.log(arr)

**Output:

 array([ -inf, 0. , 0.69314718, 1.09861229, 1.38629436,**

 **1.60943791, 1.79175947, 1.94591015, 2.07944154, 2.19722458])**

**CONCLUSION:**

Hence, python programs to perform various operations have been written, executed and output has been verified.

**5. INTRODUCTION TO PANDAS - SERIES**

**AIM:**

To write a program in python to display the function of series using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**Series:**

The first main data type for pandas is the Series data type

A Series is very similar to a NumPy array (in fact it is built on top of the NumPy array object) but a Series can have axis labels, meaning it can be indexed by a label, instead of just a number location. It also doesn&#39;t need to hold numeric data, it can hold any arbitrary Python Object.

**PROGRAMS WITH OUTPUT:**

import numpy as np
import pandas as pd

### Creating a Series:

_#A list, numpy array, or dictionary can be converted into a Series_
labels = [&#39;a&#39;,&#39;b&#39;,&#39;c&#39;]
my\_list = [10,20,30]
arr = np.array([10,20,30])
d = {&#39;a&#39;:10,&#39;b&#39;:20,&#39;c&#39;:30}

**Using Lists:**

pd.Series(data=my\_list)

**Output:**

**0 10**
**1 20**
**2 30**
**dtype: int64**

pd.Series(data=d)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int64**

pd.Series(data=labels)

**Output:**

**0 a**
**1 b**
**2 c**
**dtype: object**

pd.Series(data=my\_list,index=labels)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int64**

pd.Series(index=labels,data=my\_list)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int64**

pd.Series(my\_list,labels)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int64**

**Using NumPy Arrays:**

pd.Series(arr)

**Output:**

**0 10**
**1 20**
**2 30**
**dtype: int32**

pd.Series(arr,labels)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int32**

**Using Dictionary:**

pd.Series(d)

**Output:**

**a 10**
**b 20**
**c 30**
**dtype: int64**

### Data in a Series:

_# A pandas Series can hold a variety of object types_
pd.Series(data=labels)

**Output:**

**0 a**
**1 b**
**2 c**
**dtype: object**

##

## Using an Index:

_# The key to using a Series is understanding its index. Pandas makes use of these index names or numbers by allowing for fast look ups of information (works like a hash table or dictionary)._

ser1 = pd.Series([1,2,3,4],index = [&#39;USA&#39;, &#39;Germany&#39;,&#39;USSR&#39;, &#39;Japan&#39;])
ser1

**Output:**

**USA 1**
**Germany 2**
**USSR 3**
**Japan 4**
**dtype: int64**

ser2 = pd.Series([1,2,5,4],index = [&#39;USA&#39;, &#39;Germany&#39;,&#39;Italy&#39;, &#39;Japan&#39;])
ser2

**Output:**

**USA 1**
**Germany 2**
**Italy 5**
**Japan 4**
**dtype: int64**

ser1[&#39;USA&#39;]

**Output:**  **1**

_# Operations are then also done based off of index:_
ser1 + ser2

**Output:**

**Germany 4.0**
**Italy NaN**
**Japan 8.0**
**USA 2.0**
**USSR NaN**
**dtype: float64**

**CONCLUSION:**

Hence, various python programs to display the functions of series using pandas library have been written, executed and output has been verified.

**6. INTRODUCTION TO PANDAS - DATAFRAMES**

**AIM:**

To write a program in python to display the functions of dataframes using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**Dataframes:**

DataFrame is a bunch of Series objects put together to share the same index.

**Selection and Indexing:**

Grabs data from Dataframe.

**Conditional Selection:**

An important feature of pandas is conditional selection using bracket notation, very similar to numpy.

## Indexing:

Various features of indexing includes resetting the index ,setting it to something else, index hierarchy etc.

**PROGRAMS WITH OUTPUT:**

import pandas as pd
 import numpy as np
 from numpy.random import randn
 np.random.seed(101)

df = pd.DataFrame(randn(5,4),index=&#39;A B C D E&#39;.split(),columns=&#39;W X Y Z&#39;.split())
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ad5b116483454eb.png)

**Selection and Indexing:**

df[&#39;W&#39;]

**Output:**

**A 2.706850**

**B 0.651118**

**C -2.018168**

**D 0.188695**

**E 0.190794**

**Name: W, dtype: float64**

_# Pass a list of column names_

df[[&#39;W&#39;,&#39;Z&#39;]]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_508a40ae2219afed.png)

type(df[&#39;Z&#39;])

**Output:**  **pandas.core.series.Series**

**Creating a new column:**

df[&#39;new&#39;] = df[&#39;W&#39;] + df[&#39;Y&#39;]
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_a84a2cbdaf3ebb2d.png)

_#Removing columns_
df.drop(&#39;new&#39;,axis=1)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1b2ca68a4f093dc1.png)

_# Not inplace unless specified_
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_8020965f667f9c64.png)

df.drop(&#39;new&#39;,axis=1,inplace=True)
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_c246b2cf2ad37344.png)

df.drop(&#39;E&#39;,axis=0)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_bf4902434526f60f.png)

**Selecting Rows:**

df.loc[&#39;C&#39;]

**Output:**

**W -2.018168**

**X 0.740122**

**Y 0.528813**

**Z -0.589001**

**Name: C, dtype: float64**

df.iloc[2]

**Output:**

**W -2.018168**

**X 0.740122**

**Y 0.528813**

**Z -0.589001
 Name: C, dtype: float64**

df.loc[&#39;B&#39;,&#39;Y&#39;]

**Output:**  **-0.8480769834036315**

df.loc[[&#39;A&#39;,&#39;B&#39;],[&#39;W&#39;,&#39;Y&#39;]]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_67f5e2e5db3a000.png)

**Conditional Selection:**

df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_c2b0f98da79c1cf5.png)

df\&gt;0

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_fb7cd516e5dc229f.png)

df[df\&gt;0]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_5157dc53c1501486.png)

df[df[&#39;W&#39;]\&gt;0]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_34d4074cf409ab5e.png)

df[df[&#39;W&#39;]\&gt;0][&#39;Y&#39;]

**Output:**

**A 0.907969**

**B -0.848077**

**D -0.933237**

**E 2.605967**

**Name: Y, dtype: float64**

df[df[&#39;W&#39;]\&gt;0][[&#39;Y&#39;,&#39;X&#39;]]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_bdc9268cc3c4c4b7.png)

df[(df[&#39;W&#39;]\&gt;0) &amp; (df[&#39;Y&#39;] \&gt; 1)]

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d2525560dd7f56f2.png)

**More Index Details:**

df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_decfe77f3f726252.png)

# Reset to default 0,1...n index
 df.reset\_index()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ec066a9e17edd7fe.png)

newind = &#39;CA NY WY OR CO&#39;.split()
 df[&#39;States&#39;] = newind
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_2a59a51fd6b2be67.png)

df.set\_index(&#39;States&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_8f68b24f60c26209.png)

df.set\_index(&#39;States&#39;,inplace=True)
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_2bca7eabdfba8b1f.png)

**CONCLUSION:**

Hence, various python programs to display the functions of dataframes using pandas library have been written, executed and output has been verified.

**7. INTRODUCTION TO PANDAS – MISSING DATA**

**AIM:**

To write a program in python to analyze the missing data of a dataset using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**Missing Data:**

Missing Data can occur when no information is provided for one or more items or for a whole unit. Missing Data is a very big problem in real life scenario. Missing Data can also refer to as NA(Not Available) values in pandas. In DataFrame sometimes many datasets simply arrive with missing data, either because it exists and was not collected or it never existed.

**PROGRAMS WITH OUTPUT:**

import numpy as np
import pandas as pd

df = pd.DataFrame({&#39;A&#39;:[1,2,np.nan],
&#39;B&#39;:[5,np.nan,np.nan],
_&#39;C&#39;_:[1,2,3]})
df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_43a2b33f47a48aa.png)

df.dropna()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_5749248f786ccbf3.png)

df.dropna(axis=1)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_dff994acc4bb9604.png)

df.dropna(thresh=1)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_675a9a7d57443468.png)

df.fillna(value=&#39;FILL VALUE&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_340f89617138e804.png)

df[&#39;A&#39;].fillna(value=df[&#39;A&#39;].mean())

**Output:**

**0 1.0**
**1 2.0**
**2 1.5**
**Name: A, dtype: float64**

#

**CONCLUSION:**

Hence, various python programs to analyze the missing data of a dataset using pandas library have been written, executed and output has been verified.

**8. INTRODUCTION TO PANDAS – GROUPBY**

**AIM:**

To write a program in python to perform various operations related to groupby() function using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**Groupby:**

Pandas ** ** groupby method is used to group rows of data together and call aggregate functions. The pandas objects can be split on any of their axes. The abstract definition of grouping is to provide a mapping of labels to group names.

**PROGRAMS WITH OUTPUT:**

 **Groupby:**

import pandas as pd
_# Create dataframe_
data = {&#39;Company&#39;:[&#39;GOOG&#39;,&#39;GOOG&#39;,&#39;MSFT&#39;,&#39;MSFT&#39;,&#39;FB&#39;,&#39;FB&#39;],
_&#39;Person&#39;_:[&#39;Sam&#39;,&#39;Charlie&#39;,&#39;Amy&#39;,&#39;Vanessa&#39;,&#39;Carl&#39;,&#39;Sarah&#39;],
_&#39;Sales&#39;_:[200,120,340,124,243,350]}
df = pd.DataFrame(data)
df

Output:

![](RackMultipart20210731-4-1qy8gmm_html_a0448d8f7107311b.png)

_#.groupby() method to group rows together based off of a column name_
df.groupby(&#39;Company&#39;)

Output:

**\&lt;pandas.core.groupby.generic.DataFrameGroupBy object at 0x0000017D9E1A74C0\&gt;**

_#This object can be saved as a new variable_
by\_comp = df.groupby(&quot;Company&quot;)

**Aggregate methods:**

by\_comp.mean()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_7d61d0080c53f9a1.png)

df.groupby(&#39;Company&#39;).mean()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_b177811d50312d79.png)

by\_comp.std()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_b0c295cf5c305fdc.png)

by\_comp.min()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_a68ebc50763b93d3.png)

by\_comp.max()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_a7a3967cf385f737.png)

by\_comp.count()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_46917224741fdf9b.png)

by\_comp.describe()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_e5d65674cb6dd8.png)

by\_comp.describe().transpose()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_90188e4fd3ac7380.png)

by\_comp.describe().transpose()[&#39;GOOG&#39;]

Output:

**Sales count 2.000000**
 **mean 160.000000**
 **std 56.568542**
 **min 120.000000**
 **25% 140.000000**
 **50% 160.000000**
 **75% 180.000000**
 **max 200.000000**
**Name: GOOG, dtype: float64**

**CONCLUSION:**

Hence, python programs to perform various operations related to groupby() function using pandas library have been written, executed and output has been verified.

**9. INTRODUCTION TO PANDAS –**

**MERGING, JOINING, CONCATENATING**

**AIM:**

To write a program in python to perform Merging, Joining and Concatenating among different dataframes using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).
 Pandas provides various facilities for easily combining together Series or DataFrame with various kinds of set logic for the indexes and relational algebra functionality in the case of join / merge-type operations.

**Concatenation:**

Concatenation basically glues together DataFrames. The dimensions should match along the axis concatenating on. **pd.concat can be used**  and passed in a list of DataFrames to concatenate together.

## Merging:

The  **merge**  function allows you to merge DataFrames together using a similar logic as merging SQL Tables together.

## Joining:

Joining is a convenient method for combining the columns of two potentially differently-indexed DataFrames into a single result DataFrame.

**PROGRAMS WITH OUTPUT:**

### Example DataFrames:

import pandas as pd

df1 = pd.DataFrame({&#39;A&#39;: [&#39;A0&#39;, &#39;A1&#39;, &#39;A2&#39;, &#39;A3&#39;],
_&#39;B&#39;_: [&#39;B0&#39;, &#39;B1&#39;, &#39;B2&#39;, &#39;B3&#39;],
_&#39;C&#39;_: [&#39;C0&#39;, &#39;C1&#39;, &#39;C2&#39;, &#39;C3&#39;],
_&#39;D&#39;_: [&#39;D0&#39;, &#39;D1&#39;, &#39;D2&#39;, &#39;D3&#39;]},
 index=[0, 1, 2, 3])

df2 = pd.DataFrame({&#39;A&#39;: [&#39;A4&#39;, &#39;A5&#39;, &#39;A6&#39;, &#39;A7&#39;],
_&#39;__B&#39;_: [&#39;B4&#39;, &#39;B5&#39;, &#39;B6&#39;, &#39;B7&#39;],
_&#39;C&#39;_: [&#39;C4&#39;, &#39;C5&#39;, &#39;C6&#39;, &#39;C7&#39;],
_&#39;__D&#39;_: [&#39;D4&#39;, &#39;D5&#39;, &#39;D6&#39;, &#39;D7&#39;]},
 index=[4, 5, 6, 7])

df3 = pd.DataFrame({&#39;A&#39;: [&#39;A8&#39;, &#39;A9&#39;, &#39;A10&#39;, &#39;A11&#39;],
_&#39;__B&#39;_: [&#39;B8&#39;, &#39;B9&#39;, &#39;B10&#39;, &#39;B11&#39;],
_&#39;__C&#39;_: [&#39;C8&#39;, &#39;C9&#39;, &#39;C10&#39;, &#39;C11&#39;],
_&#39;D&#39;_: [&#39;D8&#39;, &#39;D9&#39;, &#39;D10&#39;, &#39;D11&#39;]},
 index=[8, 9, 10, 11])

df1

Output:

![](RackMultipart20210731-4-1qy8gmm_html_14e51a177a2925c3.png)

df2

Output:

![](RackMultipart20210731-4-1qy8gmm_html_2f9a6c032a6d6f67.png)

df3

Output:

![](RackMultipart20210731-4-1qy8gmm_html_41c4bd19496a000a.png)

**Concatenation:**

pd.concat([df1,df2,df3])

Output:

![](RackMultipart20210731-4-1qy8gmm_html_fc0d83b9c520e6d.png)

pd.concat([df1,df2,df3],axis=1)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_dc6782ea7b11501a.png)

**Example DataFrames:**

left = pd.DataFrame({&#39;key&#39;: [&#39;K0&#39;, &#39;K1&#39;, &#39;K2&#39;, &#39;K3&#39;],
_&#39;A&#39;_: [&#39;A0&#39;, &#39;A1&#39;, &#39;A2&#39;, &#39;A3&#39;],
_&#39;B&#39;_: [&#39;B0&#39;, &#39;B1&#39;, &#39;B2&#39;, &#39;B3&#39;]})
right = pd.DataFrame({&#39;key&#39;: [&#39;K0&#39;, &#39;K1&#39;, &#39;K2&#39;, &#39;K3&#39;],
_&#39;C&#39;_: [&#39;C0&#39;, &#39;C1&#39;, &#39;C2&#39;, &#39;C3&#39;],
_&#39;D&#39;_: [&#39;D0&#39;, &#39;D1&#39;, &#39;D2&#39;, &#39;D3&#39;]})
left

Output:

![](RackMultipart20210731-4-1qy8gmm_html_c8716765fbd0743d.png)

Right

Output:

![](RackMultipart20210731-4-1qy8gmm_html_7e3f3a97fafa21ad.png)

## Merging:

pd.merge(left,right,how=&#39;inner&#39;,on=&#39;key&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_60790c0de243a25a.png)

left = pd.DataFrame({&#39;key1&#39;: [&#39;K0&#39;, &#39;K0&#39;, &#39;K1&#39;, &#39;K2&#39;],
_&#39;key2&#39;_: [&#39;K0&#39;, &#39;K1&#39;, &#39;K0&#39;, &#39;K1&#39;],
_&#39;A&#39;_: [&#39;A0&#39;, &#39;A1&#39;, &#39;A2&#39;, &#39;A3&#39;],
_&#39;B&#39;_: [&#39;B0&#39;, &#39;B1&#39;, &#39;B2&#39;, &#39;B3&#39;]})

right = pd.DataFrame({&#39;key1&#39;: [&#39;K0&#39;, &#39;K1&#39;, &#39;K1&#39;, &#39;K2&#39;],
_&#39;key2&#39;_: [&#39;K0&#39;, &#39;K0&#39;, &#39;K0&#39;, &#39;K0&#39;],
_&#39;C&#39;_: [&#39;C0&#39;, &#39;C1&#39;, &#39;C2&#39;, &#39;C3&#39;],
_&#39;D&#39;_: [&#39;D0&#39;, &#39;D1&#39;, &#39;D2&#39;, &#39;D3&#39;]})
pd.merge(left, right, on =[&#39;key1&#39;, &#39;key2&#39;])

Output:

![](RackMultipart20210731-4-1qy8gmm_html_130c44f93feea685.png)

pd.merge(left, right, how=&#39;outer&#39;, on=[&#39;key1&#39;, &#39;key2&#39;])

Output:

![](RackMultipart20210731-4-1qy8gmm_html_b365818f3ce1c344.png)

pd.merge(left, right, how=&#39;right&#39;, on=[&#39;key1&#39;, &#39;key2&#39;])

Output:

![](RackMultipart20210731-4-1qy8gmm_html_4d99782d90a0c58c.png)

pd.merge(left, right, how=&#39;left&#39;, on=[&#39;key1&#39;, &#39;key2&#39;])

Output:

![](RackMultipart20210731-4-1qy8gmm_html_c7bd49914551f00e.png)

## Joining:

left = pd.DataFrame({&#39;A&#39;: [&#39;A0&#39;, &#39;A1&#39;, &#39;A2&#39;],
_&#39;B&#39;_: [&#39;B0&#39;, &#39;B1&#39;, &#39;B2&#39;]},
 index=[&#39;K0&#39;, &#39;K1&#39;, &#39;K2&#39;])
right = pd.DataFrame({&#39;C&#39;: [&#39;C0&#39;, &#39;C2&#39;, &#39;C3&#39;],
_&#39;D&#39;_: [&#39;D0&#39;, &#39;D2&#39;, &#39;D3&#39;]},
 index=[&#39;K0&#39;, &#39;K2&#39;, &#39;K3&#39;])
left.join(right)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_1365fbb0495f7135.png)

left.join(right, how=&#39;outer&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_623b48e0af287b20.png)

**CONCLUSION:**

Hence, python programs to perform Merging, Joining and Concatenating among different dataframes using pandas library have been written, executed and output has been verified.

**10. INTRODUCTION TO PANDAS – DF OPERATIONS**

**AIM:**

To write a program in python to perform various Dataframe operations using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**DF Operations:**

Using pandas, functions like unique, selecting data, applying function to check the removing a column, sorting in ascending or descending order, null values, fill the null positions, and to find pivot are performed.

# PROGRAMS WITH OUTPUT:

import pandas as pd

#
df = pd.DataFrame({&#39;col1&#39;:[1,2,3,4],&#39;col2&#39;:[444,555,666,444],&#39;col3&#39;:[&#39;abc&#39;,&#39;def&#39;,&#39;ghi&#39;,&#39;xyz&#39;]})
df.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ac9adec1556fd0a3.png)

**Info on Unique Values:**

df[&#39;col2&#39;].unique()

**Output:** **array([444, 555, 666], dtype=int64)**

df[&#39;col2&#39;].nunique()

**Output:**  **3**

df[&#39;col2&#39;].value\_counts()

**Output:**

**444 2**
**555 1**
**666 1**
**Name: col2, dtype: int64**

###

### Selecting Data:

_#Select from DataFrame using criteria from multiple columns_
newdf = df[(df[&#39;col1&#39;]\&gt;2) &amp; (df[&#39;col2&#39;]==444)]
newdf

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_5ae24e3cece63120.png)

### Applying Functions:

def times2(x):
return x\*2
df[&#39;col1&#39;].apply(times2)

**Output:**

**0 2**
**1 4**
**2 6**
**3 8**
**Name: col1, dtype: int64**

df[&#39;col3&#39;].apply(len)

**Output:**

**0 3**
**1 3**
**2 3**
**3 3**
**Name: col3, dtype: int64**

df[&#39;col1&#39;].sum()

**Output:**  **10**

**Permanently Removing a Column:**
**del** df[&#39;col1&#39;]
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_35189aa8421dddec.png)

_#Get column and index names_
df.columns

**Output:** **Index([&#39;col2&#39;, &#39;col3&#39;], dtype=&#39;object&#39;)**

df.index

**Output:** **RangeIndex(start=0, stop=4, step=1)**

**Sorting and Ordering a DataFrame:**

df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d21ba6225293a1a2.png)

df.sort\_values(by=&#39;col2&#39;) _#inplace=False by default_

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_f50a657062736063.png)

**Find or Check for Null Values:**

df.isnull()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_a3a5b5fe837f7008.png)

_# Drop rows with NaN Values_
df.dropna()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_187c3d13c30ff0cc.png)

**Filling in NaN values:**

import numpy as np

df = pd.DataFrame({&#39;col1&#39;:[1,2,3,np.nan],
&#39;col2&#39;:[np.nan,555,666,444],
_&#39;col3&#39;_:[&#39;abc&#39;,&#39;def&#39;,&#39;ghi&#39;,&#39;xyz&#39;]})
df.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1fe86ced24592166.png)

df.fillna(&#39;FILL&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_dc9875a454ba387f.png)

data = {&#39;A&#39;:[&#39;foo&#39;,&#39;foo&#39;,&#39;foo&#39;,&#39;bar&#39;,&#39;bar&#39;,&#39;bar&#39;],
_&#39;B&#39;_:[&#39;one&#39;,&#39;one&#39;,&#39;two&#39;,&#39;two&#39;,&#39;one&#39;,&#39;one&#39;],
_&#39;C&#39;_:[&#39;x&#39;,&#39;y&#39;,&#39;x&#39;,&#39;y&#39;,&#39;x&#39;,&#39;y&#39;],
_&#39;D&#39;_:[1,3,2,5,4,1]}
df = pd.DataFrame(data)
df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_b1c545763b0bd809.png)

df.pivot\_table(values=&#39;D&#39;,index=[&#39;A&#39;, &#39;B&#39;],columns=[&#39;C&#39;])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_53cc24a6058e9ed9.png)

**CONCLUSION:**

Hence, python programs to perform various Dataframe operations using pandas library have been written, executed and output has been verified.

**11. INTRODUCTION TO PANDAS –**

**DATA INPUT AND OUTPUT**

**AIM:**

To write a program in python to get variety of file types using pandas library.

**DESCRIPTION:**

**Introduction to Pandas:**

Pandas for data analysis is an extremely powerful version of Excel, and is a [software library](https://en.wikipedia.org/wiki/Software_library) written for the [Python programming language](https://en.wikipedia.org/wiki/Python_(programming_language)) for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and [time series](https://en.wikipedia.org/wiki/Time_series).

**Data Input and Output:**

Pandas can read a variety of file types like csv, excel, html using its pd.read methods

## CSV:

Read a comma-separated values (csv) file into DataFrame and also supports optionally iterating or breaking of the file into chunks.

## Excel:

Pandas can read, write excel files and only imports data. Formulas or images, having images or macros may cause this read\_excel method to crash.

## HTML:

For HTML, htmllib5,lxml, and BeautifulSoup4 needs to be installed.

pip install can be used for Anaconda Distribution (or)

_#In your terminal/command prompt run_
conda install lxml
conda install html5lib
conda install BeautifulSoup4
_#Restart Jupyter Notebook_

**PROGRAMS WITH OUTPUT:**

import numpy as np
import pandas as pd

## CSV:

### CSV Input:

df = pd.read\_csv(&#39;example&#39;)
df

Output:

![](RackMultipart20210731-4-1qy8gmm_html_249074c9f198c3f2.png)

### CSV Output:

df.to\_csv(&#39;example&#39;,index=False)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_f73a031afd69280d.png)

**EXCEL:**

### Excel Input:

pd.read\_excel(&#39;Excel\_Sample.xlsx&#39;,sheetname=&#39;Sheet1&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_303c47c653ac43be.png)

### Excel Output:

df.to\_excel(&#39;Excel\_Sample.xlsx&#39;,sheet\_name=&#39;Sheet1&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_15191f3b54e68c2b.png)

## HTML:

### HTML Input:

df = pd.read\_html(&#39;http://www.fdic.gov/bank/individual/failed/banklist.html&#39;)
df[0]

Output:

![](RackMultipart20210731-4-1qy8gmm_html_cc5ad892a9fccfc9.png)

# ASSIGNMENT:

import pandas as pd

df=pd.read\_csv(&quot;Salaries.csv - Salaries.csv.csv&quot;)
df

1. **Use the .info() method to find out how many entries there are.**

df.info()

 Output:

**\&lt;class &#39;pandas.core.frame.DataFrame&#39;\&gt;**
**RangeIndex: 148654 entries, 0 to 148653**
**Data columns (total 13 columns):**
 **# Column Non-Null Count Dtype**
**--- ------ -------------- -----**
 **0 Id 148654 non-null int64**
 **1 EmployeeName 148654 non-null object**
 **2 JobTitle 148654 non-null object**
 **3 BasePay 148045 non-null float64**
 **4 OvertimePay 148650 non-null float64**
 **5 OtherPay 148650 non-null float64**
 **6 Benefits 112491 non-null float64**
 **7 TotalPay 148654 non-null float64**
 **8 TotalPayBenefits 148654 non-null float64**
 **9 Year 148654 non-null int64**
 **10 Notes 0 non-null float64**
 **11 Agency 148654 non-null object**
 **12 Status 0 non-null float64**
**dtypes: float64(8), int64(2), object(3)**
**memory usage: 14.7+ MB**

1. **Find the Average Basepay.**

df[&#39;BasePay&#39;].mean()

 Output: **66325.44884050643**
2. **Find the highest amount of overtimepay.**

df[&#39;OvertimePay&#39;].max()

 Output: **245131.88**

1. **What is the job title of JOSEPH DRISCOLL? Note: Use all caps, otherwise you may get an answer that doesn&#39;t match up (there is also a lowercase Joseph Driscoll).**

df[df[&#39;EmployeeName&#39;]==&#39;JOSEPH DRISCOLL&#39;][&#39;JobTitle&#39;]

 Output:

**24 CAPTAIN, FIRE SUPPRESSION**
**Name: JobTitle, dtype: object**
2. **How much does JOSEPH DRISCOLL make (including benefits)?**

df[df[&#39;EmployeeName&#39;]==&#39;JOSEPH DRISCOLL&#39;][&#39;TotalPayBenefits&#39;]

 Output:

**24 270324.91**
**Name: TotalPayBenefits, dtype: float64**
3. **What is the name of highest paid person (including benefits)?**

df[df[&#39;TotalPayBenefits&#39;]== df[&#39;TotalPayBenefits&#39;].max()][&#39;EmployeeName&#39;]

 Output:

**0 NATHANIEL FORD**
**Name: EmployeeName, dtype: object**
4. **What is the name of lowest paid person (including benefits)? Do you notice something strange about how much he or she is paid?**

df[df[&#39;TotalPayBenefits&#39;]== df[&#39;TotalPayBenefits&#39;].min()][&#39;EmployeeName&#39;]

 Output:

**148653 Joe Lopez**
**Name: EmployeeName, dtype: object**
5. **What was the average (mean) BasePay of all employees per year? (2011-2014) ?**

df.groupby(&#39;Year&#39;)[&#39;BasePay&#39;].mean()
 Output:
**Year**
**2011 63595.956517**
**2012 65436.406857**
**2013 69630.030216**
**2014 66564.421924**
**Name: BasePay, dtype: float64**
6.
# How many unique job titles are there?[nunique operation]

df[&#39;JobTitle&#39;].nunique()

Output:2159
7.
# How many people have the word Chief in their job title?

**def** chief(values):
 x=values.str.lower()
 count=x.str.contains(&#39;chief&#39;).value\_counts()
print(count)
chief(df[&#39;JobTitle&#39;])

Output:

False 148027
True 627
Name: JobTitle, dtype: int64

**CONCLUSION:**

Hence, python programs to get variety of file types using pandas libraryhave been written, executed and output has been verified.

**12. INTRODUCTION TO MATPLOTLIB**

**AIM:**

To create and customize plots in python using matplotlib, including how to create different types of plots and customize plot colors and labels.

**DESCRIPTION:**

Matplotlib is an excellent 2D and 3D graphics library for generating scientific figures.

Some of the major Pros of Matplotlib are:

- Generally easy to get started for simple plots
- Support for custom labels and texts
- Great control of every element in a figure
- High-quality output in many formats
- Very customizable in general

Matplotlib is used to create reproducible figures programmatically.

### Figure size, aspect ratio and DPI:

Matplotlib allows the aspect ratio, DPI and figure size to be specified when the Figure object is created.
 \* figsize is a tuple of the width and height of the figure in inches
 \* dpi is the dots-per-inch (pixel per inch).

## Saving figures:

Matplotlib can generate high-quality output in a number formats, including PNG, JPG, EPS, SVG, PGF and PDF.
 To save a figure to a file, savefig method is used in the Figure class.

**Legends, labels and titles:**

**Figure titles:**

A title can be added to each axis instance in a figure. To set the title, the set\_title method in the axes instance is used.

**Axis labels:**

Similarly, with the methods set\_xlabel and set\_ylabel, we can set the labels of the X and Y axes.

### Legends:

The label=&quot;label text&quot; keyword argument is used when plots or other objects are added to the figure, and the legend method is used without arguments to add the legend to the figure.

The legend function takes an optional keyword argument loc that can be used to specify where in the figure the legend is to be drawn. The allowed values of loc are numerical codes for the various places the legend can be drawn.

## Setting colors, linewidths, linetypes:

### Colors with MatLab like syntax:

With matplotlib, the colors of lines and other graphical elements can be explained in a number of ways. MATLAB-like syntax is used where &#39;b&#39; means blue, &#39;g&#39; means green, etc.
 The MATLAB API for selecting line styles are also supported: where, for example, &#39;b.-&#39; means a blue line with dots.

### Colors with the color= parameter:

Colors can be defined by their names or RGB hex codes and optionally provide an alpha value using the color and alpha keyword arguments. Alpha indicates opacity.

### Line and marker styles:

To change the line width, the linewidth or lw keyword argument is used. The line style can be selected using the linestyle or ls keyword arguments.

### Control over axis appearance:

## Plot range:

The ranges of the axes can be configured using the set\_ylim and set\_xlim methods in the axis object, or axis(&#39;tight&#39;) for automatically getting &quot;tightly fitted&quot; axes ranges.

**PROGRAMS WITH OUTPUT:**

import matplotlib.pyplot as plt
_#This line helps to see plots in the notebook_
%matplotlib inline

Basic Example:

import numpy as np
x = np.linspace(0, 5, 11)
y = x \*\* 2
x

**Output:**
 **array([0. , 0.5, 1. , 1.5, 2. , 2.5, 3. , 3.5, 4. , 4.5, 5.])**

y

**Output:**
 **array([0. , 0.25, 1. , 2.25, 4. , 6.25, 9. , 12.25, 16. ,** **20.25, 25.])**

**Basic Matplotlib Commands:**

## _#Basic Matplotlib Commands_
plt.plot(x, y, &#39;r&#39;) _# &#39;r&#39; is the color red_
plt.xlabel(&#39;X Axis Title Here&#39;)
plt.ylabel(&#39;Y Axis Title Here&#39;)
plt.title(&#39;String Title Here&#39;)
plt.show()

![](RackMultipart20210731-4-1qy8gmm_html_2cab6dd6295395a4.png)

## Creating Multiplots on Same Canvas:

_# plt.subplot(nrows, ncols, plot\_number)_
plt.subplot(1,2,1)
plt.plot(x, y, &#39;r-&#39;) _# More on color options later_
plt.subplot(1,2,2)
plt.plot(y, x, &#39;g\*-&#39;);

![](RackMultipart20210731-4-1qy8gmm_html_5bdc887e72fab0c.png)

_# Creates blank canvas_
fig = plt.figure()

axes1 = fig.add\_axes([0.1, 0.1, 0.8, 0.8]) _# main axes_
axes2 = fig.add\_axes([0.2, 0.5, 0.4, 0.3]) _# inset axes_

_# Larger Figure Axes 1_
axes1.plot(x, y, &#39;b&#39;)
axes1.set\_xlabel(&#39;X\_label\_axes2&#39;)
axes1.set\_ylabel(&#39;Y\_label\_axes2&#39;)
axes1.set\_title(&#39;Axes 2 Title&#39;)

_# Insert Figure Axes 2_
axes2.plot(y, x, &#39;r&#39;)
axes2.set\_xlabel(&#39;X\_label\_axes2&#39;)
axes2.set\_ylabel(&#39;Y\_label\_axes2&#39;)
axes2.set\_title(&#39;Axes 2 Title&#39;);

![](RackMultipart20210731-4-1qy8gmm_html_293875b07a61a249.png)

## subplots():

_#The plt.subplots() object will act as a more automatic axis manager._
_# Use similar to plt.figure() except use tuple unpacking to grab fig and axes_
fig, axes = plt.subplots()

_# Now use the axes object to add stuff to plot_
axes.plot(x, y, &#39;r&#39;)
axes.set\_xlabel(&#39;x&#39;)
axes.set\_ylabel(&#39;y&#39;)
axes.set\_title(&#39;title&#39;);

![](RackMultipart20210731-4-1qy8gmm_html_a8b45daf4727fe3d.png)

_#Then you can specify the number of rows and columns when creating the subplots() object_
_# Empty canvas of 1 by 2 subplots_
fig, axes = plt.subplots(nrows=1, ncols=2)

![](RackMultipart20210731-4-1qy8gmm_html_bcd38a91a8a314.png)

_# Axes is an array of axes to plot on_
axes

**Output:**

**array([\&lt;matplotlib.axes.\_subplots.AxesSubplot object at 0x000001BDAE69A5C0\&gt;,**
 **\&lt;matplotlib.axes.\_subplots.AxesSubplot object at 0x000001BDAE6C1550\&gt;],**
 **dtype=object)**

_#We can iterate through this array:_

**for** ax in axes:
 ax.plot(x, y, &#39;b&#39;)
 ax.set\_xlabel(&#39;x&#39;)
 ax.set\_ylabel(&#39;y&#39;)
 ax.set\_title(&#39;title&#39;)
_# Display the figure object_
fig

![](RackMultipart20210731-4-1qy8gmm_html_9b51d8a9b85f78b0.png)

_#A common issue with matplolib is overlapping subplots or figures. We can use_ _fig.tight\_layout() or plt.tight\_layout()_ _method, which automatically adjusts the positions of the axes on the figure canvas so that there is no overlapping content._

fig, axes = plt.subplots(nrows=1, ncols=2)
**for** ax in axes:
 ax.plot(x, y, &#39;g&#39;)
 ax.set\_xlabel(&#39;x&#39;)
 ax.set\_ylabel(&#39;y&#39;)
 ax.set\_title(&#39;title&#39;)
fig
plt.tight\_layout()

![](RackMultipart20210731-4-1qy8gmm_html_876ffca35e0cef6d.png)

### Figure size, aspect ratio and DPI:

fig = plt.figure(figsize=(8,4), dpi=100)

**Output:**

**\&lt;Figure size 800x400 with 0 Axes\&gt;**

_#The same arguments can also be passed to layout managers, such as the_ _subplots_ _function_

fig, axes = plt.subplots(figsize=(12,3))

axes.plot(x, y, &#39;r&#39;)
axes.set\_xlabel(&#39;x&#39;)
axes.set\_ylabel(&#39;y&#39;)
axes.set\_title(&#39;title&#39;);

![](RackMultipart20210731-4-1qy8gmm_html_eab25f84d3486ac6.png)

## Saving figures:

fig.savefig(&quot;filename.png&quot;)

_#Here we can also optionally specify the DPI and choose between different output formats_

fig.savefig(&quot;filename.png&quot;, dpi=200)

**Legends, labels and titles:**

**Figure titles:**

ax.set\_title(&quot;title&quot;);

**Axis labels:**

ax.set\_xlabel(&quot;x&quot;)
ax.set\_ylabel(&quot;y&quot;);

### Legends:

fig = plt.figure()
ax = fig.add\_axes([0,0,1,1])
ax.plot(x, x\*\*2, label=&quot;x\*\*2&quot;)
ax.plot(x, x\*\*3, label=&quot;x\*\*3&quot;)
ax.legend()

![](RackMultipart20210731-4-1qy8gmm_html_65258e66119e149c.png)

_# legend overlaps some of the actual plot._

ax.legend(loc=1) _# upper right corner_
ax.legend(loc=2) _# upper left corner_
ax.legend(loc=3) _# lower left corner_
ax.legend(loc=4) _# lower right corner_
ax.legend(loc=0) _# let matplotlib decide the optimal location_
fig

![](RackMultipart20210731-4-1qy8gmm_html_65258e66119e149c.png)

## Setting colors, linewidths, linetypes:

### Colors with MatLab like syntax:

_# MATLAB style line color and style_
fig, ax = plt.subplots()
ax.plot(x, x\*\*2, &#39;b.-&#39;) _# blue line with dots_
ax.plot(x, x\*\*3, &#39;g--&#39;) _# green dashed line_

![](RackMultipart20210731-4-1qy8gmm_html_7dcf94514051063f.png)

### Colors with the color= parameter:

fig, ax = plt.subplots()
ax.plot(x, x+1, color=&quot;blue&quot;, alpha=0.5) _# half-transparant_
ax.plot(x, x+2, color=&quot;#8B008B&quot;) _# RGB hex code_
ax.plot(x, x+3, color=&quot;#FF8C00&quot;) _# RGB hex code_

![](RackMultipart20210731-4-1qy8gmm_html_e202d5cd435c19e8.png)

**Line and marker styles**** :**

fig, ax = plt.subplots(figsize=(12,6))

ax.plot(x, x+1, color=&quot;red&quot;, linewidth=0.25)
ax.plot(x, x+2, color=&quot;red&quot;, linewidth=0.50)
ax.plot(x, x+3, color=&quot;red&quot;, linewidth=1.00)
ax.plot(x, x+4, color=&quot;red&quot;, linewidth=2.00)

_# possible linestype options &#39;-&#39;, &#39;–&#39;, &#39;-.&#39;, &#39;:&#39;, &#39;steps&#39;_
ax.plot(x, x+5, color=&quot;green&quot;, lw=3, linestyle=&#39;-&#39;)
ax.plot(x, x+6, color=&quot;green&quot;, lw=3, ls=&#39;-.&#39;)
ax.plot(x, x+7, color=&quot;green&quot;, lw=3, ls=&#39;:&#39;)

_# custom dash_
line, = ax.plot(x, x+8, color=&quot;black&quot;, lw=1.50)
line.set\_dashes([5, 10, 15, 10]) _# format: line length, space length, ..._

_# possible marker symbols: marker = &#39;+&#39;, &#39;o&#39;, &#39;\*&#39;, &#39;s&#39;, &#39;,&#39;, &#39;.&#39;, &#39;1&#39;, &#39;2&#39;, &#39;3&#39;, &#39;4&#39;, ..._
ax.plot(x, x+ 9, color=&quot;blue&quot;, lw=3, ls=&#39;-&#39;, marker=&#39;+&#39;)
ax.plot(x, x+10, color=&quot;blue&quot;, lw=3, ls=&#39;--&#39;, marker=&#39;o&#39;)
ax.plot(x, x+11, color=&quot;blue&quot;, lw=3, ls=&#39;-&#39;, marker=&#39;s&#39;)
ax.plot(x, x+12, color=&quot;blue&quot;, lw=3, ls=&#39;--&#39;, marker=&#39;1&#39;)

_# marker size and color_
ax.plot(x, x+13, color=&quot;purple&quot;, lw=1, ls=&#39;-&#39;, marker=&#39;o&#39;, markersize=2)
ax.plot(x, x+14, color=&quot;purple&quot;, lw=1, ls=&#39;-&#39;, marker=&#39;o&#39;, markersize=4)
ax.plot(x, x+15, color=&quot;purple&quot;, lw=1, ls=&#39;-&#39;, marker=&#39;o&#39;, markersize=8, markerfacecolor=&quot;red&quot;)
ax.plot(x, x+16, color=&quot;purple&quot;, lw=1, ls=&#39;-&#39;, marker=&#39;s&#39;, markersize=8,
 markerfacecolor=&quot;yellow&quot;, markeredgewidth=3, markeredgecolor=&quot;green&quot;);

![](RackMultipart20210731-4-1qy8gmm_html_b84a5e3603916baf.png)

### Control over axis appearance:

## Plot range:

fig, axes = plt.subplots(1, 3, figsize=(12, 4))

axes[0].plot(x, x\*\*2, x, x\*\*3)
axes[0].set\_title(&quot;default axes ranges&quot;)

axes[1].plot(x, x\*\*2, x, x\*\*3)
axes[1].axis(&#39;tight&#39;)
axes[1].set\_title(&quot;tight axes&quot;)

axes[2].plot(x, x\*\*2, x, x\*\*3)
axes[2].set\_ylim([0, 60])
axes[2].set\_xlim([2, 5])
axes[2].set\_title(&quot;custom axes range&quot;);

![](RackMultipart20210731-4-1qy8gmm_html_f6d301fedc97fd8b.png)

# Special Plot Types:

plt.scatter(x,y)

![](RackMultipart20210731-4-1qy8gmm_html_e792f8edace5ef0.png)

from random import sample
data = sample(range(1, 1000), 100)
plt.hist(data)

**Output:**

**(array([12., 11., 8., 10., 10., 8., 12., 8., 10., 11.]),**
 **array([ 6. , 104.3, 202.6, 300.9, 399.2, 497.5, 595.8, 694.1, 792.4,**
 **890.7, 989. ]),**
 **\&lt;a list of 10 Patch objects\&gt;)**

![](RackMultipart20210731-4-1qy8gmm_html_5c80ead54910957.png)

data = [np.random.normal(0, std, 100) **for** std in range(1, 4)]
_# rectangular box plot_
plt.boxplot(data,vert=True,patch\_artist=True);

![](RackMultipart20210731-4-1qy8gmm_html_ef4f546f89deaee9.png)

# Exercise:Visualizing Titanic dataset

# Step1:Import necessary libraries

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline

# Step2:Read the dataset

data=pd.read\_csv(&quot;Titanic&quot;)
data.head()

![](RackMultipart20210731-4-1qy8gmm_html_1df1b4683b3d97d8.png)

# Step3:Set Passengerid as the index

data.set\_index(&quot;PassengerId&quot;).head()

![](RackMultipart20210731-4-1qy8gmm_html_2b417373d63799e2.png)

# Step4:Visualization

## Line Graph-Age:

plt.figure(figsize=(14,6))
plt.title(&#39;Line Graph-age&#39;)
plt.plot(data[&#39;Age&#39;])

![](RackMultipart20210731-4-1qy8gmm_html_a992744c6f97453c.png)

## Barchart-Survived:

data[&#39;Survived&#39;].value\_counts().plot(kind=&#39;bar&#39;)
plt.xlabel(&#39;Survived&#39;)
plt.ylabel(&#39;Frequency&#39;)
plt.title(&#39;Barchart-Survived&#39;)
plt.legend()

![](RackMultipart20210731-4-1qy8gmm_html_ea4cf6464f16d0d1.png)

## Histogram-Age:

plt.xlabel(&#39;Age&#39;)
plt.ylabel(&#39;Frequency&#39;)
plt.title(&#39;Histogram of age&#39;)
plt.hist(data[&#39;Age&#39;])

![](RackMultipart20210731-4-1qy8gmm_html_c6c788b2b3067631.png)

## Scatterplot-Fare:

plt.scatter(data.Age,data.Fare)
plt.xlabel(&#39;Age&#39;)
plt.ylabel(&#39;Fare&#39;)
plt.title(&#39;Scatterplot-Fare&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_a56c640144cb7517.png)

## Piechart for presenting male/female proportion:

Males=(data[&#39;Sex&#39;]==&#39;male&#39;).sum()
Females=(data[&#39;Sex&#39;]==&#39;female&#39;).sum()
Gender=[Males,Females]

plt.title(&quot;Sex Proportion&quot;)
plt.pie(Gender,colors=[&#39;blue&#39;,&#39;red&#39;],labels=[&#39;Males&#39;,&#39;Females&#39;],
_#with the start angle at 90%_
 startangle=90,
_#with one slide exploded out_
 explode=[0.15,0],
_#with the percent listed as fraction_
 autopct=&#39;%1.1f%%&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_3897405794afbece.png)

**CONCLUSION**

Hence, various plots have been created and customized using matplotlib.

**13. DATA VISUALIZATION USING SEABORN**

**AIM:**

To create and visualize various plots in python using seaborn.

**DESCRIPTION:**

Seaborn is a library for making statistical graphics in Python. It is built on top of matplotlib and closely integrated with pandas data structures.

Seaborn aims to make visualization a central part of exploring and understanding data. Its dataset-oriented plotting functions operate on dataframes and arrays containing whole datasets and internally perform the necessary semantic mapping and statistical aggregation to produce informative plots.

**PLOT TYPES:**

**Lineplot:**

A Line plot is a graph that shows frequency of data along a number line.

**Distplot:**

Flexibly plot a univariate distribution of observations.

**Jointplot:**

Seaborn&#39;s Jointplot displays a relationship between 2 variables (bivariate) as well as 1D profiles (univariate) in the margins.

**Lmplot:**

The Lmplot plot shows the line along with datapoints on the 2d space. By specifying x and y you can set the horizontal and vertical labels respectively.

**Barplot:**

These very similar plots allow you to get aggregate data off a categorical feature in your data. Barplot is a general plot that allows you to aggregate the categorical data based off some function, by default the mean.

**Countplot:**

This is essentially the same as Barplot except the estimator is explicitly counting the number of occurrences which is why we only pass the x value:

**Boxplot and Violinplot:**

Boxplots and Violinplots are used to show the distribution of categorical data. A Box plot (or Box-and-Whisker plot) shows the distribution of quantitative data in a way that facilitates comparisons between variables or across levels of a categorical variable. The box shows the quartiles of the dataset while the whiskers extend to show the rest of the distribution, except for points that are determined to be &quot;outliers&quot; using a method that is a function of the inter-quartile range.

A Violin plot plays a similar role as a box and whisker plot. It shows the distribution of quantitative data across several levels of one (or more) categorical variables such that those distributions can be compared. Unlike a Box plot, in which all of the plot components correspond to actual datapoints, the violin plot features a kernel density estimation of the underlying distribution.

**Stripplot and Swarmplot:**

The Stripplot will draw a scatterplot where one variable is categorical. A Strip plot can be drawn on its own, but it is also a good complement to a box or violin plot in cases where you want to show all observations along with some representation of the underlying distribution.

The Swarmplot is similar to Stripplot, but the points are adjusted (only along the categorical axis) so that they don&#39;t overlap. This gives a better representation of the distribution of values, although it does not scale as well to large numbers of observations (both in terms of the ability to show all the points and in terms of the computation needed to arrange them).

**Factorplot:**

Factorplot is the most general form of a categorical plot. It can take in a kind parameter to adjust the plot type.

**Pairplot:**

Pair Plot ia a simple way to visualize relationships between each variable. It produces a matrix of relationships between each variable for instant examination of data. It can also be used for determining types of regression analysis to use.

**Heatmap:**

Heat maps display numeric tabular data where the cells are colored depending upon the contained value. Heat maps are great for making trends in this kind of data more readily apparent, particularly when the data is ordered and there is clustering.

**PROGRAMS WITH OUTPUT:**

_#Import libraries and read the dataset_

import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline

tips = sns.load\_dataset(&#39;tips&#39;)
tips.head()

![](RackMultipart20210731-4-1qy8gmm_html_3dd278730ef54656.png)

**Lineplot:**

sns.lineplot(data=tips[&#39;size&#39;],label=&#39;size&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_9650d4886fbdd588.png)

**Distplot:**

sns.distplot(tips[&#39;size&#39;],label=&quot;size&quot;)

![](RackMultipart20210731-4-1qy8gmm_html_f26bc164336be22b.png)

**Jointplot:**

sns.jointplot(tips[&#39;total\_bill&#39;],tips[&#39;tip&#39;])

![](RackMultipart20210731-4-1qy8gmm_html_8764de6ab0ce2f1d.png)

**Lmplot:**

sns.lmplot(x=&#39;total\_bill&#39;,y=&#39;tip&#39;,data=tips)

![](RackMultipart20210731-4-1qy8gmm_html_d1c69f8add349724.png)

**Barplot:**

sns.barplot(x=&#39;sex&#39;,y=&#39;total\_bill&#39;,data=tips)

![](RackMultipart20210731-4-1qy8gmm_html_bd25dc52a4f0a1fa.png)

_#You can change the estimator object to your own function, that converts a vector to a scalar:_

sns.barplot(x=&#39;sex&#39;,y=&#39;total\_bill&#39;,data=tips,estimator=np.std)

![](RackMultipart20210731-4-1qy8gmm_html_9736a5fe35261f99.png)

**Countplot** :

sns.countplot(x=&#39;sex&#39;,data=tips)

![](RackMultipart20210731-4-1qy8gmm_html_360b5e9141b92506.png)

**Boxplot:**

sns.boxplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,palette=&#39;rainbow&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_beffa6f5930658f5.png)

_# Can do entire dataframe with orient=&#39;h&#39;_
sns.boxplot(data=tips,palette=&#39;rainbow&#39;,orient=&#39;h&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_486343dee451818d.png)

sns.boxplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, hue=&quot;smoker&quot;,data=tips, palette=&quot;coolwarm&quot;)

![](RackMultipart20210731-4-1qy8gmm_html_e89d93d2da151b91.png)

**Violinplot:**

sns.violinplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,palette=&#39;rainbow&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_f85707a4dc39ca76.png)

sns.violinplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,hue=&#39;sex&#39;,palette=&#39;Set1&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_89707e90f81b388f.png)

sns.violinplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,hue=&#39;sex&#39;,split=True,palette=&#39;Set1&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_da2347c7b92a6356.png)

**Stripplot:**

sns.stripplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips)

![](RackMultipart20210731-4-1qy8gmm_html_980fe6b19d42faed.png)

sns.stripplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,jitter=True)

![](RackMultipart20210731-4-1qy8gmm_html_7ff7c6ef36ac765.png)

sns.stripplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,jitter=True,hue=&#39;sex&#39;,palette=&#39;Set1&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_75f45f67f6ba0acd.png)

sns.stripplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips,jitter=True,hue=&#39;sex&#39;,palette=&#39;Set1&#39;,split=True)

![](RackMultipart20210731-4-1qy8gmm_html_f510551bef72da7c.png)

**Swarmplot:**

sns.swarmplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;, data=tips)

![](RackMultipart20210731-4-1qy8gmm_html_9f113248c216f1ff.png)

sns.swarmplot(x=&quot;day&quot;, y=&quot;total\_bill&quot;,hue=&#39;sex&#39;,data=tips, palette=&quot;Set1&quot;, split=True)

![](RackMultipart20210731-4-1qy8gmm_html_1b1ce19fba5e63ba.png)

**Combining Categorical Plots**** :**

sns.violinplot(x=&quot;tip&quot;, y=&quot;day&quot;, data=tips,palette=&#39;rainbow&#39;)
sns.swarmplot(x=&quot;tip&quot;, y=&quot;day&quot;, data=tips,color=&#39;black&#39;,size=3)

![](RackMultipart20210731-4-1qy8gmm_html_5b88799c163b40f2.png)

**Factorplot:**

sns.factorplot(x=&#39;sex&#39;,y=&#39;total\_bill&#39;,data=tips,kind=&#39;bar&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_1e3dfd26cd98f4a3.png)

**Pairplot:**

sns.pairplot(tips,hue=&#39;sex&#39;)

![](RackMultipart20210731-4-1qy8gmm_html_bc9fe26368a37d80.png)

**Heatmap:**

plt.figure(figsize=(14,10))
sns.heatmap(tips[[&#39;tip&#39;,&#39;size&#39;]])

![](RackMultipart20210731-4-1qy8gmm_html_2854b51e2716dff6.png)

**CONCLUSION**

Hence, various plots have been created and visualized using seaborn.

#

**14.**  **PLOTLY AND CUFFLINKS**

**AIM:**

To write a program in python to create an interactive visualization with plotly and Cufflinks.

**DESCRIPTION:**

Plotly is a library used to create interactive plots which can be used in dashboards or websites. They can be saved as html files or static images.

The [plotly](https://plotly.com/python/) Python library is an interactive, [open-source](https://plotly.com/python/is-plotly-free) plotting library that supports over 40 unique chart types covering a wide range of statistical, financial, geographic, scientific, and 3-dimensional use-cases.

#

# PROGRAMS WITH OUTPUT:

Import Libraries:

import plotly
import cufflinks as cf
import pandas as pd
import numpy as np
_#To display the plots_
%matplotlib inline
_#Enabling the offline mode for interactive plotting locally_
from plotly.offline import download\_plotlyjs,init\_notebook\_mode,plot,iplot
init\_notebook\_mode(connected=True)
cf.go\_offline()

**Read data:**

df=pd.read\_csv(&quot;PRICE.csv&quot;)
df

Output:

![](RackMultipart20210731-4-1qy8gmm_html_b21802eef2ed7ca7.png)

# Simple Plot:

_#The plots are marked in the manner of dataset(based on the index)_
df.iplot()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_87b69a0b4b7e74e0.png)

**Scatter Plot:**

_#The plots are marked in the manner of dataset(based on the index)_
_#Markers need to be specified else line will be taken as default_
df[[&#39;carlength&#39;,&#39;carwidth&#39;,&#39;carheight&#39;,&#39;price&#39;]].iplot(kind = &#39;scatter&#39; , mode = &#39;markers&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_5ac0ce452210f903.png)

_#x and y are specified_
df.iplot(kind=&#39;scatter&#39;,x=&#39;carlength&#39;,y=&#39;price&#39;,mode=&#39;markers&#39;,size=10)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_24ee5c308e192934.png)

# Bar Plots:

df.iplot(kind=&#39;bar&#39;,x=&#39;Affordable&#39;,y=&#39;price&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_95b373a0fac3ce98.png)

_#Gives the count of each data_
df.count().iplot(kind=&#39;bar&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_4460f6607169fe75.png)

_#Gives horizontal view_
df.count().iplot(kind=&#39;barh&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_4fd0ebb9d3b515d9.png)

**Boxplots:**

df.iplot(kind=&#39;box&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_3d6817065ed4c434.png)

# 3d Surfaceplot:

_#gives 3d view of x, y and z axis_
df[[&#39;carlength&#39;,&#39;price&#39;,&#39;carheight&#39;]].iplot(kind = &#39;surface&#39;, colorscale = &#39;rdylbu&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_3dbbe9b85319b07b.png)

# Spreadplot:

_#Shows the spread between two or more than numerical columns at any particular point._
_#Gives the difference between the two values (i.e) spread_
df[[&#39;carlength&#39;,&#39;carheight&#39;]].iplot(kind=&#39;spread&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_69913b619f537b48.png)

# Histogram:

_#Bins to specify the quantity of distribution buckets._
df[&#39;price&#39;].iplot(kind=&#39;hist&#39;,bins=25)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_56359568a57c2e69.png)

# Bubbleplot:

df.iplot(kind=&#39;bubble&#39;,x=&#39;carlength&#39;,y=&#39;carheight&#39;,size=&#39;price&#39;)

Output:

![](RackMultipart20210731-4-1qy8gmm_html_60dd9ce3266dad7d.png)

# scatter\_matrix():

_#Similar to sns.pairplot()_
df.scatter\_matrix()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_100074b87363476c.png)

**CONCLUSION:**

Hence, python programs to create an interactive visualization with plotly and Cufflinks have been executed and output has been verified.

**15. FOLIUM**

**AIM:**

To write a program in python to create a map leaflet using folium.

**DESCRIPTION:**

Folium helps to visualize the coordinates of a area along with measures.
It makes it easy to visualize data that&#39;s been manipulated in Python on an interactive Leaflet map. It enables both the binding of data to a map for choropleth visualizations as well as passing Vincent/Vega visualizations as markers on the map.

**PROGRAMS WITH OUTPUT:**

import numpy as np
import pandas as pd
import folium

district\_wise\_census = pd.read\_csv(&quot;districtwise\_population\_and\_centroids&quot;)
district\_wise\_census.head()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_13f50e92253ac3ab.png)

surat\_city\_long = district\_wise\_census[district\_wise\_census[&quot;District&quot;] == &quot;Surat&quot;].Longitude.values[0]
surat\_city\_lat = district\_wise\_census[district\_wise\_census[&quot;District&quot;] == &quot;Surat&quot;].Latitude.values[0]
m = folium.Map(location=[surat\_city\_lat, surat\_city\_long])
m

Output:

![](RackMultipart20210731-4-1qy8gmm_html_a0ad5f5935b23f70.png)

state\_wise\_centroid = pd.read\_csv(&quot;statewise\_centroids\_2011&quot;)
state\_wise\_centroid.head()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_94c9831099cd10a6.png)

state\_wise\_census = district\_wise\_census.groupby(by=&quot;State&quot;).sum()[[&quot;Population in 2001&quot;,&quot;Population in 2011&quot;]].reset\_index()
state\_wise\_census.head()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_77782c9bc30d7ef4.png)

state\_wise\_centroid.head()

Output:

![](RackMultipart20210731-4-1qy8gmm_html_5fc85783ccb18512.png)

state\_wise\_census = state\_wise\_centroid.merge(state\_wise\_census, left\_on=&quot;State&quot;, right\_on=&quot;State&quot;)
state\_wise\_census

Output:

![](RackMultipart20210731-4-1qy8gmm_html_f6253d982ef38236.png)

center\_lat = state\_wise\_census.mean().Latitude
center\_long = state\_wise\_census.mean().Longitude
m = folium.Map(location=[center\_lat, center\_long], zoom\_start=4.5)
**for** state in state\_wise\_census[&quot;State&quot;].unique():
 state\_census = state\_wise\_census[state\_wise\_census[&quot;State&quot;]==state]
 folium.CircleMarker(
 location=[state\_census.Latitude.values[0], state\_census.Longitude.values[0]],
 radius = float(state\_census[&quot;Population in 2011&quot;].values[0]/1e7),
 popup=&quot;Population 2011 : %s&quot;%state\_census[&quot;Population in 2011&quot;].values[0],
 tooltip = state\_census.State.values[0],
 color=&quot;black&quot;,
 fill\_color=&quot;black&quot;
 ).add\_to(m)

m

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_b7af4ec7a7aec185.png)

**CONCLUSION:**

Hence, python program to create a map leaflet using folium has been executed and output has been verified.

**16.**  **INSTALLATION OF PYSPARK**

**AIM:**

To install PySpark and to run PySpark on jupyter notebook.

**DESCRIPTION:**

PySpark has been released in order to support the collaboration of Apache Spark(written in Scala programming language) and Python, it actually is a Python API for Spark. PySpark also helps to interface with Resilient Distributed Datasets (RDDs) in Apache Spark and Python programming language.

**PySparkSQL:**

A PySpark library used to apply SQL-like analysis on a huge amount of structured or semi-structured data. SQL queries can also be used along with PySparkSQL. It can also be connected to Apache Hive. HiveQL can be also be applied. PySparkSQL is a wrapper over the PySpark core. PySparkSQL introduced the DataFrame, a tabular representation of structured data that is similar to that of a table from a relational database management system.

**PROGRAMS WITH OUTPUT:**

1. **Needed resources:**

1. Spark distribution from [spark.apache.org](https://spark.apache.org/downloads.html)

![](RackMultipart20210731-4-1qy8gmm_html_f13282bc5cbd307f.png)

1. Python and Jupyter Notebook - by installing the Python 3.x version of [Anaconda distribution](https://www.anaconda.com/download/).

1. winutils.exe — a Hadoop binary for Windows — from Steve Loughran&#39;s [GitHub repo](https://github.com/steveloughran/winutils/).
 From the corresponding Hadoop version in the Spark distribution, from winutils.exe under /bin. [https://github.com/steveloughran/winutils/blob/master/hadoop-2.7.1/bin/winutils.exe](https://github.com/steveloughran/winutils/blob/master/hadoop-2.7.1/bin/winutils.exe)

![](RackMultipart20210731-4-1qy8gmm_html_fe98af73e68710d5.png)

1. The _findspark_ Python module, which can be installed by running _python -m pip install findspark_ either in Windows command prompt or Git bash if Python is installed. Command prompt is searched by typing cmd in the search box.

![](RackMultipart20210731-4-1qy8gmm_html_b506a7d5d98abe22.png)

1. If Java is not available or if Java version is 7.x or less, the latest JDK (current version 9.0.1) can be downloaded and installed from [Oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html).

![](RackMultipart20210731-4-1qy8gmm_html_1e980c166dfb832b.png)

1. To unpack the .tgz file on Windows [7-zip](http://www.7-zip.org/download.html) can be by downloaded and installed on Windows

To unpack the .tgz file from Spark distribution, right-click on the file icon and
 select _7-zip \&gt; Extract Here_.

![](RackMultipart20210731-4-1qy8gmm_html_1c0966dffff6e629.png)

1.
## Installing PySpark:

1. Unpack the .tgz file put under _D:\spark\spark-2.2.1-bin-hadoop2.7_

![](RackMultipart20210731-4-1qy8gmm_html_971406a38c7df66e.png)

1. Move the _winutils.exe_ downloaded from step A3 to the _\bin_ folder of Spark distribution. _D:\spark\spark-2.2.1-bin-hadoop2.7\bin\winutils.exe_
2. Add environment variables: Enables Windows to find where the files are when we PySpark kernel gets started. It can be done by finding the environment variable settings by putting &quot;_environ…_&quot; in the search box.

| **Name** | **Value** |
| --- | --- |
| SPARK\_HOME | D:\spark\spark-2.2.1-bin-hadoop2.7 |
| --- | --- |
| HADOOP\_HOME | D:\spark\spark-2.2.1-bin-hadoop2.7 |
| PYSPARK\_DRIVER\_PYTHON | jupyter |
| PYSPARK\_DRIVER\_PYTHON\_OPTS | notebook |

![](RackMultipart20210731-4-1qy8gmm_html_454ee2f459a1c07c.png)

1. In the same environment variable settings window, under the _Path_ or _PATH__ _variable, edit is clicked and _D:\spark\spark-2.2.1-bin-hadoop2.7\bin_ is added to it.

In _Path_  semicolon ; is used to separate the values.

1. Add the installed Java JDK folder from step A5,

_D:\Program Files\Java\jdk1.8.0\_121_

| **Name** | **Value** |
| --- | --- |
| JAVA\_HOME | D:\Progra~1\Java\jdk1.8.0\_121 |
| --- | --- |

If JDK is installed under \Program Files (x86), Progra~1 part is replaced
 by Progra~2 instead.

1. **Running PySpark in Jupyter Notebook:**

Open a Python 3 notebook from Jupyter.

![](RackMultipart20210731-4-1qy8gmm_html_9c0a8a8f36920ec7.png)

#Following code is run:

import findspark
 findspark.init()

_# only run after findspark.init()_
 import pyspark
 from pyspark.sql import SparkSession
 spark = SparkSession.builder.getOrCreate()

df = spark.sql(&#39;&#39;&#39;select &#39;spark&#39; as hello &#39;&#39;&#39;)
 df.show()

When run, a Windows firewall pop-up will appear which can be cancelled. ![](RackMultipart20210731-4-1qy8gmm_html_4823639dcafd7227.png)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_fa142b806f835ccc.png)

**CONCLUSION:**

Hence, PySpark has been installed successfully and has been tested using Jupyter notebook.

**17.**  **INTRODUCTION TO HDF5\_PYTABLE**

**AIM:**

To define own records in Python and save collections of them (i.e. a _table_) into a file.

**DESCRIPTION:**

Hierarchical Data Format (HDF) is a specification and technology for the storage of big numerical data. HDF was created in the supercomputing community and is now an open standard. The latest version of HDF is HDF5. HDF5 structures data in groups and datasets. Datasets are multidimensional homogeneous arrays. Groups can contain other groups or datasets. Groups are like directories in a hierarchical filesystem.

The two main HDF5 Python libraries are:

1. h5y
2. PyTables

PyTables has a number of dependencies:

1. NumPy
2. Numexpr - This package claims that it evaluates multiple-operator array expressions
 many times faster than NumPy can.
3. HDF5

The HDFStore class is the pandas abstraction responsible for dealing with HDF5 data.

**Importing tables objects:**

Public objects in the tables package needs to be imported first. However, PyTables has a contained set of first-level primitives, which can be considered as an alternative. If NumPy arrays are used, functions from the numpy package needs to be imported.

**Declaring a Column Descriptor:**

If a particle detector is available and in order to create a table object for saving data retrieved from it, a table needs to be defined along with number of columns and the kind of object is contained in each column.

Particle detector has a TDC (Time to Digital Converter) counter with a dynamic range of 8 bits and an ADC (Analogical to Digital Converter) with a range of 16 bits. For these values, 2 fields are defined in the record object called TDCcount and ADCcount. To save the grid position in which the particle has been detected, two new fields called grid\_i and grid\_j are added. Instrumentation can also obtain pressure and energy of the particle.

The resolution of the pressure-gauge uses a single-precision float to store pressure readings, while the energy value will need a double-precision float. Finally, to track the particle, a name is assigned to identify the kind of the particle it is along with a unique numeric identifier is given. Hence, two more fields are added:

1. name - string of up to 16 characters
2. idnumber - an integer of 64 bits (which allows to store records for extremely large
 numbers of particles).

A new Particle class that will contain all the above information is declared for each field which is needed along with its value to which an instance of the appropriate Col subclass is assigned, according to the kind of column defined (the data type, the length, the shape, etc). Hence, this Particle instance can be used as a descriptor for the detector data table.

**Creating a PyTables file:**

The top-level _open\_file()_ function is used to create a PyTables file. _open\_file()_ is one of the objects imported by the _`from tables import *`_ statement. This function attempts to open the file, and if successful, returns the File object instance h5file. The root of the object tree is specified in the instance&#39;s root attribute.

**Creating a new group:**

A group called _detector_ is created that branches from the root node. The particle data table is saved in the group. This function creates a new Group object instance that will be assigned to the variable group.

**Creating a new table:**

A Table object is created as a branch off the newly-created group using _File.create\_table()_ method of the h5file object. Hence, a new Table instance is created and assigned to the variable table.

More detailed information can be displayed about the objects and their children by just printing them leading to that introspection capability to be very useful.

The row attribute of table points to the Row instance that will be used to write data rows into the table. A data is written simply by assigning the Row instance, the values for each row as if it were a dictionary (although it is actually an extension class), using the column names as keys.

**Flushing:**

After all data have been processed, the table&#39;s I/O buffer needs to flushed if all this data needs to be written to disk which is achieved by calling the _table.flush()_ method. Flushing is a very important step as it will not only help to maintain the integrity of file, but also will free valuable memory resources (i.e. internal buffers) that the program may need for other things.

**Reading (and selecting) data in a table:**

This task helps to access the data and select from specific columns the values needed. The first line creates a &quot;shortcut&quot; to the readout table deeper on the object tree. The natural naming schema is used to access it.

PyTables do offer other, more powerful ways of performing selections which may be more suitable for very large tables or if a very high query speed is needed. They are called _inkernel_ and _indexed_ queries, which can be used through _Table.where()_ and other related methods.

In-kernel and indexed queries are not only faster, but also, they look more compact, and are among the greatest features for PyTables.

**Closing the file:**

The close method of the h5file File object is used to close the file before exiting Python. Hence, a PyTables file with a table and two arrays have been created which can be examined with any generic HDF5 tool, such as h5dump or h5ls.

**PROGRAMS WITH OUTPUT:**

**Importing tables objects:**

_#Import packages_
conda install -c anaconda hdf5
 pip install numexpr
 pip install tables

import numpy as np
import h5pymatrix1 = np.random.random(size=(1000,1000))
matrix2 = np.random.random(size=(1000,100))

with h5py.File(&quot;I:\\hdf5\_data.h5&quot;,&quot;w&quot;) as hdf:
 hdf.create\_dataset(&#39;dataset1&#39;,data=matrix1)
 hdf.create\_dataset(&#39;dataset2&#39;,data=matrix2)

_#Reading the hdf5_
withh5py.File(&quot;I:\\hdf5\_data.h5&quot;,&quot;r&quot;) as hdf:
 ls=list(hdf.keys())
print(&quot;List of datasets in this file &quot;,ls)
 data = hdf.get(&#39;dataset1&#39;)
 dataset1=np.array(data)
print(&quot;Shape of dataset &quot;,dataset1.shape)

**Output:**

**List of datasets in this file [&#39;dataset1&#39;, &#39;dataset2&#39;]**
**Shape of dataset (1000, 1000)**

![](RackMultipart20210731-4-1qy8gmm_html_4e03c5ccaa1e57ef.png)

**Declaring a Column Descriptor:**

from tables import \*

classParticle(IsDescription):
 name = StringCol(16) _# 16-character String_
 idnumber = Int64Col() _# Signed 64-bit integer_
 ADCcount = UInt16Col() _# Unsigned short integer_
 TDCcount = UInt8Col() _# unsigned byte_
 grid\_i = Int32Col() _# 32-bit integer_
 grid\_j = Int32Col() _# 32-bit integer_
 pressure = Float32Col() _# float (single-precision)_
 energy = Float64Col() _# double (double-precision)_

**Creating a PyTables file:**

_# Tto create a new file in the current working directory called &quot;tutorial2.h5&quot; in &quot;w&quot;rite mode and with a descriptive title string (&quot;Test file&quot;). _
h5file = open\_file(&quot;tutorial2.h5&quot;, mode=&quot;w&quot;, title=&quot;Test file&quot;)

**Creating a new group:**

_#The File instance h5fileis taken and invoked its File.create\_group() method to create a new group called  __detector__  branching from &quot;/&quot; ._
group = h5file.create\_group(&quot;/&quot;, &#39;detector&#39;, &#39;Detector information&#39;)

**Creating a new table:**

_# Node name &quot; __readout__&quot; is assigned to this table.
 # The Particle class declared before is the _ _description__ parameter (to define the columns of the table)
 # &quot;_ _Readout example __&quot; is set as the Table title.__  _
table = h5file.create\_table(group, &#39;readout&#39;,Particle, &quot;Readout example&quot;)

# _To examine the object tree, print the File instance variable __h5file_
_# Dump of the object tree would be displayed and the Group and Table objects which are created can be easily seen_

print(h5file)

**Output:**

**tutorial2.h5 (File) &#39;Test file&#39;**
**Last modif.: &#39;Wed Dec 2 10:46:38 2020&#39;**
**Object Tree:**
**/ (RootGroup) &#39;Test file&#39;**
**/detector (Group) &#39;Detector information&#39;**
**/detector/readout (Table(0,)) &#39;Readout example&#39;**

_# For more information_
h5file

**Output:**

**File(filename=tutorial2.h5, title=&#39;Test file&#39;, mode=&#39;w&#39;, root\_uep=&#39;/&#39;, filters=Filters(complevel=0, shuffle=False, bitshuffle=False, fletcher32=False, least\_significant\_digit=None))**
**/ (RootGroup) &#39;Test file&#39;**
**/detector (Group) &#39;Detector information&#39;**
**/detector/readout (Table(0,)) &#39;Readout example&#39;**
 **description := {**
 **&quot;ADCcount&quot;: UInt16Col(shape=(), dflt=0, pos=0),**
 **&quot;TDCcount&quot;: UInt8Col(shape=(), dflt=0, pos=1),**
 **&quot;energy&quot;: Float64Col(shape=(), dflt=0.0, pos=2),**
 **&quot;grid\_i&quot;: Int32Col(shape=(), dflt=0, pos=3),**
 **&quot;grid\_j&quot;: Int32Col(shape=(), dflt=0, pos=4),**
 **&quot;idnumber&quot;: Int64Col(shape=(), dflt=0, pos=5),**
 **&quot;name&quot;: StringCol(itemsize=16, shape=(), dflt=b&#39;&#39;, pos=6),**
 **&quot;pressure&quot;: Float32Col(shape=(), dflt=0.0, pos=7)}**
 **byteorder := &#39;little&#39;**
 **chunkshape := (1394,)**

_# To get pointer to the Row instance of this table instance_
particle = table.row

_# To write rows_
for i in range(10):
 particle[&#39;name&#39;] = &#39;Particle: %6d&#39; % (i)
 particle[&#39;TDCcount&#39;] = i % 256
 particle[&#39;ADCcount&#39;] = (i \* 256) % (1 \&lt;\&lt; 16)
 particle[&#39;grid\_i&#39;] = i
 particle[&#39;grid\_j&#39;] = 10 - i
 particle[&#39;pressure&#39;] = float(i\*i)
 particle[&#39;energy&#39;] = float(particle[&#39;pressure&#39;] \*\* 4)
 particle[&#39;idnumber&#39;] = i \* (2 \*\* 34)
_# Insert a new particle record_
 particle.append()

**Flushing:**

table.flush()

**Reading (and selecting) data in a table:**

_# Creates a &quot;shortcut&quot; to the  __readout__  table deeper on the object tree_
table = h5file.root.detector.readout

_# Loops over the rows in  __table__  as they are provided by the Table.iterrows() iterator
 # The iterator returns values until all the data in table is exhausted._
 pressure = [x[&#39;pressure&#39;] **for** x in table.iterrows() **if** x[&#39;TDCcount&#39;] \&gt; 3 and 20 \&lt;= x[&#39;pressure&#39;] \&lt; 50]
 pressure

**Output:**
**[25.0, 36.0, 49.0]**

_# Using an in-kernel selection to query the name column for the same set of cuts_
names = [x[&#39;name&#39;] for x in table.where(&quot;&quot;&quot;(TDCcount \&gt; 3) &amp; (20 \&lt;= pressure) &amp; (pressure \&lt; 50)&quot;&quot;&quot;) ]
 names

**Output:**
**[b&#39;Particle: 5&#39;, b&#39;Particle: 6&#39;, b&#39;Particle: 7&#39;]**

**Closing the file:**

h5file.close()
 h5file\_Emp.close()

**EXAMPLE:**

classEmployee(IsDescription):
 name = StringCol(16) _# 16-character String_
 idnumber = Int64Col() _# Signed 64-bit integer_

_# h5file\_Emp = tables.open\_file(&quot;Emp4.h5&quot;, mode=&quot;w&quot;, title=&quot;Emp file&quot;)_
h5file\_Emp = open\_file(&quot;Emp5.h5&quot;, mode=&quot;w&quot;, title=&quot;Emp file&quot;)

![](RackMultipart20210731-4-1qy8gmm_html_db0b106060fab0c4.png)

group1 = h5file\_Emp.create\_group(&quot;/&quot;, &#39;GV&#39;, &#39;SRM&#39;)

_#table = h5file.create\_table(group, &#39;readout&#39;,Particle, &quot;Readout example&quot;)_
table\_Emp = h5file\_Emp.create\_table(group1, &#39;Emp5&#39;,Employee, &quot;EmployeeData&quot;)

print(h5file\_Emp)

**Output:**

**Emp5.h5 (File) &#39;Emp file&#39;**
**Last modif.: &#39;Wed Dec 2 10:53:55 2020&#39;**
**Object Tree:**
**/ (RootGroup) &#39;Emp file&#39;**
**/GV (Group) &#39;SRM&#39;**
**/GV/Emp5 (Table(0,)) &#39;EmployeeData&#39;**

h5file\_Emp

**Output:**

**File(filename=Emp5.h5, title=&#39;Emp file&#39;, mode=&#39;w&#39;, root\_uep=&#39;/&#39;, filters=Filters(complevel=0, shuffle=False, bitshuffle=False, fletcher32=False, least\_significant\_digit=None))**
**/ (RootGroup) &#39;Emp file&#39;**
**/GV (Group) &#39;SRM&#39;**
**/GV/Emp5 (Table(0,)) &#39;EmployeeData&#39;**
 **description := {**
 **&quot;idnumber&quot;: Int64Col(shape=(), dflt=0, pos=0),**
 **&quot;name&quot;: StringCol(itemsize=16, shape=(), dflt=b&#39;&#39;, pos=1)}**
 **byteorder := &#39;little&#39;**
 **chunkshape := (2730,)**

emprow = table\_Emp.row

for i in range(10):
 emprow[&#39;name&#39;] = i
 emprow[&#39;idnumber&#39;] = i
 emprow.append()

table\_Emp.flush()

table\_Emp = h5file\_Emp.root.GV.Emp5

table\_Emp

**Output:**

**/GV/Emp5 (Table(10,)) &#39;EmployeeData&#39;**
 **description := {**
 **&quot;idnumber&quot;: Int64Col(shape=(), dflt=0, pos=0),**
 **&quot;name&quot;: StringCol(itemsize=16, shape=(), dflt=b&#39;&#39;, pos=1)}**
 **byteorder := &#39;little&#39;**
 **chunkshape := (2730,)**

names = [x[&#39;name&#39;] for x in table\_Emp.where(&quot;&quot;&quot;(idnumber \&gt; 3) &quot;&quot;&quot;) ]
names

**Output:**

**[b&#39;4&#39;, b&#39;5&#39;, b&#39;6&#39;, b&#39;7&#39;, b&#39;8&#39;, b&#39;9&#39;]**

h5file\_Emp.close()

**CONCLUSION:**

Hence, records in Python have been defined and saved into a file using PyTable.

**18.**  **INTRODUCTION TO PYSTORE**

**AIM:**

To understand and execute the basics of PyStore.

**DESCRIPTION:**

##
 PyStore, a fast data store for Pandas timeseries data, is a simple (yet powerful) datastore for Pandas dataframes, and while it can store any Pandas object,  **it was designed with storing timeseries data in mind**.

It&#39;s built on top of [Pandas](http://pandas.pydata.org/), [Numpy](http://numpy.pydata.org/), [Dask](http://dask.pydata.org/), and [Parquet](http://parquet.apache.org/) (via [Fastparquet](https://github.com/dask/fastparquet)) in a hierarchical directory structure, to provide an easy to use, fast, powerful, and pythonic datastore for Pandas dataframes that can easily query millions of rows in sub-second speed.Files are compressed using Snappy, a fast and efficient compression/decompression library from Google.

Dask can create DataFrames from various data storage formats like CSV, HDF, Apache Parquet, and others. For most formats, this data can live on various storage systems including local disk, network file systems (NFS), the Hadoop File System (HDFS), and Amazon&#39;s S3 (excepting HDF, which is only available on POSIX like file systems).

Snappy (previously known as Zippy) is a fast data compression and decompression library written in C++ by Google based on ideas from LZ77 and open-sourced in 2011.It does not aim for maximum compression, or compatibility with any other compression library; instead, it aims for very high speeds and reasonable compression. Compression speed is 250 MB/s and decompression speed is 500 MB/s using a single core.

**PROGRAMS WITH OUTPUT:**

**Setting storage path**
 Defaults to ~/pystore or PYSTORE\_PATH environment variable (if set)
 pystore.set\_path(&quot;~/pystore&quot;)

**List stores**
 pystore.list\_stores()

**Connect to datastore (create it if not exist)**
 store = pystore.store(&#39;mydatastore&#39;)

 **List existing collections**
 store.list\_collections()

**Access a collection (create it if not exist)**
 collection = store.collection(&#39;NASDAQ&#39;)

**List items in collection**
 collection.list\_items()

**Load some data from Quandl**
 aapl = quandl.get(&quot;WIKI/AAPL&quot;, authtoken=&quot;your token here&quot;)

**Store the first 100 rows of the data in the collection under &quot;AAPL&quot;**
 collection.write(&#39;AAPL&#39;, aapl[:100], metadata={&#39;source&#39;: &#39;Quandl&#39;})

**Reading the item&#39;s data**
 item = collection.item(&#39;AAPL&#39;) data = item.data # \&lt;-- Dask dataframe (see dask.pydata.org) metadata = item.metadata df = item.to\_pandas()

**Append the rest of the rows to the &quot;AAPL&quot; item**
 collection.append(&#39;AAPL&#39;, aapl[100:])

**Reading the item&#39;s data**
 item = collection.item(&#39;AAPL&#39;) data = item.data metadata = item.metadata df = item.to\_pandas()

**PROGRAMS WITH OUTPUT:**

_# Install package_
pip install quandl
 conda install -c conda-forge snappy
 conda install -c ranaroussi pystore

_# Import libraries_
import quandl
 import pystore

_#__Using Quandl&#39;s API to download 37+ years worth of historical data for Apple&#39;s stock._
aapl = quandl.get(&#39;WIKI/AAPL&#39;)
 aapl.head()

**Output:**![](RackMultipart20210731-4-1qy8gmm_html_c59a9fa2a2c0ef23.png)

_# Storage path_
 pystore.get\_path()

**Output:**
**WindowsPath(&#39;C:/Users/HP/pystore&#39;)**

_# Path can be changed by calling set\_path() mathod
 # Set storage path_
 pystore.set\_path(&#39;./pystore\_demo&#39;)

_# show the new storage path_
 pystore.get\_path()

**Output:**
**&#39;** **WindowsPath(&#39;C:/pystore\_demo&#39;)**

_# Get list of datastores found in this location
 # Since this is a start, output is an empty list
 # List stores_
 pystore.list\_stores()

**Output:
 []**

**Creating / connecting to datastore:**

_# When connecting to a datastore, if it doesn&#39;t exist, it will be automatically created_
store = pystore.store(&#39;mydatastore&#39;)
store

**Output:**
**PyStore.datastore \&lt;C:\pystore\_demo\mydatastore\&gt;**

_# To get a list with the new datastore listed_
pystore.list\_stores()

**Output:
 [&#39;mydatastore&#39;]**

**Creating / connecting to a Collection:**

_# To create a Collection (or namespace) that maps to a directory containing partitioned parquet files for each item (e.g. symbol)
 # When connecting to a collection, if it doesn&#39;t exist, it will be automatically created_ _# Access a collection (create it if not exist)_
 collection = store.collection(&#39;NASDAQ.EOD&#39;)
 collection

**Output:**
**PyStore.collection \&lt;NASDAQ.EOD\&gt;**

_# List can show all the newly created collection_
 store.list\_collections()

**Output:
 [&#39;NASDAQ.EOD&#39;]**

**Working with collection items:**

_# To see if there are any existing items in the collection_
 collection.list\_items()

**Output:
 set()**

_# To store data_
 collection.write(&#39;AAPL&#39;, aapl[:-1], metadata={&#39;source&#39;: &#39;Quandl&#39;},overwrite=True)

_# To list all items in the collections, to see newly created item_
 collection.list\_items()

**Output:
 {&#39;AAPL&#39;}**

_# Read the item&#39;s data_
 item = collection.item(&#39;AAPL&#39;)
 item

**Output:**
**PyStore.item \&lt;NASDAQ.EOD/AAPL\&gt;**

_# data returns a Dask datafram
 # metadata returns the metadata attached to the item, along with an &quot;updated&quot; timestamp_
 data = item.data
 data

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_1edeb64d8fbd3f52.png)

item.metadata

**Output:**
 {&#39;source&#39;: &#39;Quandl&#39;, &#39;\_updated&#39;: &#39;2020-12-09 13:01:11.380157&#39;}

_# To load the item&#39;s data as a Pandas dataframe_
df = item.to\_pandas()
 df.tail()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_541f6e312d9f997d.png)

# To append the last day (row) to item
 collection.append(&#39;AAPL&#39;, aapl[-1:])

 df = collection.item(&#39;AAPL&#39;).to\_pandas()
 df.tail()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_c20c8f7c72333e1c.png)

**Querying Collections:**

_# To look some items up by metadata by adding metadata key to the list\_items method_
 collection.list\_items(source=&#39;Quandl&#39;)

**Output:
 {&#39;AAPL&#39;}**

**Working with Snapshots:**

_# PyStore allows to create snapshots - a point-in-time, named reference for all current items in a collection.
 # To see if there are any existing snapshots_ collection.list\_snapshots()

**Output:
 []**

_# Creating a snapshot using the create\_snapshot method_
 collection.create\_snapshot(&#39;snapshot\_name&#39;)
 collection.list\_snapshots()

**Output:
 [&#39;snapshot\_name&#39;]**

_# To see how snapshots work, original AAPL is changed to only include the Close and Volume columns_
 collection.write(&#39;AAPL&#39;, aapl[[&#39;Close&#39;, &#39;Volume&#39;]], metadata={&#39;source&#39;: &#39;Quandl&#39;}, overwrite=True)
_# Load the &quot;new&quot; item_
 df = collection.item(&#39;AAPL&#39;).to\_pandas()
 df.tail()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_7664ba6dfa61ab92.png)

_# To load the item from a previous snapshot_
 snap\_df = collection.item(&#39;AAPL&#39;, snapshot=&#39;snapshot\_name&#39;)
 snap\_df.to\_pandas().tail()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_c092843ac76de6a6.png)

_# To restore data from snapshot_
 collection.write(&#39;AAPL&#39;, snap\_df,metadata={&#39;source&#39;: &#39;Quandl&#39;},overwrite=True)
 df = collection.item(&#39;AAPL&#39;).to\_pandas()
 df.tail()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1ae2cec475055577.png)

_# Delete a collection snapshot_
 collection.delete\_snapshot(&#39;snapshot\_name&#39;)
_# To delete all snapshots
 # collection.delete\_snapshots()_

**Output:
 True**

**Deleting items, collections and stores:**

_# Delete the item from the current version_
 collection.delete\_item(&#39;AAPL&#39;)

**Output:
 True**

_# Delete the collection_
 store.delete\_collection(&#39;NASDAQ.EOD&#39;)

**Output:
 True**

_# Delete the datastore_
 pystore.delete\_store(&#39;mydatastore&#39;)

_# to delete all datastores in the path
 # pystore.delete\_stores()_

**Output:
 True**

**CONCLUSION:**

Hence, the basics in PyStore has been understood and code has been written, executed and output has been verified.

**19.**  **INTRODUCTION TO JSON**

**AIM:**

To understand, read and write JSON files using Python and Pandas.

**DESCRIPTION:**

JavaScript Object Notation (JSON) is a data format that stores data in a human-readable form. While it can be technically be used for storage, JSON files are primarily used for serialization and information exchange between a client and server. Although it was derived from JavaScript, it&#39;s platform-agnostic and is a widely-spread and used format - most prevalently in REST APIs.

**Creating a JSON File:**

To create JSON files via Python, data has to be stored in a certain way. There are multiple ways of storing this data using Python.

**Creating JSON Data via a Nested Dictionaries:**

In Python, nested dictionaries can be used to create JSON data. Each item inside the outer dictionary corresponds to a column in the JSON file. The key of each item is the column header and the value is another dictionary consisting of rows in that particular column.

**Creating JSON Data via Lists of Dictionaries:**

Another way to create JSON data is via a list of dictionaries. Each item in the list consists of a dictionary and each dictionary represents a row. This approach is a lot more readable than using nested dictionaries.

**Writing Data to a JSON File via Python:**

With nested dictionary and a list of dictionaries, data can be stored in a JSON file. For this, JSON module and dump() method are used.

**Reading JSON Files with Pandas from Local Files**** :**

To read a JSON file via Pandas, the read\_json() method is used and the path to the file to be read is applied to it. The method returns a Pandas Dataframe that stores data in the form of columns and rows.

**Reading JSON from Remote Files:**

The read\_json() method isn&#39;t limited to only reading local files but also used to read JSON files located on remote servers by passing the path of the remote JSON file to the function call.

**Converting Pandas to JSON Data Files:**

To convert a Pandas dataframe to a JSON file, to\_json() function is used on the dataframe, and the path is passed to the soon-to-be file as a parameter.

**PROGRAMS WITH OUTPUT:**

**Creating JSON Data via a Nested Dictionaries:**

_# First item represents Name column.
 # Item value consists of a dictionary where dictionary items represent rows
 # Keys of the inner dictionary items represents index numbers of rows_ patients = {
 &quot;Name&quot;:{&quot;0&quot;:&quot;John&quot;,&quot;1&quot;:&quot;Nick&quot;,&quot;2&quot;:&quot;Ali&quot;,&quot;3&quot;:&quot;Joseph&quot;},
 &quot;Gender&quot;:{&quot;0&quot;:&quot;Male&quot;,&quot;1&quot;:&quot;Male&quot;,&quot;2&quot;:&quot;Female&quot;,&quot;3&quot;:&quot;Male&quot;},
 &quot;Nationality&quot;:{&quot;0&quot;:&quot;UK&quot;,&quot;1&quot;:&quot;French&quot;,&quot;2&quot;:&quot;USA&quot;,&quot;3&quot;:&quot;Brazil&quot;},
 &quot;Age&quot; :{&quot;0&quot;:10,&quot;1&quot;:25,&quot;2&quot;:35,&quot;3&quot;:29}
 }

**Creating JSON Data via Lists of Dictionaries:**

_# Each dictionary items represents a row in a JSON file_
cars = [
 {&quot;Name&quot;:&quot;Honda&quot;, &quot;Price&quot;: 10000, &quot;Model&quot;:2005, &quot;Power&quot;: 1300},
 {&quot;Name&quot;:&quot;Toyota&quot;, &quot;Price&quot;: 12000, &quot;Model&quot;:2010, &quot;Power&quot;: 1600},
 {&quot;Name&quot;:&quot;Audi&quot;, &quot;Price&quot;: 25000, &quot;Model&quot;:2017, &quot;Power&quot;: 1800},
 {&quot;Name&quot;:&quot;Ford&quot;, &quot;Price&quot;: 28000, &quot;Model&quot;:2009, &quot;Power&quot;: 1200},
 ]

**Writing Data to a JSON File via Python:**

import json
 with open(&#39;H:\\patients.json&#39;, &#39;w&#39;) as f:
 json.dump(patients, f)

with open(&#39;H:\\cars.json&#39;, &#39;w&#39;) as f:
 json.dump(cars, f)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_f59b426f7c073498.png)

**Reading JSON Files with Pandas from Local Files**** :**

import pandas as pd
 patients\_df = pd.read\_json(&#39;H:\\patients.json&#39;)
 patients\_df.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_b08aaa864ea8b0c4.png)
 import pandas as pd
 cars\_df = pd.read\_json(&#39;H:\\cars.json&#39;)
 cars\_df.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_8c8ce3c5f983f05a.png)

**Reading JSON from Remote Files:**

import pandas as pd
 iris\_data=pd.read\_json(&quot;https://raw.githubusercontent.com/domoritz/maps/master/data/iris.json&quot;)iris\_data.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_b086b2c378f8a0c6.png)

**Converting Pandas to JSON Data Files:**

_#Load a dataset (seaborn tips dataset)_
import seaborn as sns
 dataset = sns.load\_dataset(&#39;tips&#39;)
 dataset.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_a1723bcb1caee81b.png)

_#_ _Convert the dataset to json file_
dataset.to\_json(&#39;H:\\tips.json&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_3c85974c0325b057.png)

**CONCLUSION:**

Hence, reading and writing of JSON files has been understood and programs have been written and output has been verified.

**20.**  **INTRODUCTION TO RSS\_BEAUTIFULSOUP**

**AIM:**

To understand the data and to do operations of fetching and parsing using Beautifulsoup.

**DESCRIPTION:**

It is possible to extract data from Web and this is called Web Scraping. Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.

[Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/) is a Python library for pulling data (scrape data from the web) out of HTML and XML files.
 It works to provide idiomatic ways of navigating, searching, and modifying the parse tree. It commonly saves hours or days of work.

**PROGRAMS WITH OUTPUT:**
_#_ _Install the Essential Python Libraries_
pip install requests beautifulsoup4

_# Import_ _&quot;requests&quot;__ library to fetch the page content
 # Import bs4 (Beautiful Soup) for parsing the HTML page content_ from bs4 import BeautifulSoup
 import requests

url = &quot;[https://en.wikipedia.org/wiki/List\_of\_countries\_by\_GDP\_(nominal)](https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(nominal))&quot;
_# Make a GET request to fetch the raw HTML content_
 html\_content = requests.get(url).text
_# Parse the html content_
 soup = BeautifulSoup(html\_content, &quot;lxml&quot;)
_# print the parsed data of html_
 print(soup.prettify())

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_4e4944ecfeae1b69.png)

_# Print title of the webpage_
print(soup.title)

**Output:**
**\&lt;title\&gt;List of countries by GDP (nominal) - Wikipedia\&lt;/title\&gt;**

_# To get the text without the HTML tags_
 print(soup.title.text)

**Output:**
**List of countries by GDP (nominal) – Wikipedia**

_# To get all links in the page with attributes (href, title,inner Text)_

for link in soup.find\_all(&quot;a&quot;):

print(&quot;Inner Text: {}&quot;.format(link.text))

print(&quot;Title: {}&quot;.format(link.get(&quot;title&quot;)))

print(&quot;href: {}&quot;.format(link.get(&quot;href&quot;)))

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_7bfbdcf832bcd932.png)

_# First  __tr__  tag is for headings of all three tables_

_# Next  __tr__  tag is for table data for all three inner tables.

 # To get all three table headings_
  gdp\_table = soup.find(&quot;table&quot;, attrs={&quot;class&quot;: &quot;wikitable&quot;})

_# contains 2 rows_

gdp\_table\_data = gdp\_table.tbody.find\_all(&quot;tr&quot;)

_# Get all the headings of Lists_

headings = []

for td in gdp\_table\_data[0].find\_all(&quot;td&quot;):

_# remove any newlines and extra spaces from left and right_

headings.append(td.b.text.replace(&#39;\n&#39;, &#39; &#39;).strip())

print(headings)

**Output:**
**[&#39;Per the International Monetary Fund (2020 estimates)&#39;, &#39;Per the World Bank (2019)&#39;, &#39;Per the United Nations (2019)&#39;]**

_# To get content of all three tables by iterating over each table and its rows_
data = {}

for table, heading in zip(gdp\_table\_data[1].find\_all(&quot;table&quot;), headings):

_# Get headers of table i.e., Rank, Country, GDP_

t\_headers = []

for th in table.find\_all(&quot;th&quot;):

_# remove any newlines and extra spaces from left and right_

t\_headers.append(th.text.replace(&#39;\n&#39;, &#39; &#39;).strip())

_# Get all the rows of table_

table\_data = []

_# find all tr&#39;s from table&#39;s tbody_

for tr in table.tbody.find\_all(&quot;tr&quot;):

t\_row = {}

_# Each table row is stored in the form of_

_# t\_row = {&#39;Rank&#39;: &#39;&#39;, &#39;Country/Territory&#39;: &#39;&#39;, &#39;GDP(US$million)&#39;: &#39;&#39;}_

_# find all td&#39;s(3) in tr and zip it with t\_header_

for td, th in zip(tr.find\_all(&quot;td&quot;), t\_headers):

t\_row[th] = td.text.replace(&#39;\n&#39;, &#39;&#39;).strip()

table\_data.append(t\_row)

_# Put the data for the table with his heading_

data[heading] = table\_data

print(data)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1e7c9c67949d42d6.png)

_# Export to CSV file by iterating over it_
 import csv

 for topic, table in data.items():
 _# Create csv file for each table_
 with open(f&quot;{topic}.csv&quot;, &#39;w&#39;) as out\_file:
 _# Each 3 table has headers as following_
 headers = [
 &quot;Country/Territory&quot;,
 &quot;GDP(US$million)&quot;,
 &quot;Rank&quot;
 ]
_# == t\_headers_
 writer = csv.DictWriter(out\_file, headers)
 _# write the header_
 writer.writeheader()
 for row in table:
 if row:
 writer.writerow(row)

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_cb17a8a0d4f38590.png)

**Example:**

**Importing the libraries:**

from bs4 import BeautifulSoup
 import requests
 import csv

**Sending a HTTP request to a URL:**

url = [https://www.srmist.edu.in/department-of-information-technology/faculty](https://www.srmist.edu.in/department-of-information-technology/faculty)
_# Make a GET request to fetch the raw HTML content_
 html\_content = requests.get(url).text

**Parse the html content:**

soup = BeautifulSoup(html\_content, &quot;lxml&quot;)

**Analyze the HTML tag:**

my\_table = soup.find(&quot;table&quot;, attrs={&quot;class&quot;: &quot;table table-striped hostel-fee&quot;})
 my\_table\_data = my\_table.tbody.find\_all(&quot;tr&quot;)

**Getting the headers:**

headings = []
 for td in my\_table\_data[0].find\_all(&quot;td&quot;):
 headings.append(td.b.text.replace(&#39;\n&#39;, &#39; &#39;).strip())
 headings

**Output:**
**[&#39;FACULTY&#39;, &#39;DESIGNATION&#39;, &#39;RESEARCH INTEREST&#39;]**

**Getting the Data:**

from bs4 import BeautifulSoup
 name\_data =[]
 research\_data=[]
_# find all tr&#39;s from table&#39;s tbody_
 for tr in my\_table.tbody.find\_all(&quot;tr&quot;):
 if(tr.a==None):
 name\_data.append(headings[0])
 research\_data.append(headings[2])
 else:
 name\_data.append(tr.a.text)
 t1=tr.text.replace(&#39;\n&#39;, &#39;&#39;)
 t2=t1.split(&#39;\t&#39;)
 research\_data.append(t2[-1])
_#print(research\_data)_

**Converting the data into csv format:**

import csv
 with open(&#39;file.csv&#39;, &#39;w&#39;) as f:
 writer = csv.writer(f)
 writer.writerows(zip(name\_data, research\_data))

**Displaying the table data:**

import pandas as pd
 df=pd.read\_csv(&#39;file.csv&#39;,encoding= &#39;unicode\_escape&#39;)
 df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d5fa00fa2ee9b235.png)

**CONCLUSION:**

Hence, operations of fetching and parsing using Beautifulsoup has been understood and programs have been written and output has been verified.

**21.**  **INTRODUCTION TO SCRAPY**

**AIM:**

To understand the data and use [Scrapy](https://scrapy.org/) library to scrape data from a website.

**DESCRIPTION:**

It is possible to extract data from Web and this is called Web Scraping. Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.

 Scrapy is an open source and collaborative framework for extracting data from websites in a fast, simple, yet extensible way. It is a framework which allows to focus on the data extraction using CSS selectors and choosing XPath expressions and less on the intricate internals of how spiders are supposed to work. Spiders are classes that are defined and that Scrapy uses to scrape information from a website (or a group of websites).

They must subclass Spider and define the initial requests to make, optionally how to follow links in the pages, and how to parse the downloaded page content to extract data.

 **PROGRAMS WITH OUTPUT:**

_# Settings for notebook_
 from IPython.core.interactiveshell import InteractiveShell
 InteractiveShell.ast\_node\_interactivity = &quot;all&quot;
_# Show Python version_
 import platform
 platform.python\_version()

**Import Scrapy:**

try:

import scrapy

except:

!pip install scrapy

import scrapy

from scrapy.crawler import CrawlerProcess

**Setup a Pipeline:**

_# This class creates a simple pipeline that writes all found items to a JSON file, where each line contains one JSON element_

import json

class JsonWriterPipeline(object):

def open\_spider(self, spider):

self.file = open(&#39;quoteresult.jl&#39;, &#39;w&#39;)

def close\_spider(self, spider):

self.file.close()

def process\_item(self, item, spider):

line = json.dumps(dict(item)) + &quot;\n&quot;

self.file.write(line)

return item

**Define the Spider:**

_# QuotesSpider class defines from which URLs to start crawling and which values to retrieve_

_# Logging level of the crawler is set to warning to avoid DEBUG messages_

import logging

class QuotesSpider(scrapy.Spider):

name = &quot;quotes&quot;

start\_urls = [

&#39;http://quotes.toscrape.com/page/1/&#39;,

&#39;http://quotes.toscrape.com/page/2/&#39;,

]

custom\_settings = {

&#39;LOG\_LEVEL&#39;: logging.WARNING,

&#39;ITEM\_PIPELINES&#39;: {&#39;\_\_main\_\_.JsonWriterPipeline&#39;: 1}, _# Used for pipeline 1_

&#39;FEED\_FORMAT&#39;:&#39;json&#39;, _# Used for pipeline 2_

&#39;FEED\_URI&#39;: &#39;quoteresult.json&#39; _# Used for pipeline 2_

}

def parse(self, response):

for quote in response.css(&#39;div.quote&#39;):

yield {

&#39;text&#39;: quote.css(&#39;span.text::text&#39;).extract\_first(),

&#39;author&#39;: quote.css(&#39;span small::text&#39;).extract\_first(),

&#39;tags&#39;: quote.css(&#39;div.tags a.tag::text&#39;).extract(),

}

**Start the crawler:**

process = CrawlerProcess({

&#39;USER\_AGENT&#39;: &#39;Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 5.1)&#39;

})

process.crawl(QuotesSpider)

process.start()

**Create dataframes:**

import pandas as pd

df = pd.read\_json(&#39;quoteresult.jl&#39;, lines=True)

df.head(10)

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_7a8e4f01e6515b8.png)

**CONCLUSION:**

Hence, scraping of data from website using [Scrapy](https://scrapy.org/) library has been understood and programs have been written and output has been verified.

**22. INTRODUCTION TO**  **WORDCLOUD**

**AIM:**

To understand wordcloud and visualize words in a text using wordcloud.

**DESCRIPTION:**

_Word cloud is a technique for visualising frequent words in a text where the size of the words represents their frequency._ Various arguments for _WordCloud_ function:

1. width/height: The word cloud dimension can be changed to preferred width and height
2. random\_state:  By setting this parameter, reproducibility of the exact same word cloud can be ensured.
3. background\_colour: &#39;white&#39; and &#39;black&#39; are common background colours.
4. colormap: To set up colour theme that the words are displayed in. (eg) &#39;rainbow&#39;, &#39;seismic&#39;, &#39;Pastel1&#39; and Pastel2&#39;.
5. collocations: This is set as _False _to ensure that the word cloud doesn&#39;t appear as if it contains any duplicate words. Otherwise, &#39;web&#39;, &#39;scraping&#39; and &#39;web scraping&#39; is seen as a collocation in the word cloud, giving an impression that words have been duplicated.
6. stopwords: Stopwords are common words which provide little to no value to the meaning of the text. (eg)&#39;We&#39;, &#39;are&#39; and &#39;the&#39;.

**PROGRAMS WITH OUTPUT:**

**Data:**
_# To use text from Wikipedia_
pip install Wikipedia

_# Import packages_
import Wikipedia
 import re
_# Specify the title of the Wikipedia page_
wiki = wikipedia.page(&#39;List\_of\_political\_parties\_in\_India&#39;)
_# Extract the plain text content of the page_
text = wiki.content
_# Clean text_
text = re.sub(r&#39;==.\*?==+&#39;, &#39;&#39;, text)
 text = text.replace(&#39;\n&#39;, &#39;&#39;)
 text

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_7f283cabac95d577.png)

**Wordcloud:**

import matplotlib.pyplot as plt
_# Define a function to plot word cloud_
def plot\_cloud(wordcloud):
 _# Set figure size_
 plt.figure(figsize=(10, 5))
 _# Display image_
 plt.imshow(wordcloud)
 _# No axis details
 # plt.axis(&quot;off&quot;)_

_# Import package_
from wordcloud import WordCloud, STOPWORDS
_# Generate word cloud_
wordcloud = WordCloud(width = 500, height = 500, random\_state=1, background\_color=&#39;white&#39;, colormap=&#39;Set2&#39;, collocations=False, stopwords = STOPWORDS).generate(text)
_# Plot_
 plot\_cloud(wordcloud)
**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_9f5aeb25e1b25044.png)

**Example:**

# Using beautifulsoup
 import requests
 from bs4 import BeautifulSoup

_# url = &quot;_[_https://timesofindia.indiatimes.com/politics/news&quot;_](https://timesofindia.indiatimes.com/politics/news%22)
 _# page\_request = requests.get(url)
 # data = page\_request.content
 # soup = BeautifulSoup(data,&quot;html.parser&quot;)_

soup = BeautifulSoup(requests.get(&quot;https://timesofindia.indiatimes.com/topic/Tamil-Nadu-Election/news&quot;).content,&quot;html.parser&quot;)
 reviews = soup.find(name=&quot;div&quot;, attrs={&#39;class&#39;: &#39;tab\_content&#39;}).ul
 for a in reviews(href = True):
 temp = str(&quot;https://timesofindia.indiatimes.com&quot;+str(a[&#39;href&#39;]))
 print(temp)
 results = [&quot;https://timesofindia.indiatimes.com&quot;+a[&#39;href&#39;] for a in reviews(href=True)]

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_3502ea72c1744b99.png)

_# To derive the content from links_
 import pandas as pd
 import numpy as np
 from newspaper import Article
 for i in results:
 art = Article(i)
 art.download()
 art.parse()
 print(art.text)

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_f8b7f85ad1878c1e.png)

_# To tokenize text_
 import nltk
 raw = art.text
 tokens = nltk.word\_tokenize(raw)
 tokens

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_e1ac55aa61331969.png)

_# To convert tokens to lowercase_
 tokens = [item.lower() for item in tokens]
 tokens

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_b62c74bb9c5c329a.png)

_#To display poltical parties and their members_
 list1=[&#39;dhinakaran&#39;,&#39;jayalalithaa&#39;,&#39;kamal&#39;,&#39;rajinikanth&#39;,&#39;haasan&#39;,&#39;edappadi&#39;,&#39;palanisamy&#39;,&#39;panneerselvam&#39;,&#39;amma&#39;]
 list2=[&#39;aiadmk&#39;,&#39;bjp&#39;,&#39;dmk&#39;,&#39;ammk&#39;]
 Members = [i for i in tokens if i in list1]
 Parties = [i for i in tokens if i in list2]

_# Wordcloud_
 import matplotlib.pyplot as plt
_# Define a function to plot word cloud_
 def plot\_cloud(wordcloud):
 _# Set figure size_
 plt.figure(figsize=(8, 8))
 _# Display image_
 plt.imshow(wordcloud)
 _# No axis details
 # plt.axis(&quot;off&quot;)_

_# Import package_
from wordcloud import WordCloud, STOPWORDS
_# Import packages_
import numpy as np
_# PIL used from importing image_
 from PIL import Image
_# Import image to np.array_
mask = np.array(Image.open(&#39;tamilnadu.jpg&#39;))
_# Generate wordcloud_
wordcloud = WordCloud( background\_color=&#39;WHITE&#39;, collocations=False, stopwords = STOPWORDS, mask=mask).generate(str(tokens))
_# Plot_
 plot\_cloud(wordcloud)
 plt.title(&quot;TAMIL NADU LATEST POLITIC NEWS&quot;, fontdict = {&#39;fontsize&#39; : 10})

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_2702b84a143083c3.png)

_# Display Politic Members
 # Import package_
 from wordcloud import WordCloud, STOPWORDS
_# Generate word cloud_
 wordcloud = WordCloud(width = 300, height = 300, random\_state=1, background\_color=&#39;black&#39;, colormap=&#39;Set2&#39;, collocations=False, stopwords = STOPWORDS).generate(str(Members))
_# Plot_
 plot\_cloud(wordcloud)
 plt.title(&quot;TAMIL NADU POLITIC MEMBERS&quot;, fontdict = {&#39;fontsize&#39; : 10})

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_9e9a0a84f394b4ce.png)

_#_ _Display Political Parties_
_# Import package_
 from wordcloud import WordCloud, STOPWORDS
_# Generate word cloud_
 wordcloud = WordCloud(width = 200, height = 100, random\_state=1, background\_color=&#39;black&#39;, colormap=&#39;Set2&#39;, collocations=False, stopwords = STOPWORDS).generate(str(Parties))
_# Plot_
 plot\_cloud(wordcloud)
 plt.title(&quot;TAMIL NADU POLITIC PARTIES&quot;, fontdict = {&#39;fontsize&#39; : 10})

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_e6a7562f1acf453a.png)

**CONCLUSION:**

Hence, forming wordcloud has been understood and words in a text have been visualized and output has been verified.

**23.**  **INTRODUCTION TO SQLITE**

**AIM:**

To understand SQLite and to do basic operations with it.

**DESCRIPTION:**

[SQL](https://en.wikipedia.org/wiki/SQL) (Structured Query Language) is a domain-specific language used in programming and designed for managing data held in a relational database management system (RDBMS), or for stream processing in a relational data stream management system (RDSMS). It is particularly useful in handling structured data where there are relations between different entities/variables of the data.

SQLite is an in-process library that implements a [self contained](https://www.sqlite.org/selfcontained.html), [serverless](https://www.sqlite.org/serverless.html), [zero configuration](https://www.sqlite.org/zeroconf.html), [transactional](https://www.sqlite.org/transactional.html) SQL database engine. The code for SQLite is in the [public domain](https://www.sqlite.org/copyright.html) and is thus free for use for any purpose, commercial or private.

SQLite is an embedded SQL database engine. Unlike most other SQL databases, SQLite does not have a separate server process. SQLite reads and writes directly to ordinary disk files. A complete SQL database with multiple tables, indices, triggers, and views, is contained in a single disk file. It is a compact library and is [very carefully tested](https://www.sqlite.org/testing.html) prior to every release and has a reputation for being very reliable. Most of the SQLite source code is devoted purely to testing and verification.

**PROGRAMS WITH OUTPUT:**

**Import SQLite:**

_# Import to use SQLite3 module_
import sqlite3

**Create a SQLite Database:**

db = sqlite3.connect(&#39;test.db&#39;)

**Create table:**

cursor = db.cursor()

 cursor.execute(&quot;CREATE TABLE writer(FirstName VARCHAR(50) NOT NULL, LastName VARCHAR(50) NOT NULL, USERID int PRIMARY KEY)&quot;)

cursor.execute(&quot;SELECT name FROM sqlite\_master WHERE type = &#39;table&#39;&quot;).fetchall()

**Output:**

**[(&#39;books&#39;,), (&#39;writer&#39;,)]**

**Insert data:**

cursor.execute(&quot;INSERT INTO writer VALUES (&#39;William&#39;, &#39;Shakespeare&#39;, 1618)&quot;)
 cursor.execute(&quot;INSERT INTO writer VALUES (&#39;Lin&#39;, &#39;Han&#39;, 1997)&quot;)
 cursor.execute(&quot;INSERT INTO writer VALUES (&#39;Peter&#39;, &#39;Brecht&#39;, 1979)&quot;)
cursor.execute(&quot;commit&quot;)

**Write query:**

rows=cursor.execute(&quot;SELECT \* from writer&quot;).fetchall()
 rows

**Output:**
**[(&#39;William&#39;, &#39;Shakespeare&#39;, 1618),
 (&#39;Lin&#39;, &#39;Han&#39;, 1997),
 (&#39;Peter&#39;, &#39;Brecht&#39;, 1979)]**

**Close connection:**

db.close()

**CONCLUSION:**

Hence, basics of SQLite has been understood and programs have been written, executed and output has been verified.

**24.**  **LINEAR REGRESSION**

**AIM:**

To predict and summarize relationships between dependent and independent variable using Linear Regression model.

**DESCRIPTION:**

Creating a model and predicting housing prices for regions in the USA.

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

**Attributes:**

- &#39;Avg. Area Income&#39;: Avg. Income of residents of the city house is located in.
- &#39;Avg. Area House Age&#39;: Avg Age of Houses in same city
- &#39;Avg. Area Number of Rooms&#39;: Avg Number of Rooms for Houses in same city
- &#39;Avg. Area Number of Bedrooms&#39;: Avg Number of Bedrooms for Houses in same city
- &#39;Area Population&#39;: Population of city house is located in
- &#39;Price&#39;: Price that the house sold at
- &#39;Address&#39;: Address for the house

**Regression Evaluation Metrics:**

Here are three common evaluation metrics for regression problems:

**Mean Absolute Error**  (MAE) is the mean of the absolute value of the errors:

1𝑛∑𝑖=1𝑛|𝑦𝑖−𝑦̂ 𝑖|1n∑i=1n|yi−y^i|

**Mean Squared Error**  (MSE) is the mean of the squared errors:

1𝑛∑𝑖=1(𝑦𝑖−𝑦̂ 𝑖)21n∑i=1n(yi−y^i)2

**Root Mean Squared Error**  (RMSE) is the square root of the mean of the squared errors:

1𝑛∑𝑖=1(𝑦𝑖−𝑦̂ 𝑖)21n∑i=1n(yi−y^i)2

Comparing these metrics:

- **MAE**  is the easiest to understand, because it&#39;s the average error.
- **MSE**  is more popular than MAE, because MSE &quot;punishes&quot; larger errors, which tends to be useful in the real world.
- **RMSE**  is even more popular than MSE, because RMSE is interpretable in the &quot;y&quot; units.

All of these are loss functions, because we want to minimize them.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

_# Data preprocessing/numerical calculations_

import numpy as np

_# Read data/import data_

import pandas as pd

_# Mathematic plotting library/plotting data/visualization_

import matplotlib.pyplot as plt

%matplotlib inline

import seaborn as sns

_# Machine Learning model_

from sklearn.linear\_model import LinearRegression

_# For Train/Test operations_

from sklearn.model\_selection import train\_test\_split

**Read dataset:**

USAhousing = pd.read\_csv(&#39;USA\_Housing.csv&#39;)

USAhousing.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_608e9385eddf2fa0.png)

USAhousing.info()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_5012cb6625e6a2b1.png)

USAhousing.describe()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d08c30f98e3f4faf.png)

**Exploratory Data Analysis:**

**Pairplot:**

sns.pairplot(USAhousing)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_bcff5c493d2273d2.png)

**Distplot:**

sns.distplot(USAhousing[&#39;Price&#39;])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_11660cd1ff57aa7c.png)

**Heatmap:**

Heatmap - sns.heatmap(USAhousing.corr())

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_457d9f5c98c45ae.png)

**Model Building:**

**Step1: Determine Input and Output**

X = USAhousing[[&#39;Avg. Area Income&#39;, &#39;Avg. Area House Age&#39;, &#39;Avg. Area Number of Rooms&#39;, &#39;Avg. Area Number of Bedrooms&#39;, &#39;Area Population&#39;]]
 y = USAhousing[&#39;Price&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, y\_train, y\_test = train\_test\_split(X, y, test\_size=0.4, random\_state=101)

**Step3: Fit training data into model**

lm = LinearRegression()
 lm.fit(X\_train,y\_train)

**Output:**

**LinearRegression(copy\_X=True, fit\_intercept=True, n\_jobs=None, normalize=False)**

**Step4: Model Evaluation**

print(lm.intercept\_)
 coeff\_df = pd.DataFrame(lm.coef\_,X.columns,columns=[&#39;Coefficient&#39;])
 coeff\_df

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1a965adccfd0ba74.png)

**Step5: Model Interpretation**

- Holding all other features fixed, a 1 unit increase in  **Avg. Area Income**  is associated with an \*_increase of $21.52 \*_.
- Holding all other features fixed, a 1 unit increase in  **Avg. Area House Age**  is associated with an \*_increase of $164883.28 \*_.
- Holding all other features fixed, a 1 unit increase in  **Avg. Area Number of Rooms**  is associated with an \*_increase of $122368.67 \*_.
- Holding all other features fixed, a 1 unit increase in  **Avg. Area Number of Bedrooms**  is associated with an \*_increase of $2233.80 \*_.
- Holding all other features fixed, a 1 unit increase in  **Area Population**  is associated with an \*_increase of $15.15 \*_.

**Step6: Model Predictions**

predictions = lm.predict(X\_test)

plt.scatter(y\_test,predictions)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d9a1d9b3e88ddddf.png)

sns.distplot((y\_test-predictions),bins=50)

**Output: Residual Histogram**

![](RackMultipart20210731-4-1qy8gmm_html_cd5d0c0c46aeba4a.png)

**Regression Evaluation Metrics:**

print(&#39;MAE:&#39;, metrics.mean\_absolute\_error(y\_test, predictions))
 print(&#39;MSE:&#39;, metrics.mean\_squared\_error(y\_test, predictions))
 print(&#39;RMSE:&#39;, np.sqrt(metrics.mean\_squared\_error(y\_test, predictions)))

**Output:**

**MAE: 82288.22251914957**

**MSE: 10460958907.209501**

**RMSE: 102278.82922291153**

**CONCLUSION** :

Hence, a simple linear regression model to predict and summarize relationships between dependent and independent variable has been created and output has been verified.

**25.**  **LOGISTIC REGRESSION**

**AIM:**

To predict and summarize relationships between dependent and independent variable using Logistic Regression model.

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

**DESCRIPTION:**

Creating a model and predicting the presence or absence of diabetes(outcome) using various attributes.

**Attributes:**

- &#39;Pregnancies&#39;: Total number of pregnancies of patients
- &#39;Glucose&#39;: Glucose level of patients
- &#39;Blood Pressure&#39;: Blood Pressure level of patients
- &#39;Skin Thickness&#39;: Skin Thickness of patients
- &#39;Insulin&#39;: Insulin level of patients
- &#39;BMI&#39;: BMI value of patients
- &#39;DiabetesPedigreeFunction&#39;: DiabetesPedigreeFunction of patients
- &#39;Age&#39;: Age of patients
- &#39;Outcome&#39;: Outcome (0 for diabetes and 1 fro non-diabetes) of patients

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

_# Data preprocessing/numerical calculations_

import numpy as np

_# Read data/import data_

import pandas as pd

import warnings

warnings.filterwarnings(&#39;ignore&#39;)

_# Mathematic plotting library/plotting data/visualization_

import matplotlib.pyplot as plt

%matplotlib inline

import seaborn as sns

_# Machine Learning model_

from sklearn.linear\_model import LogisticRegression

_# For Train/Test operations_

from sklearn.model\_selection import train\_test\_split

_# calculating metrics, confusion matrix and classification report and accuracy score_

from sklearn import metrics

from sklearn.metrics import confusion\_matrix

from sklearn.metrics import classification\_report

from sklearn.metrics import accuracy\_score

**Read dataset:**

df = pd.read\_csv(&#39;diabetes.csv&#39;)
 df.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_1826abc442d4e6c0.png)

df.info()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_e4cd57fbacaf36bf.png)

df.describe()

**Output:**

 ![](RackMultipart20210731-4-1qy8gmm_html_596f96e098ebfd5b.png)

df.isnull().sum()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_a6068be3cf435221.png)

**Exploratory Data Analysis:**

**Heatmap:**

plt.figure(figsize=[15,10])
 sns.heatmap(df.corr(), annot=True)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_27ea5fac2c72e018.png)

**Barplot:**

plt.figure(figsize=[15,10])
 df[&#39;Pregnancies&#39;].value\_counts().plot(kind=&#39;bar&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_c8454212967a0b6d.png)

**Piechart:**

plt.figure(figsize=[10,7])
 df[&#39;Outcome&#39;].value\_counts().plot(kind=&quot;pie&quot;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_b5d1deda337f5a68.png)

**Histogram:**

df.plot(x=&#39;BMI&#39;,y=[&#39;Pregnancies&#39;,&#39;Glucose&#39;,&#39;BloodPressure&#39;,&#39;SkinThickness&#39;],kind=&#39;hist&#39;)
 plt.show()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_54d3be230aaea4b6.png)

**Boxplot:**

plt.figure(figsize=[15,10])
 plt.subplot(3,3,1)
 sns.boxplot(df[&#39;BMI&#39;])
 plt.subplot(3,3,2)
 sns.boxplot(df[&#39;Pregnancies&#39;])
 plt.subplot(3,3,3)
 sns.boxplot(df[&#39;SkinThickness&#39;])
 plt.subplot(3,3,4)
 sns.boxplot(df[&#39;Glucose&#39;])
 plt.subplot(3,3,5)
 sns.boxplot(df[&#39;BloodPressure&#39;])
 plt.subplot(3,3,6)
 sns.boxplot(df[&#39;Insulin&#39;])
 plt.subplot(3,3,7)
 sns.boxplot(df[&#39;DiabetesPedigreeFunction&#39;])
 plt.subplot(3,3,8)
 sns.boxplot(df[&#39;Age&#39;])
 plt.subplot(3,3,9)
 sns.boxplot(df[&#39;Outcome&#39;])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_f68c824f06598877.png)

**Histogram:**

df.plot(kind=&#39;hist&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_7b7a83622e531c1d.png)

**Scatterplot:**

plt.figure(figsize=[15,10])
 plt.scatter(df[&#39;BMI&#39;],df[&#39;SkinThickness&#39;])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_bebc83bde41a97bc.png)

**Pairplot:**

sns.pairplot(df)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_b439e72201f994d0.png)

**Model Building:**

**Step1: Determine Input and Output**

X = df.drop(&#39;Outcome&#39;,axis=1)
 y = df[&#39;Outcome&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, y\_train, y\_test = train\_test\_split(X,y, test\_size=0.30, random\_state=101)

**Step3: Fit training data into model**

 logmodel = LogisticRegression(max\_iter=5000)
 logmodel.fit(X\_train,y\_train)

**Output:**

**LogisticRegression(max\_iter=5000)**

**Step4: Model Evaluation**

predictions = logmodel.predict(X\_test)
 print(classification\_report(y\_test,predictions)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ed98c506e52bfa9e.png)

confusion\_matrix(y\_test,predictions)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_6dd05d7a4f134011.png)

accuracy\_score(y\_test,predictions)

**Output:**

**0.7835497835497836**

**CONCLUSION** :

Hence, a logistic regression model to predict and summarize relationships between dependent and independent variable has been created and output has been verified.

**26.**  **KNN**

**AIM:**

To create a model to classify target class for classified data, depending on different independent variables.

**DESCRIPTION:**

K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions).

Creating a model and classifying target class for classified data, depending on different independent variables.

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

_# Data preprocessing/numerical calculations_

import numpy as np

_# Read data/import data_

import pandas as pd

import warnings

warnings.filterwarnings(&#39;ignore&#39;)

_# Mathematic plotting library/plotting data/visualization_

import matplotlib.pyplot as plt

%matplotlib inline

_# Machine Learning model_

from sklearn.neighbors import KNeighborsClassifier

_# For Train/Test operations_

from sklearn.model\_selection import train\_test\_split

_# calculating metrics, confusion matrix, classification report and accuracy score_

from sklearn import metrics

from sklearn.metrics import confusion\_matrix

from sklearn.metrics import classification\_report

from sklearn.metrics import accuracy\_score

**Read dataset:**

df = pd.read\_csv(&#39;Classified Data&#39;)
 df.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_4a10d1da069106d8.png)

**Model Building:**

**Step1: Determine Input and Output**

X = df.drop(&#39;TARGET CLASS&#39;,axis=1)
 y = df[&#39;TARGET CLASS&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, y\_train, y\_test = train\_test\_split(X,y, test\_size=0.30, random\_state=101)

**Step3: Fit training data into model**

knn = KNeighborsClassifier(n\_neighbors=1)
 knn.fit(X\_train, y\_train)

**Output:**

**KNeighborsClassifier(n\_neighbors=1)**

**Step4: Model Evaluation**

pred = knn.predict(X\_test)
 print(classification\_report(y\_test, pred))

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_3cb98e7ab22e720.png)

confusion\_matrix(y\_test, pred)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_7bb06e709d053e2.png)

accuracy\_score(y\_test, pred)

**Output:**

**0.54**

The KNN model varies with different K values thus figuring out the optimum K value will give us better results for our model.

Two ways to find out the K values is as follows:

**Graphical Representation of the accuracy&#39;s method:**

accuracy = []

for i in range(1,40):

knn = KNeighborsClassifier(n\_neighbors=i)

knn.fit(X\_train, y\_train)

pred\_i = knn.predict(X\_test)

accuracy.append(accuracy\_score(y\_test, pred\_i))

# Plotting graph

plt.figure(figsize=(10,6))

plt.plot(range(1,40), accuracy, color=&#39;blue&#39;, linestyle=&#39;dashed&#39;,marker=&#39;o&#39;, markerfacecolor=&#39;red&#39;, markersize=10)

plt.title(&#39;Error rate vs K value&#39;)

plt.xlabel(&#39;K&#39;)

plt.ylabel(&#39;Error rate&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_363d75fd94698415.png)

**Confusion matrix method:**

_#Calculating the sensitivity, specificity, accuracy for different K values_

df\_threshold = pd.DataFrame( columns = [&#39;K-Value&#39;,&#39;accuracy&#39;,&#39;sensitivity&#39;,&#39;specificity&#39;])

num = []

for i in range(1,25):

num.append(i)

for i in num:

knn = KNeighborsClassifier(n\_neighbors=i)

knn.fit(X\_train, y\_train)

pred\_i = knn.predict(X\_test)

cm1 =confusion\_matrix(y\_test, pred\_i)

acc = accuracy\_score(y\_test,pred\_i)

speci = cm1[0,0]/(cm1[0,0]+cm1[0,1])

sensi = cm1[1,1]/(cm1[1,0]+cm1[1,1])

df\_threshold.loc[i] =[i ,acc,sensi,speci]

print(df\_threshold)

df\_threshold.plot(x=&#39;K-Value&#39;, y=[&#39;accuracy&#39;,&#39;sensitivity&#39;,&#39;specificity&#39;])

plt.show()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_39cc6e72a2ea72ba.png)

**CONCLUSION** :

Hence, a KNN model to classify target class for classified data, depending on different independent variables has been created and output has been verified.

**27.**  **DECISION TREES AND VISUALIZATION**

**AIM:**

To predict and summarize relationships between dependent and independent variable using decision tree model and visualize it.

**DESCRIPTION:**

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, decision tress and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

Decision trees are a popular supervised learning method for a variety of reasons. Benefits of decision trees include that they can be used for both regression and classification, they don&#39;t require feature scaling, and they are relatively easy to interpret as decision trees can be visualized. This is not only a powerful way to understand model, but also to communicate how model works. Consequently, it would help to know how to make a visualization based on the model.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

_# Data preprocessing/numerical calculations_

import numpy as np

_# Read data/import data_

import pandas as pd

import warnings

warnings.filterwarnings(&#39;ignore&#39;)

_# Mathematic plotting library/plotting data/visualization_

import matplotlib.pyplot as plt

%matplotlib inline

_# from sklearn.datasets import load\_iris_

from sklearn.datasets import load\_iris

_# Machine Learning model_

from sklearn import tree

from sklearn.tree import DecisionTreeClassifier

_# For Train/Test operations_

from sklearn.model\_selection import train\_test\_split

**Read dataset:**

from sklearn.datasets import load\_iris
 data = load\_iris()
 df = pd.DataFrame(data.data, columns=data.feature\_names)
 df[&#39;target&#39;] = data.target
 df.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_7356500e19a52bd0.png)

**Model Building:**

**Step1: Determine Input and Output**

X = df[data.feature\_names]
 Y = df[&#39;target&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, Y\_train, Y\_test = train\_test\_split(X, Y, random\_state=0)

**Step3: Fit training data into model**

_# Import the model you want to use_
 from sklearn.tree import DecisionTreeClassifier
_# Make an instance of the Model_
 clf = DecisionTreeClassifier(max\_depth = 2,random\_state = 0)
_# Train the model on the data_
 clf.fit(X\_train, Y\_train)

**Output:**

**DecisionTreeClassifier(max\_depth=2, random\_state=0)**

**Step4: Model Evaluation**

_# Predict labels of unseen (test) data_
 clf.predict(X\_test)

**Output:**

**array([2, 1, 0, 2, 0, 2, 0, 1, 1, 1, 2, 1, 1, 1, 1, 0, 1, 1, 0, 0, 1, 1,**

**0, 0, 1, 0, 0, 1, 1, 0, 2, 1, 0, 1, 2, 1, 0, 2])**

**Visualization:**

_# Entropy is a measure of disorder or uncertainty
 # Goal of machine learning models is to reduce uncertainty_
 tree.plot\_tree(clf);

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ae2cc66ae8c08307.png)

fn=[&#39;sepal length (cm)&#39;,&#39;sepal width (cm)&#39;,&#39;petal length (cm)&#39;,&#39;petal width (cm)&#39;]
 cn=[&#39;setosa&#39;, &#39;versicolor&#39;, &#39;virginica&#39;]
 fig, axes = plt.subplots(nrows = 1,ncols = 1,figsize = (2,2), dpi=300)
 tree.plot\_tree(clf,
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 #fig.savefig(&#39;dt1.png&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_3168e76d083c6da4.png)

**Example:**

**Import libraries:**

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

%matplotlib inline
 from sklearn.model\_selection import train\_test\_split

**Read dataset:**

df = pd.read\_csv(&#39;kyphosis.csv&#39;)
 df.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_a184d22d0b16b325.png)

**Exploratory Data Analysis:**

sns.pairplot(df,hue=&#39;Kyphosis&#39;,palette=&#39;Set1&#39;)

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_61ba1b2677aae23a.png)

**Model Building:**

**Step1: Determine Input and Output**

X = df.drop(&#39;Kyphosis&#39;,axis=1)
 y = df[&#39;Kyphosis&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, y\_train, y\_test = train\_test\_split(X, y, test\_size=0.30)

**Step3: Fit training data into model**

_# Import the model you want to use_
 from sklearn.tree import DecisionTreeClassifier
_# Make an instance of the Model_
 dtree = DecisionTreeClassifier()
_# Train the model on the data_
 dtree.fit(X\_train,y\_train)

**Output:**

**DecisionTreeClassifier()**

**Step4: Model Evaluation**

_# Predict labels of unseen (test) data_
 predictions = dtree.predict(X\_test)
 from sklearn.metrics import classification\_report,confusion\_matrix
 print(classification\_report(y\_test,predictions))

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_3b8f57f9c10da1df.png)

print(confusion\_matrix(y\_test,predictions))

**Output:**
**[[19 4]
 [0 2]]**

**Tree Visualization:**

from sklearn import tree
 tree.plot\_tree(dtree)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_8f42b73a654446b1.png)

fn=[&#39;Age&#39;,&#39;Number&#39;,&#39;Start&#39;]
 cn=[&#39;absent&#39;, &#39;present&#39;]
 fig, axes = plt.subplots(nrows = 1,ncols = 1,figsize = (4,4), dpi=300)
 tree.plot\_tree(dtree,
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 fig.savefig(&#39;dt1.png&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_cc7484b9cfc27013.png)

**CONCLUSION** :

Hence, decision tree model to predict and summarize relationships between dependent and independent variable has been created and output has been visualized and verified.

**28.**  **RANDOM FOREST**

**AIM:**

To predict and summarize relationships between dependent and independent variable using random forest and visualize it.

**DESCRIPTION:**

Scikit-learn is a free machine learning library for Python which features various algorithms like support vector machine, random forests, decision tress and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy.

A random forest randomly selects observations/rows and specific features/variables to build multiple decision trees from and then averages the results. After a large number of trees are built using this method, each tree &quot;votes&quot; or chooses the class, and the class receiving the most votes by a simple majority is the &quot;winner&quot; or predicted class.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

%matplotlib inline
 from sklearn.model\_selection import train\_test\_split

**Read dataset:**

df = pd.read\_csv(&#39;kyphosis.csv&#39;)
 df.head()

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_a184d22d0b16b325.png)

**Exploratory Data Analysis:**

sns.pairplot(df,hue=&#39;Kyphosis&#39;,palette=&#39;Set1&#39;)

**Output:**
 ![](RackMultipart20210731-4-1qy8gmm_html_61ba1b2677aae23a.png)

**Model Building:**

**Step1: Determine Input and Output**

X = df.drop(&#39;Kyphosis&#39;,axis=1)
 y = df[&#39;Kyphosis&#39;]

**Step2: Splitting data**

_#Data is split into a training set and a testing set.
 #Train set to train out model
 #Test set to evaluate the model._

X\_train, X\_test, y\_train, y\_test = train\_test\_split(X, y, test\_size=0.30)

**Step3: Fit training data into model**

_# Import the model you want to use_
 from sklearn.ensemble import RandomForestClassifier
_# Make an instance of the Model_
 rfc = RandomForestClassifier(n\_estimators=100)
_# Train the model on the data_
 rfc.fit(X\_train, y\_train)

**Output:**

**RandomForestClassifier(bootstrap=True, class\_weight=None, criterion=&#39;gini&#39;,**

**max\_depth=None, max\_features=&#39;auto&#39;, max\_leaf\_nodes=None,**

**min\_impurity\_decrease=0.0, min\_impurity\_split=None,**

**min\_samples\_leaf=1, min\_samples\_split=2,**

**min\_weight\_fraction\_leaf=0.0, n\_estimators=100,**

**n\_jobs=None, oob\_score=False, random\_state=None,**

**verbose=0, warm\_start=False)**

**Step4: Model Evaluation**

_#_ _Predict labels of unseen (test) data_
 rfc\_pred = rfc.predict(X\_test)
 from sklearn.metrics import classification\_report,confusion\_matrix
 print(classification\_report(y\_test,rfc\_pred))

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_70142c1b52e22488.png)

print(confusion\_matrix(y\_test,rfc\_pred))

**Output:**
**[[19 3]
 [2 1]]**

**Tree Visualization:**

1. from sklearn import tree
 fn=[&#39;Age&#39;,&#39;Number&#39;,&#39;Start&#39;]
 cn=[&#39;absent&#39;, &#39;present&#39;]
 fig, axes = plt.subplots(nrows = 1,
 ncols = 1,
 figsize = (4,4),
 dpi=300)
 tree.plot\_tree(rfc.estimators\_[0],
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 fig.savefig(&#39;dt2.png&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ea4b8d66dcd75f39.png)

1. fn=[&#39;Age&#39;,&#39;Number&#39;,&#39;Start&#39;]
 cn=[&#39;absent&#39;, &#39;present&#39;]
 fig, axes = plt.subplots(nrows = 1,
 ncols = 1,
 figsize = (4,4),
 dpi=300)
 tree.plot\_tree(rfc.estimators\_[1],
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 fig.savefig(&#39;dt3.png&#39;)

1. fn=[&#39;Age&#39;,&#39;Number&#39;,&#39;Start&#39;]
 cn=[&#39;absent&#39;, &#39;present&#39;]
 fig, axes = plt.subplots(nrows = 1,
 ncols = 1,
 figsize = (4,4),
 dpi=300)
 tree.plot\_tree(rfc.estimators\_[2],
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 fig.savefig(&#39;dt4.png&#39;)

**Output:**![](RackMultipart20210731-4-1qy8gmm_html_1004881f15c8de0c.png)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_2dcf2d33e860f73b.png)

1. fn=[&#39;Age&#39;,&#39;Number&#39;,&#39;Start&#39;]
 cn=[&#39;absent&#39;, &#39;present&#39;]
 fig, axes = plt.subplots(nrows = 1,
 ncols = 1,
 figsize = (4,4),
 dpi=300)
 tree.plot\_tree(rfc.estimators\_[3],
 feature\_names = fn,
 class\_names=cn,
 filled = True);
 fig.savefig(&#39;dt5.png&#39;)

**Output:**![](RackMultipart20210731-4-1qy8gmm_html_d089c3b3bec8dcc8.png)

**CONCLUSION** :

Hence, random forest model to predict and summarize relationships between dependent and independent variable has been created and output has been visualized and verified.

**29.**  **K-MEANS CLUSTERING**

**AIM:**

To identify clusters in the data, understand, predict model using K-Means and to visualize it.

**DESCRIPTION:**

K-means clustering is one of the simplest and popular unsupervised machine learning algorithms. Typically, unsupervised algorithms make inferences from datasets using only input vectors without referring to known, or labelled, outcomes.

The objective of K-means is to group similar data points together and discover underlying patterns. To achieve this, K-means looks for a fixed number (_k_) of clusters in a dataset. A cluster refers to a collection of data points aggregated together because of certain similarities.

A target number _k__is defined_, which refers to the number of centroids needed in the dataset. A centroid is the imaginary or real location representing the center of the cluster. Every data point is allocated to each of the clusters through reducing the in-cluster sum of squares. In other words, the K-means algorithm identifies _k_ number of centroids, and then allocates every data point to the nearest cluster, while keeping the centroids as small as possible. The _&#39;means&#39;_ in the K-means refers to averaging of the data; that is, finding the centroid.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

import seaborn as sns
 import matplotlib.pyplot as plt
 %matplotlib inline

**Read dataset:**

from sklearn.datasets import make\_blobs
 data = make\_blobs(n\_samples=200, n\_features=2,
 centers=4, cluster\_std=1.8,random\_state=101)

data[0][:10,0]

**Output:**

**array([ -6.42884095, 5.86867888, -0.37610937, 2.16679181,**

**5.0950857 , -10.87888819, 2.03405554, -1.71798771,**

**1.16911341, -1.35185444])**

**Visualization:**

plt.scatter(data[0][:,0],data[0][:,1])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_7bd4f2152bb431e4.png)

plt.scatter(data[0][:,0],data[0][:,1],c=data[1],cmap=&#39;rainbow&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_228560364e9ae8fd.png)

**Cluster Creation:**

from sklearn.cluster import KMeans
 kmeans = KMeans(n\_clusters=4)
 kmeans.fit(data[0])

**Output:**

**KMeans(n\_clusters=4)**

kmeans.cluster\_centers\_

**Output:**

**array([[3.71749226, 7.01388735],**

**[-9.46941837, -6.56081545],**

**[-4.13591321, 7.95389851],**

**[-0.0123077 , 2.13407664]])**

kmeans.labels\_

**Output:**

**array([2, 0, 3, 0, 0, 1, 0, 3, 0, 3, 2, 3, 0, 0, 2, 3, 0, 3, 1, 2, 1, 3,**

**3, 1, 2, 1, 1, 3, 0, 0, 2, 1, 0, 3, 3, 2, 1, 1, 1, 3, 1, 2, 2, 2,**

**3, 0, 2, 3, 1, 3, 3, 2, 0, 3, 1, 2, 3, 3, 2, 0, 1, 0, 1, 2, 0, 3,**

**1, 0, 0, 1, 0, 3, 1, 3, 1, 0, 0, 3, 2, 3, 3, 1, 0, 1, 3, 3, 3, 2,**

**3, 1, 1, 1, 1, 3, 3, 1, 0, 2, 1, 0, 3, 1, 3, 3, 0, 3, 1, 0, 1, 1,**

**0, 2, 2, 0, 1, 0, 2, 2, 0, 2, 3, 2, 3, 2, 3, 0, 2, 3, 1, 2, 2, 2,**

**3, 1, 1, 2, 0, 2, 0, 3, 1, 0, 1, 2, 2, 0, 3, 1, 2, 2, 2, 2, 3, 0,**

**3, 2, 0, 0, 0, 3, 0, 3, 3, 2, 1, 2, 3, 0, 2, 3, 0, 3, 2, 0, 3, 2,**

**0, 0, 1, 0, 2, 1, 1, 2, 1, 1, 1, 1, 1, 3, 1, 0, 0, 2, 1, 3, 0, 0,**

**1, 3])**

f, (ax1, ax2) = plt.subplots(1, 2, sharey=True,figsize=(10,6))
 ax1.set\_title(&#39;K Means&#39;)
 ax1.scatter(data[0][:,0],data[0][:,1],c=kmeans.labels\_,cmap=&#39;rainbow&#39;)
 ax2.set\_title(&quot;Original&quot;)
 ax2.scatter(data[0][:,0],data[0][:,1],c=data[1],cmap=&#39;rainbow&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_d757dbbf9bd96d15.png)

**CONCLUSION** :

Hence, clusters in the data has been identified, model has been understood and output has been visualized and verified.

**30.**  **PRINCIPAL COMPONENT ANALYSIS**

**AIM:**

To reduce set of variables and to analyze and interpret the data using Principal Component Analysis(PCA).

**DESCRIPTION:**

Principal Component Analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets, by transforming a large set of variables into a smaller one that still contains most of the information in the large set.

Reducing the number of variables of a data set naturally comes at the expense of accuracy, but the trick in dimensionality reduction is to trade a little accuracy for simplicity. Because smaller data sets are easier to explore and visualize and make analyzing data much easier and faster for machine learning algorithms without extraneous variables to process.

Main idea of PCA is to reduce the number of variables of a data set, while preserving as much information as possible.

**STANDARDIZATION:**

The aim is to standardize the range of the continuous initial variables so that each one of them contributes equally to the analysis.

More specifically, the reason why it is critical to perform standardization prior to PCA, is that the latter is quite sensitive regarding the variances of the initial variables. That is, if there are large differences between the ranges of initial variables, those variables with larger ranges will dominate over those with small ranges (For example, a variable that ranges between 0 and 100 will dominate over a variable that ranges between 0 and 1), which will lead to biased results. So, transforming the data to comparable scales can prevent this problem.

Mathematically, this can be done by subtracting the mean and dividing by the standard deviation for each value of each variable.

![](RackMultipart20210731-4-1qy8gmm_html_ab779481c17966e7.png)

Once the standardization is done, all the variables will be transformed to the same scale.

**PROGRAMS WITH OUTPUT:**

**Import libraries:**

import matplotlib.pyplot as plt

import pandas as pd

import numpy as np

import seaborn as sns

%matplotlib inline

**Read dataset:**

_# Cancer data_

from sklearn.datasets import load\_breast\_cancer

cancer = load\_breast\_cancer()

cancer.keys()

**Output:**

**dict\_keys([&#39;data&#39;, &#39;target&#39;, &#39;frame&#39;, &#39;target\_names&#39;, &#39;DESCR&#39;, &#39;feature\_names&#39;, &#39;filename&#39;])**

print(cancer[&#39;DESCR&#39;])

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_975097b3124500d8.png)

df = pd.DataFrame(cancer[&#39;data&#39;],columns=cancer[&#39;feature\_names&#39;])

df.head()

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_bf44ba1cf228223e.png)

**Standardization:**

from sklearn.preprocessing import StandardScaler
 scaler = StandardScaler()
 scaler.fit(df)
 scaled\_data = scaler.transform(df)
 scaled\_data

**Output:**

**array([[ 1.09706398, -2.07333501, 1.26993369, ..., 2.29607613,**

**2.75062224, 1.93701461],**

**[ 1.82982061, -0.35363241, 1.68595471, ..., 1.0870843 ,**

**-0.24388967, 0.28118999],**

**[ 1.57988811, 0.45618695, 1.56650313, ..., 1.95500035,**

**1.152255 , 0.20139121],**

**...,**

**[ 0.70228425, 2.0455738 , 0.67267578, ..., 0.41406869,**

**-1.10454895, -0.31840916],**

**[ 1.83834103, 2.33645719, 1.98252415, ..., 2.28998549,**

**1.91908301, 2.21963528],**

**[-1.80840125, 1.22179204, -1.81438851, ..., -1.74506282,**

**-0.04813821, -0.75120669]])**

**PCA Model:**

from sklearn.decomposition import PCA
 pca = PCA(n\_components=2)
 pca.fit(scaled\_data)

**Output:**

**PCA(n\_components=2)**

scaled\_data.shape

**Output:**

**(569, 30)**

_# Transform to first 2 principal components_
 x\_pca = pca.transform(scaled\_data)
 x\_pca.shape

**Output:**

**(569, 2)**

**Visualization:**

plt.figure(figsize=(8,6))
 plt.scatter(x\_pca[:,0],x\_pca[:,1],c=cancer[&#39;target&#39;],cmap=&#39;plasma&#39;)
 plt.xlabel(&#39;First principal component&#39;)
 plt.ylabel(&#39;Second Principal Component&#39;)

**Output:**

![](RackMultipart20210731-4-1qy8gmm_html_ed5435a21464994f.png)

**CONCLUSION** :

Hence, reduction of variables has been done and the data has been analyzed and interpreted using Principal Component Analysis (PCA).

126
