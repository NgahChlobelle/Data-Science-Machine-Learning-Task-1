# WEEK 1 ASSESSMENT

## OBJECTIVES
- To master the fundamental synthax for defining and manipulating Python's primary data structures **(Lists,Tuples and Dictionaries)** 
- To implement core python data structures in order to understand their mutability, indexing and built-in methods for data manipulation.

## TOOLS USED
- Language: **Python**
- Environment: **Jupyter Notebook**

## STEP-BY-STEP PROCESS

## COMMANDS EXECUTED

- Creating a list
1. List Operations (Mutable Sequences)

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

- **2. Tuple Operations (Immutable Sequences)**
- Defining a tuple
ngah = ('a', 'b', 'c', 'd', 'e')

- Accessing the 5th item via index 4
print(ngah[4])

- Counting occurrences of 'a'
ngah.count('a')

- Finding the index of 'c'
ngah.index('c')

- **3. Dictionary Operations (Key-Value Mapping)**
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

- Safe retrieval of values
my_dict.get('names')

- Extracting all key-value pairs, keys, and values separately
my_dict.items()
my_dict.keys()
my_dict.values()

- Adding a new category 'gender' using .update()
my_dict.update({'gender': ['female', 'female', 'male']})

## SCREENSHOTS OF RESULTS

## KEY OBSERVATIONS/LESSONS LEARNED
- Mutability: Lists and Dictionaries can be changed in place, while Tuples cannot. Attempting to change a Tuple results in a TypeError.

- The .sort() Constraint: When a list contains mixed data types (e.g., int and str), the .sort() method fails because Python cannot compare strings to numbers.

- Data Representation: Mapping a key to a list of values is the manual way to create a "Column" in a data table


## PROPER FORMATTING USING MARKDOWN

## CLEAN STRUCTURE AND PROFESSIONAL PRESENTATION
