# Introduction
* It is used to check satisfiability of logical formulas over one or more theories.
* It is a low-level tool and is used best in combination with the other tools.
* Z3 script is a sequence of commands. Some examples are like help, echo etc. 
* Z3 maintains a stack of user provided formula and declarations. These formulas are the assertios provided by the users.
* A formual F is **valid** if F is always evaluates true for any assignment of appropriate value to its uninterpreted function and contant symbols.
* A formula F is **satisfiable** if F evaluates to true for some assignment of appropriate value.
* **Validity** is about finding the proof for a statement while **satisfiability** is about finding a solution to a set of    constraints. 
* Functions are total in Z3 which means they don't have side-effects. 
* Z3 has builtin support for integer and real constants.
* Z3 has support for division, integer division, modulo and remainder operators. Internally all these operations are 
  mapped to multiplication.
* In Z3, division by 0 is satisfied but the result is not specified.
* Z3 supports bit-vector operations.
* Z3 contains a decision procedure for the basic theory of arrays.

