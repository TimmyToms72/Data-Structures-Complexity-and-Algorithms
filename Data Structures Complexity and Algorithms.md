# Data Structures Complexity and Algorithms

Data Structures is how to represent data better

Matrix 
- a matrix is a 2d representation of numbers in an array
- This is a nessenary for math like calculus and vectors
- all rows have same number of values 
- all columns have the same number of values
- has to be the same data type
- slicing and indexing start at 0

```python
matrixA = [
  [1,2,3,4],
  [5,6,7,8]
]
print( % matrixA[0])
print( % matrixA[0][0])
```

List Comprehension
- it is a concise way to make lists
- The list is member of another iterable data that satisfies a certain condition

```python
squares = [i**2 for i in range(10)]

print('Our new result: %s' % squares)
```

Map function
- the point is to apply a fuction for iterable data
map(fuctionName, sequence)

```python
def square(num):
    ''' squares the given num argument '''
    return num ** 2

array = list(range(1,11))
square_array = list(map(square, array))

print(array)
print(square_array)
```

Filter
- The idea of the filter function is to filter out items from a data set that meets a certain condition
filter(boolReturnFunction, sequence)
- the function must return a boolean value
- a sequence is a iterable data type

Tuples
- A tuple is a different data type than list and string
- () this is empty tuple
- (82,) the comma at the end of a single tuple is requierd
- all tuples are slicable and indexable

```python
example = ('C', 'Java', 'Python', 'C#', 'JavaScript')

print('Tuple example items:')
for language in example:
    print(language)

print(example[1])
print(example[-1])
print(example[::-1])
print(example[::2])
print(example[1:])
print(example[1:3])
```
there are lots of different ways to use tuples
- packing/unpacking
- Tuple Comprehension
- Tuples are Iterable, Indexable, and Sliceable

Sets
- a set is an unordered collection
- a mathimatical way to show collection of items

```python
example_set1 = {1, 2, 3}
example_set2 = {'h','e','l','l','o'}

print('example_set1:', example_set1)
print('example_set2:', example_set2)
print('--')

singleton_set = {7}
empty_set = set()
print('Singleton:', singleton_set)
print('Empty Set:', empty_set)
```

set operators
- Union
- Intersection
- Difference
- Symmetric Difference
- Proper Subset
- Subset
- Proper Superset
- Superset

Disjoint: A Set Behaviour Property
- Two set are consided disjointed when two sets share no common value.
- Let A and B both represent a set.
- If A & B is empty, then set A and B are considered disjointed.
- To check this in python there is a method called: isdisjoint()

Dictonary

Operations
- Adding a pair
- Removing a pair
- Modify an existing pair
- Lookup of a value associated with a particular key
```python
sammy = {
    'username': 'sammy',
    'online': True,
    'followers': 42
}

print('Sammy dict:', sammy)
print('Username:', sammy['username'])
print('Online Status:', sammy['online'])
print('Follower Count:', sammy['followers'])
```
dictonary propertys

keys

- a unique location vale for dictonary
- must be mutable
- cant have 2 of the same keys
- if key duplicated the newest key with overtake the old one

values
- a dictionary within a key can be any data type

Deletion
- delete a key hence deleting the value connected to the key
- empty out the entire dictionary
- delete the dictionary rarely used

Membership
- We can use the in and not in operators to check if a key exists in a dictionary

Dictionary Methods
- A.keys()
- A.values()
- A.items()
- A.get(address)
- A.update(B)
