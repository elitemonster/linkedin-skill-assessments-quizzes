Python Assessment
-------------------

#### Q1. What is an abstract class?
- An abstract class is the name for any class from which you can instantiate an object.
- Abstract classes must be redefined any time an object is instantiated from them 
- Abstract classes must inherit from concrete classes.
- An abstract class exists only so that other "concrete" classes can inherit from the abstract class. //CORRECT

#### Q2. What happens when you use the build-in function "any()" on a list?
- The "any()" function will randomly return any item from the list.
- The "any()" function returns True if any item in the list evaluates to True. Otherwise, it returns Fals. // CORRECT
- The "any()" function takes as arguments the list to check inside, and the item to check for. If "any" of the items in the list match the item to check for, the function returns True.
- The "any()" function returns a Boolean value that answers the question "Are there any items in this list?"

#### Q3. What data structure does a binary tree degenerate to if it isn't balanced properly?
- linked list //CORRECT
- queue
- set 
- OrderedDict

#### Q4. What is a static method?
- Static methods are called static because they always return "None".
- Static methods can be bound to either a class or an instance of a class.
- They serve mostly as utility methods or helper methods, since they can't access or modify a class's state. //CORRECT
- Static methods can access and modify the state of a class or an instance of a class. 

#### Q5. What are attributes?
- Attributes are long-form version of an "if/else" statement, used when testing for equality between objects.
- Attributes are a way to hold data or describe a state for a class or an instance of a class.
- Attributes are strings that describe characteristics of a class.
- Function arguments are called "attributes" in the context of class methods and instance methods. //CORRECT

#### Q6. What is the term to describe this code?
```javascript
count, fruit, price = (2, 'apple', 3.5)
```
- tuple assignment //CORRECT
- tuple unpacking
- tuple matching
- tuple duplication

#### Q7. What built-in list method would you use to remove items from a list?
- `".delete()" method`
- `pop(my_list)`
- `del(my_list)`
- `".pop()" method`  //CORRECT

#### Q8. What is one of the most common use of Python's sys library?
- to capture command-line arguments given at a file's runtime  //CORRECT
- to connect varios systems, such as connecting a web front end, an API service, a database, and a mobile app
- to take a snapshot of all the packages and libraries in your virtual environment
- to scan the health of your Python ecosystem while inside a virtual environment

#### Q9. What is the runtime of accessing a value in a dictionary by using its key?
- "O(n)", also called linear time
- "O(log n)", also called logarithmic time
- "O(n^2)", also called quadratic time
- "O(1)", also called constant time  //CORRECT

#### Q10. What is the correct syntax for defining a class called Game?
- `class Game: pass` //CORRECT
- `def Game(): pass`
- `def Game: pass`
- `class Game(): pass`

#### Q11. What is the correct way to write a doctest?
- 
```
def sum(a, b):
    """
    sum(4, 3)
    7   
    
    sum(-4, 5)
    1
    """
    return a + b
```
- 
```
def sum(a, b):   //CORRECT
    """
    >>> sum(4, 3)
    7   
    
    >>> sum(-4, 5)
    1
    """
    return a + b
```
- 
```
def sum(a, b):
    """
    # >>> sum(4, 3)
    # 7   
    
    # >>> sum(-4, 5)
    # 1
    """
    return a + b
```
- 
```
def sum(a, b):
    ###
    >>> sum(4, 3)
    7   
    
    >>> sum(-4, 5)
    1
    ###
    return a + b
```


#### Q12. What buit-in Python data type is commonly used to represent a stack?
- set
- list //CORRECT
- None. You can only build a stack from scratch.
- dictionary

#### Q13. What would this expression return?
```
college_years = ['Freshman', 'Sophomore', 'Junior', 'Senior']
return list(enumerate(college_years, 2019)
```
- `[('Freshman', 2019), ('Sophomore', 2020), ('Junior', 2021), ('Senior', 2022)]`
- `[(2019, 2020, 2021, 2022), ('Freshman', 'Sophomore', 'Junior', 'Senior')]`
- `[('Freshman', 'Sophomore', 'Junior', 'Senior'), (2019, 2020, 2021, 2022)]`
- `[(2019, 'Freshman'), (2020, 'Sophomore'), (2021, 'Junior'), (2022, 'Senior')]` //CORRECT

#### Q14. How does "defaultdict" work?
- "defaultdict" will automatically create a dictionary for you that has keys which are the integers 0-10
- "defaultdict" forces a dictionary to only accept keys that are of the types specified when you created the "defaultdict" (such as string or integers). //CORRECT
- If you try to access a key in a dictionary that doesn't exist, "defaultdict" will create a new key for you instead of throwing a "KeyError".
- "defaultdict" stores a copy of a dictionary in memory that you can default to if the original gets unintentionally modified.

