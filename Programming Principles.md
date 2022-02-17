# Programming Principles
- - - -
These principles are used for writing good code

- - - -
# KISS

 keep it stupid simple (make the code easy to read and understand) 

- - - -
# DRY 

Don't repeat yourself (use functions)

- - - -
# SRP 

Single responsibility principle. 

every module, class, or function should have responsibility over a single part of the functionality provided by the software, and that responsibility should be entirely encapsulated by the class, module or function. 

All its services should be narrowly aligned with that responsibility

- - - -
# SoC

Separation of Concerns principle 

like the single responsibility principle but on a more abstract level. 

A program should be designed so that it has many different non-overlapping encapsulations, and these encapsulations shouldn’t know about each other.

A well-known example of this is the model-view-controller (MVC) paradigm


- - - -
# Open/Closed

make the code open to extension but closed to modification.

- - - -
# Composition > Inheritance

objects with complex behaviors should do so by containing instances of objects with individual behaviors rather than inheriting a class and adding new behaviors.

- - - -
# YAGNI

you aren’t gonna need it principle

Never code for functionality that you may need in the future.

Just follow the above principles so it will be easy to code that functionality in the future.

- - - -
# Avoid Premature Optimization

no premature optimization principle. 

Don't optimise code before it’s necessary.

- - - -
# Refactor

Code refactoring is the process of restructuring existing computer code—changing the factoring—without changing its external behavior. 

Refactoring is intended to improve nonfunctional attributes of the software. 

Advantages include improved code readability and reduced complexity. 

These can improve source-code maintainability and create a more expressive internal architecture or object model to improve extensibility.

- - - -
# Clean Code > Clever Code

* Write readable code. 

* Use comments when necessary  

* Each code you rewrite/add - make it prettier.

- - - -
# DRTW

Don’t reinvent the wheel (use existing functionalities, frameworks, libraries…)