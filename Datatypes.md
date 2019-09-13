# Datatypes supported by Z3
* **Records**
  Specified as single constructor and as many arguments as record elements. The number of arguments to a record are always the same.
  The type system doesn't allow to extend records and there is no record subtyping.
* **Recursive datatypes**
  ```
  (declare-datatypes (T) ((Lst nil (cons (hd T) (tl Lst)))))
  (declare-const l1 (Lst Int))
  (declare-const l2 (Lst Bool))
  ```
* **Mutually recursive datatypes**
  Example: Tree
* **Scalars** (enumeration types)