#### Q15. What is the correct syntax for defining a class called "Game", if it inherits from a parent class called "LogicGame"?
- `class Game.LogicGame(): pass`
- `def Game(LogicGame): pass`
- `class Game(LogicGame): pass` //CORRECT
- `def Game.LogicGame(): pass`

#### Q16. What is the purpose of the "self" keyword when defining or calling instance methods?
- `self means that no other arguments are required to be passed into the method`
- `There is no real purpose for the self method; it"s just historic computer science jargona that Python keeps to stay consistent with other programming languages`
- `self  refers to the instance whose method was called` // CORRECT
- `self refers to the class that was inherited from to create the object using self`

#### Q17. Which of these is NOT a characteristic of namedtuples?
- `You can assign a name to each of the namedtuple members and refer to them that way, similarly to how you would access keys in dictionary` 
- `Each member of a namedtuple object can be indexed to directly, just like in a regular tuple`
- `namedtuples are just as memory efficient as regular tuples`
- `No import is needed to use namedtuples because they are available in the standard library` //CORRECT

#### Q18. What is an instance method?
- `Instance methods can modify the state of an instance or the state of its parent class` //CORRECT
- `Instance methods hold data related to the instance`
- `An instance method is any class method that doesn"t take any arguments`
- `An instance method is a regular function that belongs to a class, but it must return None`

#### Q19. Which choice is the most syntactically correct example of the conditional branching?
```
num_people = 5

if num_people > 10;
    print("There is a lot of people in the pool.")
elif num_people > 4;
    print("There are some people in the pool.")
elif num_people > 0;
    print("There are a few people in the pool.")
else:
    print("There is no one in the pool.")
    -------------

num_people = 5

if num_people > 10;
    print("There is a lot of people in the pool.")
if num_people > 4;
    print("There are some people in the pool.")
if num_people > 0;
    print("There are a few people in the pool.")
else:
    print("There is no one in the pool.")

    -------------
num_people = 5                            //CORRECT

if num_people > 10:
    print("There is a lot of people in the pool.")
elif num_people > 4:
    print("There are some people in the pool.")
elif num_people > 0:
    print("There are a few people in the pool.")
else:
    print("There is no one in the pool.")
    -------------
    
if num_people > 10;
    print("There is a lot of people in the pool.")
if num_people > 4;
    print("There are some people in the pool.")
if num_people > 0;
    print("There are a few people in the pool.")
else:
    print("There is no one in the pool.")
```

#### Q20. Which statement does NOT describe the object-oriented programming concenpt of encapsulation?
- `It protects the data from outside interference `
- `A parent class is encapuslated and no data from the parent class passes on to the child class`
- `It keeps data and the methods that can manipulate that data in one place`
- `It only allows the data to be changed by methods` //CORRECT

#### Q21. What is the purpose of an if/else statement?
- `An if/else statement tells the computer which chunk of code to run if the instructions you coded are incorrect `
- `An if/else statement runs one chunk of code if all the imports were succesful, and another chunk of code if the imports were not succesful `
- `An if/else statement  executes one chunk of code if a condition it true, but a different chunk of code if the condition is false` //CORRECT
- `An if/else statement tells the computer which chunk of code to run if the is enough memory to handle it. and which chunk of code to run if there is not enough memory to handle it`

#### Q22. What buit-in Python data type is commonly used to represent a queue?
- dictionary
- set
- None. You can only build a stack from scratch.
- list //CORRECT

#### Q23. What is the correct syntax for instantiating a new object of the type Game?
- `my_game = class.Game()`
- `my_game = class(Game)`
- `my_game = (Game)` //CORRECT
- `my_game = Game.create()`

#### Q24. What does the built-in map() function do?
- It creates a path from multiple values in an iterable to a single value.
- It applies a function to each item in an iterable and returns the value of that function. //CORRECT
- It converts a complex value type into simpler value types.
- It creates a mapping between two different elements of different iterables.

#### Q25. If you don't explicitly return a value from a function, what happens?
- The function will return a RuntimeError if you don't return a value.
- If the return keyword is absent, the function will return None. //CORRECT
- If the return keyword is absent, the function will return True.
- The function will enter an infinite loop because it won't know when to stop executing its code.

#### Q26. What is the purpose of the pass statement in Python?
- It is used to skip the yield statement of a generator and return a value of None.
- It is a null operation used mainly as a placeholder in functions, classes, etc. //CORRECT
- It is used to pass control from one statement block to another.
- It is used to skip the rest of a while or for loop and return to the start of the loop.

#### Q27. What is the term used to describe items that may be passed into a function?
- arguments // CORRECT
- paradigms
- attributes
- decorators

#### Q28. Which collection type is used to associate values with unique keys?
- slot
- dictionary //CORRECT
- queue
- sorted list

#### Q29. When does a for loop stop iterating?
- when it encounters an infinite loop
- when it encounters an if/else statement that contains a break keyword //CORRECT
- when it has assessed each item in the iterable it is working on or a break keyword is encountered
- when the runtime for the loop exceeds O(n^2)

