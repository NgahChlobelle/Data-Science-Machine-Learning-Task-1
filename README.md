# WEEK 1 ASSESSMENT

## OBJECTIVES
- To master the fundamental synthax for defining and manipulating Python's primary data structures **(Lists,Tuples and Dictionaries)** 
- To implement core python data structures in order to understand their mutability, indexing and built-in methods for data manipulation.

## TOOLS USED
- Language: **Python**
- Environment: **Jupyter Notebook**

## STEP-BY-STEP PROCESS

### Phase 1: List Construction and Dynamic Modification
In this phase, we created a mutable sequence and tested various methods to alter its structure and content.

##### 1. Initialize the List: Start with a basic list of characters.
letters = ['a', 'b', 'c', 'd', 'e']

##### 2. Append Data: Add a single element to the very end.
letters.append('f')

##### 3. Extend Data: Add multiple elements (g and h) to the end of the existing list.
letters.extend(['g', 'h'])

##### 4. Insert at Index: Place a new element at a specific position (index 0).
letters.insert(0, 1)

##### 5. Remove and Re-insert: Remove an element by value and place it back at a new index.
letters.remove('a')
letters.insert(1, 'a')

##### 6. Extract with Pop: Remove an item at index 3 and store it in a variable to demonstrate the .pop() return value.
pop_elements = letters.pop(3)

##### 7. Search and Count: Locate the index of 'e' and count the frequency of 'b'.
letters.index('e')
letters.count('b')

##### 8. Reorder: Attempt to sort the list (noting that mixed types like integers and strings will cause an error) and then reverse the order.
letters.sort()   # Note: This triggers a TypeError if '1' is still in the list
letters.reverse()

### Phase 2: Working with Immutable Tuples
We explored tuples to understand how to store data that should remain constant throughout a program.

##### 1. Create Tuple: Defined a fixed sequence.
ngah = ('a', 'b', 'c', 'd', 'e')

##### 2. Access and Locate: Retrieve data using indices and search for specific values.
print(ngah[4])
ngah.count('a')
ngah.index('c')

### Phase 3: Dictionary Mapping and Data Extraction

This phase focused on creating key-value pairs using various Python constructors, essential for handling structured data.
##### 1. Multiple Creation Methods: We practiced three ways to define a dictionary to understand syntax flexibility.

- Method 1: Using keyword arguments
  my_dict = dict(name='belle', age=95, city='bamenda')

- Method 2: Using a list of tuples
  my_dict = dict([('name', 'belle'), ('age', 95), ('city', 'bamenda')])

- Method 3: Using standard curly braces
  my_dict = {'name': 'belle', 'age': 95, 'city': 'bamenda'}

##### 2. Handling Complex Values: We mapped single keys to multiple values (tuples and lists) to simulate a database record.
- Mapping keys to tuples
my_dict = {
    'names': ('belle', 'clan', 'best'),
    'ages': (95, 50, 76),
    'city': ('bamenda', 'douala', 'maryland')
}

- Mapping keys to lists 
my_dict_2 = dict([
    ('names', ['belle', 'ngah', 'awah']),
    ('ages', [95, 50, 76]),
    ('city', ['bamenda', 'douala', 'maryland'])
])

##### 3. Data Retrieval: Using built-in methods to isolate keys, values, or items.
my_dict.get('names')  # Safe retrieval
my_dict.items()       # Returns key-value pairs
my_dict.keys()        # Returns all keys
my_dict.values()       # Returns all values

##### 4. Dictionary Update: Merging new data into the existing dictionary.
my_dict.update({'gender': ['female', 'female', 'male']})

## COMMANDS EXECUTED

- Creating a list
#### **1. List Operations (Mutable Sequences)**
- Initializing a list with string elements
letters = ['a', 'b', 'c', 'd', 'e']

- Adding 'f' to the end of the list
letters.append('f')

