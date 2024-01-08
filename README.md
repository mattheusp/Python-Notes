# Python Notes


## What is a virtual environment?

- It represents an isolated environment to manage dependencies without them conflicting with other projects.


### How to create a venv?

- In the root of your new project, run the following command in your terminal:
```python -m venv .venv```


### How to use venv?

- After entering venv, install the project dependencies (modules, libs in general)


### How to exit/deactivate venv?

- To exit venv, simply execute the following command, or close the terminal.

```deactivate```

___


## List dependencies with requirements.txt

- To install the requests module, run:

```pip install requests```


### Listing installed dependencies:

- To view the dependencies and their installed versions:

```pip freeze```

### Saving dependencies in requirements.txt

- Store all installed dependencies:

```pip freeze > requirements.txt```


___

## What are dictionaries in python?

- Dictionaries in python is a type of structure that stores information in key and value pairs. Each key is unique for accessing and selecting the corresponding value.

```
person = {
       "name": "Mattheus",
       "age": 21,
       "contact": "https://www.linkedin.com/in/mattheuspereira/"
}
```

### Information grouping

- Dictionaries are useful for organizing and retrieving data efficiently.

```
print(f"Name: { person['name'] }")
print(f"Age: { person['age'] }")
print(f"Contact: { person['contact'] }")
```

Note that with a single person variable, we can store different types of information, such as name, age and contact.


### List of dictionaries


- We can also build dictionary lists and display the information through loops:

### creating a list of dictionaries

```
people = [
       { "name": "Mattheus", "age": 27 },
       { "name": "Jessica", "age": 32 },
       { "name": "Lucas", "age": 18 },
]
```

### displaying users in a loop in the list

```
for p in people:
       print(f"Name: { p['name'] }, Age: { p['age'] }")


Name: Matheus, Age: 21
Name: Jessica, Age: 28
Name: Lucas, Age: 30
```


### Adding new information to the dictionary

We can add new information to the dictionary as follows:


### creating a dictionary with initial information

```
player = {
       "name": "Mattheus",
       "level 1
}
```

### adding new keys and values to the dictionary

```
player['life'] = 100
player['damage'] = 25.2
player['clan'] = "Pythonists"
player['leader_clan'] = True
```

### displaying the dictionary with the added information

print(player)

###Exit

```
{
       'name': 'Mattheus',
       'level 1,
       'life': 100,
       'damage': 25.2,
       'clan': 'Pythonists',
       'leader_clan': True
}
```

___


##Conditionals

- Changes the execution flow of our programs


### Structure of a conditional

if (condition)
       // do something

or else (other condition)
       // do something

otherwise
       // do something

- The condition must be true for the instruction block to be executed.

- We can use operators, variables, and even call functions with returns to validate a conditional.

### Examples using python

```
age = 18

if age >= 18
       print("adult")

elif age >=16:
       print("teen")

elif age >=13:
       print ("pre teenager")

else:
       print("child")
```

In the example above, I created a variable called age, which takes the value of 18.

Then I created some conditions to display a message

1. If the age is greater than or equal to 18: adult

2. Or, if the age is greater than or equal to 16: teenager

3. Or, if the age is greater than or equal to 13: pre-adolescent

4. Otherwise: child

___

## Lists

- These are ordered collections of items in Python

- The indices in a list can be of different types and can be accessed through indexes.

### Example using Python

´´´
fruits = ['apple', 'banana', 'orange']
       print (fruits[0])
´´´

___

## Repetitions (loops)

- 'for' and 'while' are control structures used to execute a block of code multiple times.

- 'for' is generally used when the number of iterations is known in advance.

- 'while is when the stopping condition is not known in advance.

### Example of 'for' in Python

for number in range (5):
       print(number)

'while' example in python

counter = 0
while counter <5:
print (counter)
counter +=1

___

## Dictionaries

- Dictionaries are data structures that store key-value pairs

- Each value is associated with a unique key, allowing quick access to data.

### Example used python

´´´student={'name': 'João', 'age':20, 'course': 'Engineering'}
print(student['age'])

___


## Functions and parameters

- Functions are blocks of code that perform a specific task and can be reused in different parts of the program.

- Parameters are values that can be passed to a function to customize its behavior.


### Python example

´´´
def greeting(name):
       print(f''Hello, {name}'')

greeting('Maria')
´´´

___