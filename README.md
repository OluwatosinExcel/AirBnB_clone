# AirBnB_clone
## Welcome to the AirBnB clone project!
## Project Description
This is a clone of AirBnB which is an American company that operates an online marketplace for lodging, primarily homestays for vacation rentals and tourism activities.
The goal of this project is to deploy on my server a simple copy of the [AirBnB website](https://www.airbnb.com/)
### Files and Directories
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
### How to start it:
### How to use it:
### Example:
