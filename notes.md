
* Title
  * Thinking with Propositions as Types

* What this presentation is not about
  * Deep dive into logic, computation, and their history
  * Static typing vs dynamic typing

* TL;DR
  * Math* and programming* are the Same Thing™
    * *mic drop*
    * *walk out*
    * For some values of math, programming, and Same Thing™

  * Logic and computation are equivalent
    * a.k.a Curry-Howard correspondent
    * Linking two fields of study together
    * Discoveries in one field also applies to the other

  * Breaking it down
    * Propositions as types
      * Proposition: statement that is true or false*
      * Type: describes the possible values*
    * Proofs as programs
    * Simplification of proofs as evaluation of programs

  * If you pick one things to remember from this talk, remember this:
    * Writing proofs and writing programming are equivalent

* The paper
  * History
    * Go watch Philip Wadler's Strange Loop video
  * Converting between systems and models
    * How different systems and models can be translated between each other
  * Illustration
    * Similarities between natural deduction and simply-typed lambda calculus
* Tracing the steps
  * Natural deduction
    * Proof calculus
      * Syntax
      * Rules
  * Simply-typed lambda calculus
    * Models of computation
      * Recursive functions
      * Lambda calculus
      * Turing machines
      * All are equivalent
    * We write programs in Turing complete languages
    * Translate our programs to lambda calculus
* Introducing natural deduction
  * Logical operators
    * **Conjunction** (and)                 &, ∙
    * Disjunction (or)                      ∨
    * **Implication** (if A, then B)        ⊃
    * Also called logical connectives   
  * Proof calculus (system for writing proofs)
    * Syntax
      * Premise(s)
      * Conclusion
      * Name
        * Logical operator
        * Introduction/elimination
    * Rules
  * First proof

* Introduction simply-typed lambda calculus
  * Type operators
    * Product type
      * Examples
        * Tuples
          * Python: `("Sue", 40) # Person`
        * Most user-created types in programming languages
          * JavaScript: `{ "name": "Sue", "age": 40 } // Person`
    * Function type
      ```
      function convertToString(/* Number */ a) {
        return a.toString();
      }
      ```
* In practice

* History
  * 1934 => Gerhard Gentzen proposed natural deduction
  * 1940 => Alonzo Church announced simply typed lambda calculus (STLC)
  * 1943 => ENIAC started being built (announced in 1946)
  * **Natural deduction and simply typed lambda calculus were discovered before the first electronic computer**
* Questions


 A -> (B -> C)      A
----------------------
      (B -> C)

```
function curry(func, a) {
  return function(b) {
    return func(a, b);
  };
}
```


```
function dbQuery(/*DatabaseConnection*/ conn, /*Query*/ query) {

}
```



A -> (B -> C)



B -> (A -> C)

```
// Boolean -> Boolean
function not(/*Boolean*/ a) {

}
```

* Resources
  * [Propositions as Types](http://homepages.inf.ed.ac.uk/wadler/papers/propositions-as-types/propositions-as-types.pdf) paper (PDF)
  * [Propositions as Types](https://www.youtube.com/watch?v=IOiZatlZtGU) talk by Philip Wadler
  * Interesting topics
    * Logic systems
      * Propositional, predicate, second-order, intuitionistic, classical, modal, linear
    * Computation
      * Lambda calculus
    *
