# The expression problem

refers to a certain challenge encountered when:
+ trying to define the grammar for a simple language
+ we're trying to interpret sentences of this language


## Key insight into language paradigms

As explained in the *craftinginterpreters* the expression problem offers us a
way to gain some insight into the nature of specific programming paradigms. In
particular, it provides an answer to the question why are object oriented
programs so called. 

The diagram in the book depict a table with types/classes making up rows and
methods making up columns. The essential problem is that the object oriented
paradigm makes it easy to add new rows, and the functional(MP) paradigm. 

The question for the implementation in the book was what sort of implementation
would make it possible to achieve easy column based expansion of the table?

The approach suggested in the book is to use the visitor pattern. 


## The visitor pattern

### things about the pattern that are confusing
+ it has nothing to do with seeing grandma
+ the meaning of the accept method is also not very clear
+ although it's being used here to traverese trees, it has nothing to do with
  trees

### things about this pattern that are clear
+ it's about approximating the functional style in an object oriented language
+ it will let us add new columns to the table easily
+ it solves the problem by adding a layer of indirection (we set up a script to
  generate the abstract syntax tree)



## what is the functional complement to the visitor pattern?


In object oriented programming, classes are used as a way to create objects and
maintain state. In functional programming, we do not hold state. 


