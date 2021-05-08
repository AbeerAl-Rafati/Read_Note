# Functional Programming in Javascript 

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data   


#### Pure functions  
It returns the same result if given the same arguments (it is also referred as deterministic), It does not cause any observable side effects   

* Pure functions benefits
The code’s definitely easier to test. 
#### Reading Files  
If our function reads external files, it’s not a pure function — the file’s contents can change.  

#### Random number generation  
Any function that relies on a random number generator cannot be pure.  



### Higher-order functions
* takes one or more functions as arguments, or  
* returns a function as its result  




* *Filter*  
higher order function to receive the even function  


 
 * *Map*  
 The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.  

 
  * *Reduce*  
  The idea of reduce is to receive a function and a collection, and return a value created by combining the items.  

  