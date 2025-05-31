# Data Structures and Object Oriented Programming

## IDE s
- Google Colab
- VS Code
- Jupyter

## Data strcutures

### Fundamental
  - Integers
  - Float
  - Strings
  - Boolean

### Non fundamental
  - Lists - Ordered changeable collections that can store different items e.e. 
  my_list = [1, "fruit", 3.5]

  - Tuples - like Lists but immutable i.e. elements cannot be changed
  my_tuple = (1, "fruit", 3.5)

  - Dictionaries - hold key value pairs
  my_dictionary = {"name" : "John", "age" : 30}

  - Sets - unordered collection of unique elements. Useful for membership testing, eliminating duplicate entries, and performing mathematical set operations like union, intersection, and difference.

## Lists and Dictionaries
 - Use Lists when order matters, duplicates are allowed and want a colleaction that yu can moify easily
 - use dictionaries when you have key value pairs, quick data retreival, flexibility to add or remove key pairs

## Data serialisation and coding conventions
It is the process of converting data structures or objects into a format that can be stored or transmitted and then reconstructed later. Common formats for serialisation include JSON, XML, and binary formats.

- Benefits
    - Data Persistance - Allows the state of the object to be saved to a file for later use.
    - Data exchange - Can be shared across systems
    - performance - efficiently transmitted over networks
 
- Serialisation formats
    - JSON - python import json data = ('name': 'Alice', 'age': 25} json_str = json. dumps(data)
    - Pickle - import pickle data = {'name': 'Alice', 'age': 25} with open('data.pkl', 'wb') as f: pickle.dump(data, f)
    - XML - import xml.etree.ElementTree as ET data = ET. Element('data') name = ET. SubElement(data, 'name') name.text = 'Alice'
 
## Coding conventions
- Indentation
- Line length - upto 79 characters
- Naming conventions
- white space
- COmments

## OOP
 - Encapsulation - Encapsulation is achieved when each object keeps its state private, inside a class. Other objects don’t have direct access to this state. Instead, they can only call a list of public functions — called methods.
 - Abstraction - Applying abstraction means that each object should only expose a high-level mechanism for using it.This mechanism should hide internal implementation details. It should only reveal operations relevant for the other objects.
 - Inheritance - When objects are very similar, they share common logic but they’re not entirely the same. To keep the common logic and extract the unique logic into a separate class can be achieved by inheritance. i.e. create a (child) class by deriving from another (parent) class. This way, we form a hierarchy. The child class reuses all fields and methods of the parent class (common part) and can implement its own (unique part).
 - Polymorphism - ??

Singleton design pattern - ??
