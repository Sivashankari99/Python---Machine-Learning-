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
