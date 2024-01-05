# Python Notes


## What is a virtual environment?

- It represents an isolated environment to manage dependencies without them conflicting with other projects.


### How to create a venv?

- In the root of your new project, run the following command in your terminal:
```python -m venv .venv```


### How to use a venv?

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
     "name": "mMttheus",
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
     { "name": "Guilherme", "age": 27 },
     { "name": "Maria", "age": 32 },
     { "name": "John", "age": 18 },
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
     "name": "Guilherme",
     "level 1
}
```

### adding new keys and values to the dictionary

```
player['life'] = 100
player['damage'] = 25.2
player['clan'] = "Pythonistas"
player['leader_clan'] = True
```

### displaying the dictionary with the added information

print(player)

### Exit

```
{
     'name': 'Guilherme',
     'level 1,
     'life': 100,
     'damage': 25.2,
     'clan': 'Pythonistas',
     'leader_clan': True
}
```