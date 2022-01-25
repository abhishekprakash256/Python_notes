## Python OOPs

- A class represents a template that is used again and again.

- if nothing is in the class just type "pass" in that

- A class has a constructor that is fixed syntax

  - ```python
    def __init__(self,arg_1,arg_2,arg_2...arg_n):
    ```

- syntax  (use two spaces in the lines where indentation is needed)

  - ```python
    class name_of_the_class:
     def __init__(self,arg_1,arg_2....arg_n):
      self.arg_1 = arg_1
      self.arg_2 = arg_2
      ..................
       self.arg_n = arg_n
    
    object = name_of_the_class(arg_1,arg_2,arg_2)        
    ```

- we can make a class variable in the class that will apply to all the objects in it.

- inside a class the functions must have a "self" passed in it.

- To view all the variable of the object use "object_name.__dict__"

- To view for the class use "class_name__dict__"

- A class method can be made directly in the class for the update process. 

  - ```python
    @classmethod
    def name_of_the_method(cls, arg_1,arg_2....arg_n):
    	cls.variable = arg_1
    ```

    

