## Python Questions 

### Common Interview questions 

- **What is pickling and unpickling?**

  - Pickle module accepts any Python object and converts it into a string  representation and dumps it into a file by using dump function. This  process is called pickling. While the process of retrieving original  Python objects from the stored string representation is called  unpickling.

- **How is Python interpreted?**

  - Python language is an interpreted language. Python program runs directly from the source code. It converts the source code that is written by  the programmer into an intermediate language, which is again translated  into machine language that has to be executed.

- **How is memory managed in Python?**

  - Python memory is managed by Python private heap space. All Python  objects and data structures are located in a private heap. The  programmer does not have an access to this private heap, and the  interpreter takes care of this Python private heap.
  - Python also has an inbuilt garbage collector, which recycles all the  unused memory and frees the memory and makes it available to the heap  space.

-  **What is the difference between list and tuple?**

  - The difference between list and tuple is that list is mutable while  tuple is not. Tuple can be hashed, for example., as a key for  dictionaries.

- **How are arguments passed by value or by reference?**

  - Everything in Python is an object, and all variables hold references to  the objects. The reference values are according to the functions.   Therefore, you cannot change the value of the references. However, you  can change the objects if it is mutable.

- **What are built-in type does python provides?**

  - Mutable built-in types are:
    - List
    - Sets
    - Dictionaries
    - Immutable built-in types
    - Strings
    - Tuples
    - Numbers
  - Immutable built-in types are:
    - Strings
    - Tuples
    - Numbers

- **Explain namespace in Python**

  - In Python, every name introduced has a place where it lives and can be  hooked for. This is known as a namespace. It is like a box where a  variable name is mapped to the object placed. Whenever the variable is  searched out, this box will be searched to get the corresponding object.

- **What is lambda in Python?**

  - It is a single expression anonymous function often used as inline function.

- **Why lambda forms in python do not have statements?**

  - A lambda form in python does not have statements as it is used to make new function object and then return them at runtime.

- **Explain pass in Python**

  - Pass means no-operation Python statement, or in other words, it is a  place holder in a compound statement, where there should be a blank  left, and nothing has to be written there.

- **What are generators in Python?**

  - The way of implementing iterators are known as generators. It is a  normal function except that it yields expression in the function.

- **What is docstring in Python?**

  - To copy an object in Python, you can try a copy.copy () or  copy.deepcopy() for the general case. You cannot copy all objects but  most of them.

- **How can you share global variables across modules?**

  - To share global variables across modules within a single program, create a special module. Import the config module in all modules of your  application. The module will be available as a global variable across  modules.

- **Explain how can you make a Python Script executable on Unix?**

  - To make a Python Script executable on Unix, you need to do two things,

    Script file’s mode must be executable, and the first line must begin with # ( #!/usr/local/bin/python)

- **What is Tuple Matching in Python?**

  - Tuple Matching in Python is a method of grouping the tuples by matching  the second element in the tuples. It is achieved by using a dictionary  by checking the second element in each tuple in python programming.  However, we can make new tuples by taking portions of existing tuples.

-  **What are all dictionary methods:**

  - copy()
  - update()
  - items()
  - sort()
  - len()
  - cmp()
  - Str()

- **Explain membership operators with example**

  - These operators test for membership in a sequence such as lists,  strings, or tuples. Two membership operators are used in Python. (in,  not in). It gives the result based on the variable present in a  specified sequence or string.

-  **Explain Inheritance with example**

  - Inheritance is a feature used in object-oriented programming; it refers  to defining a new class with less or no modification to an existing  class. The new class is called the derived class, and from one which it  inherits is called the base. Python supports inheritance; it also  supports multiple inheritances. A class can inherit attributes and  behavior methods from another class called subclass or heir class.

- **78) What are the common examples of exceptions in Python?**

  - The common examples of exceptions in Python are:
    - Division by Zero
    - Accessing a file that does not exist.
    - Addition of two incompatible types
    - Trying to access a nonexistent index of a sequence
    - Removing the table from the disconnected database server.
    - ATM withdrawal of more than the available amount

- **Explain important Python errors**

  - **ArithmeticError:** ArithmeticError act as a base class for all arithmetic exceptions. It is raised for errors in arithmetic operations.
  - **ImportError:** ImportError is raised when you are  trying to import a module which does not present. This kind of exception occurs if you have made a typing mistake in the module name or the  module which is not present in the standard path.
  - **IndexError:** An IndexError is raised when you try to refer a sequence which is out of range.

-  **How can you print without a newline in Python?**

  - From Python 3+, there is an additional parameter introduced for print()  called end=" ". This parameter takes care of removing the newline that is  added by default in print().

- ### What is Scope in Python?

  - Every object in Python functions within a scope. A scope is a block of  code where an object in Python remains relevant. Namespaces uniquely  identify all the objects inside a program. However, these namespaces  also have a scope defined for them where you could use their objects  without any prefix. A few examples of scope created during code  execution in Python are as follows:
  - A **local scope** refers to the local objects available in the current function.
  - A **global scope** refers to the objects available throughout the code execution since their inception.
  - A **module-level scope** refers to the global objects of the current module accessible in the program.
  - An **outermost scope** refers to all the built-in names callable in the program. The objects in this scope are searched last to find the name referenced.

  **Note:** Local scope objects can be synced with global scope objects using keywords such as **global**.

