## Java script

### Main 

- End of line is with semicolon

- Comments 

```javascript
//in-line comment 
/*-------
multi line comment
-------*/
```

- Data types 

  ```
  undefined , null , boolean ,string , symbol, number and object
  ```

- Variable declaration 
  - 3 ways 
    - var (use anywhere)
    - let (with in scope of function)
    - const (should not change)
  - Assignment and declaration can be done in two line 

- Printing 
  ```javascript
  console,log()
  ```

- String 

  - string is same like python deceleration and addition 

  - find the length 

    ```javascript
    var firstname = "Abhishek"
    length_of_str = firstname.length;
    ```

  - access the element by using the indexing same as python

  - indexing starts at 0 

  - string are immutable

  - getting the last character of the string 

    ```javascript
    var firstname = "Abhishek";
    var last_char = firstname[firstname.length - 1];
    ```

- Array 

  - array can take mixed data types 

    ```javascript
    var my_array = [1,2,"abhi","text"]
    ```

  - nested array same as python

  - accessing the elements - same as python like indexing method

  - mutable data-type

  - .push to add to last of the array like append()

  - .pop() to remove the last element 

  - .shift() to remove the first element of the array 

  - .unshift() to add the element at the begging of the array 

  - spread operator 

    ```js
    arr_1 = [...args]  //for the array elements assignment
    ```

    

- functions 

  - mostly same as python

  ```javascript
  function function_name(arg, args)
  {
      //body ;
  }
  
  function_name(arg, args);
  ```

  - Arrow functions 

    ```js
    var myConcat = (a1,a2) => a1.concat(a2);
    console.log(myConcat([1,2],[1,2,3]))
    ```

  - Rest operators used to take any number of operators

    ```js
    function myfunction(,,,args){
        //do something
    }
    ```

  - 

- Scope of variable

  - Outside the function can be accessed at all level 
  -  no var makes a variable available at all level 

- Boolean value are same as python

- If conditions 

  - syntax 

    ```javascript
    if (condition)
        {
            //do something 
        }
    else {
        //do something
    }
    ```

  - equality operator is same as python like == to check the value

  - === strict check the type and the data as well

  - 3 =='3' true

  - 3=== '7' False

  - !=  not equal to 

  - !== not equal to types 

  - && operator

  - || or operator

  - else if same as elif 

    ```javascript
    if (condtion) {
        
    }
    
    else if ()
    {     
             }
    else
        {
            
        }
    ```

  - switch statement 

    - syntax

      ```javascript
      switch(val){
          case "a": 
          answer = "something"
          break;
          case  "b":
          answer = "somthing2"
                  }
      ```

- Objects are like dictionary but important data structure

  - arrays can have objects inside as well, and nested structure
  - "." are used to access the nested structure that are there

  ```javascript
  var my_dict = {
  "name": "abhi",
  "work": "student",
  }
  ```

  - access the element by . property 

- Loops 

  - While loops 

    ```javascript
    while (condn)
    {
        //do something
    }
    ```

  - For loop 

    ```javascript
    for(var i = 0; i< 5; i++)
        {
            //do something 
        }
    ```

    - iteration can be done with stepping like 2 as well

  - Do while 

    ```javascript
    do {
    //do something
    }
    
    while (condn)
    
    ```

- Generate the Random numbers
  ```javascript
  Math.random()
  ```

  

- Build in function 

  - will change the str to int type

  ```js
  parseInt(str):
  ```

- Ternary operator can make the syntax more faster, used in place for return statement

  ```js
  ? "this will be out"
  ```

- Var and let 

  - Var can let to declare more times , declared globally 
  - Let can let you declare once , has smaller scope 

  ```js
  var my_1 = 6
  let my = 6
  ```

  - const let you define only one and can't be changed later

- the function and variable are case sensitive in name 

- Incrementing and decrementing 

  ```
  var--;
  var++;
  ```

- compound assignment  (same a = a+6)

  ```javascript
  a*=6
  a+=6
  a-=7
  ```

- Escape character

  - the backslash will not render

  ```javascript
  var myvar = "string "\"this is sample"
  ```

- Some escape character 

  ```javascript
  \'
  \"
  \\
  \n newline
  \r carriage return
  \t tab 
  \b  backstage
  \f form feed
  ```

  

