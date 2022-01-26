## Tips for python



### Python tools -

-  pylint for code rating 
- pytest for testing of code 
- py-coverage for test coverage
- black formatter for formatting the code



Print in the same line

```python
list1 = [10,11,12,13,14,15]  
for i in list1:
    print(i, end = " ")  
```

For appending the values in dictionary with hash function

```python
for i in range(0,len(arr)):
		my_dict.update({arr[i]: hash(arr[i])})    #hash function are used for hashing 
```

Time module in Python

```python
import time
time.time()
```

For the reversal 

```python
for in reversed(range(0,n)):
    print(i)
    
return list_name[::-1]    #for list reversal
    
```

From list to string conversion

```python
str1= ""
return (str1.join(lst))
```

Remove the white space from the string 

```python
string.replace(" ","")  #save the result in a varibale as well.
```

The comparison error in python > and < with the given argument passed in the function

```python
def function_name(arr,sum):
    sum = x #this will work for comparision. just assign a variable
```

Dictionaries (they have lookup time is O(1) worst time is O(n) ) https://wiki.python.org/moin/DictionaryKeys

```python
new_dict = {
"element_1" : 1,
"element_2" : 2,
"element_3" : 3,
"element_4" : 4
}
print(new_dict)                #print
print(new_dict["element_1"])    #element print
print(len(new_dict))             #len of dict
new_dict.update({"element_2": 5})      #updation of the element
new_dict ["elemenet_6"] = 6            #adding the new element
new_dict.update({"elemenet_7": 7}) 
print(new_dict.values())           #getting the values 
print(new_dict.items())            #getting the items
print(new_dict.popitem())          #removing the values
print(new_dict.get("element_1"))           #getting the values
for x in new_dict: #all elements print
	print(x)
for x in new_dict.values():
	print(x)
for x in new_dict.keys():
	print(x)
```

### Enumerate 

- sometimes enumerate is a better alternative than the range as it gives both index and the value 

```python
lst = [1,2,3,54,65,7,8,9]
for i in enumerate(lst):
	print(i)
```



### List compression 

- ```python
  squares  = [i*i for i in range(10)]  #Add the  values to the list
  ```

### Sorting 

```python
lst = sorted(lst,reverse = True)
```

### Sets 

```python
lst = [1,23,1,2,3,4,5,4,4,4]
my_set = set(lst) #remove all the duplicate values
```

### Generators function 

- lazy functions that can generate one value at a time, also it saves a lot of memory
- the syntax uses the parenthesis 
- good for large dataset

```python
my_gen = (i for i in range(10))
sum(my_gen)
```

### Dictionary zero key error 

- get he zero key error if the key is not defined then use the get method for the default value

```python
my_dict = {"first": 1 , "second" : 2 , "third" : 3 , "fourth" : 4}
print(my_dict.get("zero"))
```

### Counting the number of the values in the list 

- use the collections method to count the number of times a object has occurred in the list 
- .most_common() is used to get the most common element in the list 

```python
from collections import Counter
lst_2 = [2,2,4,5,6,7,8,9]
print(Counter(lst_2))
```

### String 

- Formatting is much better to use than the usual printing of the stings

- .join() method is much faster than other methods

  ```python
  str_lst = ["this", "is" , "test"]
  new = ""
  print(new.join(str_lst))
  ```

### Merge the dictionary 

- to merge the two dictionary use this syntax 

```python
dict_0 = {"first": 1 , "second" : 2 , "third" : 3 , "fourth" : 4}
dict_1 = {"five":5, "six":6, "seven":7, "eight":8}

print({**dict_0, **dict_1})
```

### Simplify the list statement 

- use in instead of == to compare

### Tuple vs list

- List are mutable and tuples are not
- Both can be unpacking done with multiple elements
- Less function for the tuple more for the list
- Tuple once created can't be changed but list can be changed
- tuple starts with (), []
- List can be copied and tuple can't be copied

### __init__.py file 

- the init file has all the imports to help for the importing 
- it simplify the process of the import 
- Use to make a directory into library 

### Project structue 

- make a main folder with project name 

- initialize the git init in main folder

- Add the README fille ASAP

- make .gitignore file

- make two folders test and src (source)

- src can have multiple folders that hold different files

- MVC file structure for the backend development (model, view, controller)

- Can use Github Project board for project progress

  

  ### Small project structure 

  - The file structure - 
    - run (main) , helpers , constant
    - run (has the minimal files as main files)
    - helpers has all the main functions
    - constant (has all the constant values)

  

  ### Complex project structue 

  - The file stucture - 
    - Directory name as per function 
    - the directory should have the (dunder_init_dunder.py) file
    - run file as the parent file in above the directory
    - Sample structure 
      - run.py or main.py
      - folder_1 
        - helper.py
        - function.py
        - constant.py
        - __init__.py  (has double dunder)
      - folder_2
        - helpers_1.py
        - functiion_2.py
        - __init__.py (has double dunder)
  - init file has all the imports to help 

  ### Package structure examples - 

  ```bash
  packaging_tutorial/
  ├── LICENSE
  ├── pyproject.toml
  ├── README.md
  ├── setup.cfg
  ├── src/
  │   └── example_package/
  │       ├── __init__.py
  │       └── example.py
  └── tests/
  ```

  ```
  helloworld/
  │
  ├── .gitignore
  ├── helloworld.py
  ├── LICENSE
  ├── README.md
  ├── requirements.txt
  ├── setup.py
  └── tests.py
  ```

  ```
  helloworld/
  │
  ├── helloworld/
  │   ├── __init__.py
  │   ├── helloworld.py
  │   └── helpers.py
  │
  ├── tests/
  │   ├── helloworld_tests.py
  │   └── helpers_tests.py
  │
  ├── .gitignore
  ├── LICENSE
  ├── README.md
  ├── requirements.txt
  └── setup.py
  ```

  ```
  helloworld/
  │
  ├── bin/
  │
  ├── docs/
  │   ├── hello.md
  │   └── world.md
  │
  ├── helloworld/
  │   ├── __init__.py
  │   ├── runner.py
  │   ├── hello/
  │   │   ├── __init__.py
  │   │   ├── hello.py
  │   │   └── helpers.py
  │   │
  │   └── world/
  │       ├── __init__.py
  │       ├── helpers.py
  │       └── world.py
  │
  ├── data/
  │   ├── input.csv
  │   └── output.xlsx
  │
  ├── tests/
  │   ├── hello
  │   │   ├── helpers_tests.py
  │   │   └── hello_tests.py
  │   │
  │   └── world/
  │       ├── helpers_tests.py
  │       └── world_tests.py
  │
  ├── .gitignore
  ├── LICENSE
  └── README.m
  ```

  ```
  sound/                          Top-level package
        __init__.py               Initialize the sound package
        formats/                  Subpackage for file format conversions
                __init__.py
                wavread.py
                wavwrite.py
                aiffread.py
                aiffwrite.py
                auread.py
                auwrite.py
                ...
        effects/                  Subpackage for sound effects
                __init__.py
                echo.py
                surround.py
                reverse.py
                ...
        filters/                  Subpackage for filters
                __init__.py
                equalizer.py
                vocoder.py
                karaoke.py
                ...
  ```

### Make the requirements.txt file 

- Two ways to do

  - In virtual environment use 

    ```
    pip freeze > requirements.txt
    ```

  - For directory of the project using pipreqs

    - come one directory up 

    - use command 

      ```
      pipreqs dir_name/
      ```

  - Poetry dependencies are also possible 

### Links - 

```
https://www.programiz.com/python-programming/docstrings  (how to put docstring)
```