- ### What are global, protected and private attributes in Python?

  - **Global** variables are public variables that are defined  in the global scope. To use the variable in the global scope inside a  function, we use the `global` keyword.
  - **Protected** attributes are attributes defined with an  underscore prefixed to their identifier eg. _sara. They can still be  accessed and modified from outside the class they are defined in but a  responsible developer should refrain from doing so.
  - **Private** attributes are attributes with double  underscore prefixed to their identifier eg. __ansh. They cannot be  accessed or modified from the outside directly and will result in an  AttributeError if such an attempt is made.

- ###  What is the use of self in Python?

  - **Self** is used to represent the instance  of the class. With this keyword, you can access the attributes and  methods of the class in python. It binds the attributes with the given  arguments. self is used in different places and often thought to be a  keyword. But unlike in C++, self is not a keyword in Python.

- ### What is __init__?

  - It is a contructor method in Python and is automatically called to allocate memory when a new object/instance is created. All classes have a **__init__** method associated with them. It helps in distinguishing methods and attributes of a class from local variables.

- ### What is docstring in Python?

  - Documentation string or docstring is a multiline string used to document a specific code segment.
  - The docstring should describe what the function or method does.

- ### What are decorators in Python?

  - **Decorators** in Python are essentially functions that add functionality to an existing function in Python without changing the  structure of the function itself. They are represented the `@decorator_name` in Python and are called in a bottom-up fashion. For example:

- ###  What is the difference between xrange and range in Python?

  - **xrange()** and **range()** are quite similar in terms of functionality. They both generate a sequence of integers, with the only difference that `range()` returns a **Python list**, whereas, `xrange()` returns an **xrange object**.
  - it sure does, because unlike range(), xrange() doesn't generate a static  list, it creates the value on the go. This technique is commonly used  with an object-type **generator** and has been termed as "**yielding**".

- ### What are generators in Python?

  - Generators are functions that return an iterable collection of items,  one at a time, in a set manner. Generators, in general, are used to  create iterators with a different approach. They employ the use of `yield` keyword rather than `return` to return a **generator** object.
  - The difference is that while a `return` statement terminates a function entirely, `yield` statement pauses the function saving all its states and later continues from there on successive calls.

- ### What is the difference between .py and .pyc files?

  - py files contain the source code of a program. Whereas, .pyc file  contains the bytecode of your program. We get bytecode after compilation of .py file (source code). .pyc files are not created for all the files that you run. It is only created for the files that you import.
  - Having .pyc file saves you the compilation time.

- ### How Python is interpreted?

  - Python as a language is not interpreted or compiled. Interpreted or  compiled is the property of the implementation. Python is a bytecode(set of interpreter readable instructions) interpreted generally.
  - Python compiles the source code to a set of instructions for a virtual  machine. The Python interpreter is an implementation of that virtual  machine. This intermediate format is called “bytecode”.
  - .py source code is first compiled to give .pyc which is bytecode. This  bytecode can be then interpreted by the official CPython or JIT(Just in  Time compiler) compiled by PyPy.

- ### What does *args and **kwargs mean?

  - *args is a special syntax used in the function definition to pass variable-length arguments.
  - “*” means variable length and “args” is the name used by convention. You can use any other.

- ### How do you access parent members in the child class?

  - **By using super():** The parent class members can be accessed in child class using the super keyword.

- ### Why is finalize used?

  - Finalize method is used for freeing up the unmanaged  resources and clean up before the garbage collection method is invoked.  This helps in performing memory management tasks.

- **What are Literals in Python and explain about different Literals**

  - A literal in python source code represents a fixed value for primitive data types. There are 5 types of literals in python-
    1. **String literals**– A string literal is created by assigning some text enclosed in single  or double quotes to a variable. To create multiline literals, assign the multiline text enclosed in triple quotes. Eg.`name=”Tanya”`
    2. **A character literal**– It is created by assigning a single character enclosed in double quotes. Eg. `a=’t’`
    3. **Numeric literals**– They include numeric values that can be either integer, floating point value, or a complex number. Eg. `a=50`
    4. **Boolean literals**– These can be 2 values- either True or False.

- **How to combine dataframes in pandas?**

  - The dataframes in python can be combined in the following ways-
    1. Concatenating them by stacking the 2 dataframes vertically.
    2. Concatenating them by stacking the 2 dataframes horizontally.
    3. Combining them on a common column. This is referred to as joining.

- ### **What is the difference between deep and shallow copy?**

  - *Shallow copy* is used when a new instance type gets created and it keeps the values that are  copied in the new instance. Shallow copy is used to copy the reference  pointers just like it copies the values. These references point to the  original objects and the changes made in any member of the class will  also affect the original copy of it. Shallow copy allows faster  execution of the program and it depends on the size of the data that is  used.

    *Deep copy* is used to store the values that are already copied. Deep copy doesn’t  copy the reference pointers to the objects. It makes the reference to an object and the new object that is pointed by some other object gets  stored. The changes made in the original copy won’t affect any other  copy that uses the object. Deep copy makes execution of the program  slower due to making certain copies for each object that is been called.

- ### **How do you do data abstraction in Python?**

  - Data Abstraction is providing only the required details and hiding the implementation from the world. It can be achieved in Python by using interfaces and abstract classes.

  





### Links - 

```
https://www.guru99.com/python-interview-questions-answers.html
https://www.tutorialspoint.com/python/python_interview_questions.htm

```

