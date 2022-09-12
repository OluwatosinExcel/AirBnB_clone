# AirBnB_clone - The console
## Welcome to the AirBnB clone project!
### Resources
* [cmd module](https://docs.python.org/3.8/library/cmd.html)
* [uuid module](https://docs.python.org/3.8/library/uuid.html)
* [datetime](https://docs.python.org/3.8/library/datetime.html)
* [unittest module](https://docs.python.org/3.8/library/unittest.html#module-unittest)
* [args/kwargs](https://yasoob.me/2013/08/04/args-and-kwargs-in-python-explained/)
* [Python test cheatsheet](https://www.pythonsheets.com/notes/python-tests.html)
## Project Description
This is a clone of AirBnB which is an American company that operates an online marketplace for lodging, primarily homestays for vacation rentals and tourism activities.
The goal of this project is to deploy on my server a simple copy of the [AirBnB website](https://www.airbnb.com/)
## Files and Directories
* The `models` directory contain all classes used for the entire project. A class called "model" in an OOP project is the representation of an object/instance.
* The `tests` directory contains all unit tests.
* `console.py` file is the entry point of the command interpreter.
* The base class of all the models is the `models/base_model.py` file. It contains the following;
- attributes: `id`, `created_at` and `updated_at`
- methods: `save()` and `to_json()`
* The `models/engine/file_storage.py` file contains all storage classes (using same prototype).
## Command Interpreter
Command interpreter serves as a means to manipulate data without visual interface, like in a Shell (perfect for development and debugging). The following can be done with the command interpreter:
- Create a new object (e.g a new User or a new Place)
- Retrieve an object from a file, a database etc.
- Do operations on objects (e.g count, compute stats, etc.)
- Update attributes of an object
- Destroy an object
### Execution
* In interactive mode:
```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```
* In non-interactive mode:
```
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
```
* All the tests passed `$ echo "python3 -m unittest discover tests" | bash` in non-interactive mode.
## Properties
### Python Scripts
* All codes in this project uses the pycodestyle (version `2.8.*`)
* Modules documentation:
```
python3 -c 'print(__import__("my_module").__doc__)'
```
* Classes documentation:
```
python3 -c 'print(__import__("my_module").MyClass.__doc__)'
```
* Functions (inside and outside a class) documentation:
```
python3 -c 'print(__import__("my_module").my_function.__doc__)'
```
And
```
python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'
```
### Python Unit Tests
* All test files are located in the `tests` folder
* The [unittest module](https://docs.python.org/3.4/library/unittest.html#module-unittest) was used for this project
* All test files are python files (extension: `.py`)
* All test files and folders start with `test_`
* All tests were executed by:
```
python3 -m unittest discover tests
```
Alternatively, tests could be executed by
```
python3 -m unittest tests/test_models/test_base_model.py
```
* Module documentation:
```
python3 -c 'print(__import__("my_module").__doc__)'
```
* Classes documentation:
```
python3 -c 'print(__import__("my_module").MyClass.__doc__)'
```
* Functions (inside and outside a class) documentation:
```
python3 -c 'print(__import__("my_module").my_function.__doc__)'
```
And
```
python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'
```
## Usage
* Starting the console in interactive mode:
```
$ ./console.py
(hbnb)
```
* Using `help` to see available commands:
```
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  count  create  destroy  help  quit  show  update

(hbnb)
```
* Quitting the console:
```
(hbnb) quit
$
```
## Authors
- [Uduak Umanah](https://github.com/Eyakenojnr/)
- [Uniquexcel](https://github.com/Uniquexcel)