#### Q30. Assuming the node is in a singly linked list, what is the runtime complexity of searching for a specific node within a singly linked list?
- The runtime is O(n) because in the worst case, the node you are searching for is the last node, and every node in the linked list must be visited. //CORRECT
- The runtime is O(nk), with n representing the number of nodes and k representing the amount of time it takes to access each node in memory.
- The runtime cannot be determined unless you know how many nodes are in the singly linked list.
- The runtime is O(1) because you can index directly to a node in a singly linked list.

#### Q31. Given the following three list, how would you create a new list that matches the desired output printed below?
```
fruits = ['apples', 'oranges', 'bananas']
quantities = [5, 3, 4]
prices = [1.50, 2.25, 0.89]

# Desired output
[('Apples', 5, 1.50),
('Oranges', 3, 2.25),
('Bananas', 4, 0.89)]
```

- 
```
output = []

fruit_tuple_0 = (first[0], quantities[0], price[0])
output.append(fruit_tuple)

fruit_tuple_1 = (first[1], quantities[1], price[1])
output.append(fruit_tuple)

fruit_tuple_2 = (first[2], quantities[2], price[2])
output.append(fruit_tuple)

return output
```
- 
```
i = 0
output = []
for fruit in fruits:
    temp_qty = quantities[i]
    temp_price = prices[i]
    output.append((fruit, temp_qty, temp_price))
    i += 1
return output
```
- 
```
groceries = zip(fruits, quantities, prices) //CORRECT
return groceries

>>> [
('Apples', 5, 1.50),
('Oranges', 3, 2.25),
('Bananas', 4, 0.89)
]
```
-
```
i = 0
output = []
for fruit in fruits:
    for qty in quantities:
        for price in prices:
            output.append((fruit, qty, price))
    i += 1
return output

```
#### Q32. What happens when you use the built-in function all() on a list?
- The all() function returns a Boolean value that answers the question "Are all the items in this list the same?"
- The all() function returns True if all the items in the list can be converted to strings. Otherwise, it returns False.
- The all() function will return all the values in the list.
- The all() function returns True if all items in the list evaluate to True. Otherwise, it returns False. //CORRECT

#### Q33. What is the correct syntax for calling an instance method on a class named Game?
- 
```
>>> dice = Game()
>>> dice.roll()    //CORRECT
```
- 
```
>>> dice = Game(self)
>>> dice.roll(self)
```
- 
```
>>> dice = Game()
>>> dice.roll(self)
```
- 
```
>>> dice = Game(self)
>>> dice.roll()
```
#### Q34. Correct representation of doctest for function in Python
-
```
def sum(a, b):
    # a = 1
    # b = 2
    # sum(a, b) = 3
    
    return a + b
```	
-
```
def sum(a, b):
    """
    a = 1
    b = 2
    sum(a, b) = 3
    """
    
    return a + b
```	
-
```
def sum(a, b):    //CORRECT
    """
    >>> a = 1
    >>> b = 2
    >>> sum(a, b)
    3
    """
    
    return a + b
```
-
```
def sum(a, b):
    '''
    a = 1
    b = 2
    sum(a, b) = 3
    '''
    
    return a + b
```
#### Q35. What is the algorithmic paradigm of quick sort?
- backtracking
- dynamic programming
- decrease and conquer
- divide and conquer //CORRECT

#### Q36. What is runtime complexity of the list's built-in .append() method?
- O(1), also called constant time //CORRECT
- O(log n), also called logarithmic time
- O(n^2), also called quardratic time
- O(n), also called linear time

#### Q37. What is key difference between a set and a list?
- A set is an ordered collection unique items. A list is an unordered collection of non-unique items.
- Elements can be retrieved from a list but they cannot be retrieved from a set
- A set is an ordered collection of non-unique items. A list is an unordered collection of unique items.
- A set is an unordered collection unique items. A list is an ordered collection of non-unique items. //CORRECT

#### Q38. What is the definition of abstraction as applied to object-oriented Python?
- Abstraction means that a different style of code can be used, since many details are already known to the program behind the scenes.
- Abstraction means the implementation is hidden from the user, and only the relevant data or information is shown. //CORRECT
- Abstraction means that the data and the functionality of a class are combined into one entity.
- Abstraction means that a class can inherit from more than one parent class.

#### Q39. What does this function print?
```
def print_alpha_nums(abs_list, num_list):
    for char in abc_list:
        for num in num_list:
            print(char, num)
    return

print_alpha_nums(['a', 'b', 'c'], [1, 2, 3])

```
- 
```
a 1
a 2
a 3
b 1
b 2
b 3
c 1
c 2
c 3
```
- 
```
['a', 'b', 'c'], [1, 2, 3]
```
- 
```
aaa
bbb
ccc
111
222
333
```
- 
```
a 1 2 3
b 1 2 3
c 1 2 3
```