# Commands in Z3:
* ## declare_const 
     (declare_const a Int) declares a variable a of type int.
* ## declare_func
     (declare_fun f (Int Bool) Int declares a function f which takes 
     Int and Bool type as two arguments and produces Int as output.
* ## assert
     (assert (> a 10)) adds a formula into Z3 stack. A set of formula is satisfied in Z3 if there is an 
     interpretation that satisfies the formula that is make it true.
* ## (check-sat)
     determines whether the current formulas on the Z3 stack are satisfiable or not. 
     If formula is satisfiable Z3 returns ###sat. If it is not statisfiable then returns ###unsat.
     Z3 can also return ###unknown when it can't determine whether a formula is satisfiable or not.
* ## (get-model)
     Retrives an interpretation that makes all formulas on the Z3 internal stack true. 
* ## (push) 
     Creates a new scope by saving the current stack size.
* ## (pop) 
     Removes any assertion or declaration oerformed between it and the matching push.
* ## (reset)
     Removes all the declarations and assertions. 
* ## (display t) 
     Applies the Z3 pretty-printer to the given expression t. 
* ## (simplify t) 
     Simplfies display a possibly simpler expression equivalent to t.