- Adding multiple elements ('g', 'h') at once
letters.extend(['g', 'h'])

- Inserting an integer '1' at the very beginning (index 0)
letters.insert(0, 1)

- Removing 'a' by value
letters.remove('a')

- Re-inserting 'a' at index 1
letters.insert(1, 'a')

- Removing and returning the element at index 3
pop_elements = letters.pop(3)

- Finding the index position of element 'e'
letters.index('e')

- Counting the occurrences of 'b'
letters.count('b')

- Sorting the list (will cause error if mixed types like int and str are present)
- letters.sort() 

- Reversing the current order of the list
letters.reverse()

#### **2. Tuple Operations (Immutable Sequences)**
- Defining a tuple
ngah = ('a', 'b', 'c', 'd', 'e')

- Accessing the 5th item via index 4
print(ngah[4])

- Counting occurrences of 'a'
ngah.count('a')

- Finding the index of 'c'
ngah.index('c')

#### **3. Dictionary Operations (Key-Value Mapping)**
- Method 1: Creation using keyword arguments
my_dict = dict(name='belle', age=95, city='bamenda')

- Method 2: Creation from a list of tuples
my_dict = dict([('name', 'belle'), ('age', 95), ('city', 'bamenda')])

- Method 3: Standard curly brace literal
my_dict = {'name': 'belle', 'age': 95, 'city': 'bamenda'}

- Advanced Structure: Dictionary with Tuples/Lists as values
my_dict = {
    'names': ('belle', 'clan', 'best'),
    'ages': (95, 50, 76),
    'city': ('bamenda', 'douala', 'maryland')
}

- Retrieval of values
my_dict.get('names')

- Extracting all key-value pairs, keys, and values separately
my_dict.items()

my_dict.keys()

my_dict.values()

- Adding a new category 'gender' using .update()
my_dict.update({'gender': ['female', 'female', 'male']})

## SCREENSHOTS OF RESULTS
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/82bbfcfb0cbdde2ce216691bde238a3c195b34e2/Data%20Structures-Data%20Science%20and%20ML%20Image%201.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/2bc5ecb724c37bacfdeac45cbc8dbb7fba6bac4a/Data%20Structures-Data%20Science%20and%20ML%20Image%202.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/44d7ced2940b550eee858e30ace37ceaa7288ac8/Data%20Structures-Data%20Science%20and%20ML%20Image%203.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/9006e67ea0a8d013e7dad1b17a9ce459232fda10/Data%20Structures-Data%20Science%20and%20ML%20Image%204.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/aaa929b33b7d04011f402afcdfac0bff3496dcbe/Data%20Structures-Data%20Science%20and%20ML%20Image%205.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/0ca2d56b9b3042f1116b3c182e925796b4c4b93a/Data%20Structures-Data%20Science%20and%20ML%20Image%206.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/75181b58582f851c5e7627e09efd60b116eaa15e/Data%20Structures-Data%20Science%20and%20ML%20Image%207.PNG)
![image alt](https://github.com/NgahChlobelle/Data-Science-Machine-Learning/blob/9c03d421b9d72adf9a23b8a77211e6a0a38379e1/Data%20Structures-Data%20Science%20and%20ML%20Image%208.PNG)
## KEY OBSERVATIONS/LESSONS LEARNED
- Lists are Dynamic: Observed that lists can be modified (mutable) using .append(), .pop(), and .insert(). This makes them ideal for datasets that grow over time.

- Tuples are Fixed: Verified that tuples are immutable. Once created, they cannot be changed, which is useful for protecting data from accidental modification.

- Attempting to execute letters.sort() resulted in a TypeError.
This occurred because the list contained a mix of integers (1) and strings ('a', 'b'). Python’s sorting algorithm requires consistent data types to perform comparison logic.

- Dictionaries are highly flexible. I successfully mapped single keys to multiple values using both tuples (for fixed records) and lists (for records that might need updating).



