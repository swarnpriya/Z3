# Propositional Logic
* Z3 supports the Boolean operators like and, or, xor, not, => (implication), ite (if-then-else), bi-directional (=)
* Example:
```
(declare-const p Bool)
(declare-const q Bool)
(define-fun demorgans () Bool
  (= (not (and p q)) 
      (or (not p) (not q))))
(assert (not demorgans))
(check-sat)
```
The above formula is valid as it is Demorgan's law (not (and p q)) = (not p) \/ (not q) hence if we prove that (not demorgans)
is unsatisfiable.
