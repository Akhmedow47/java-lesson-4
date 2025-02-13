# Closure and Recursion 
## What is a Closure?

*A closure is a function that remembers variables from its outer scope even after the outer function has finished executing. This allows functions to retain access to variables even when they are executed later.*

### Why Use Closures?

  ✔ Data Privacy (Encapsulation) - Variables remain private inside functions.   
  ✔ Maintaining State - Helps functions remember past values.  
  ✔ Avoiding Global Variables - Keeps code clean and modular.  
  ### Basic closure 
     function outer() {
                  let count = 0; // Private variable
                 return function() {
                  count++;
        return count;
    };
    }

    const counter = outer();
    console.log(counter()); // Output: 1
    console.log(counter()); // Output: 2

    🔄 Recursion

## What is Recursion?

*Recursion is a function that calls itself until a base case is met. It is useful for problems that can be broken down into smaller subproblems.*

### Why Use Recursion?

   ✔ Solves Complex Problems Easily (e.g., Tree Traversal, Searching)  
   ✔ Removes the Need for Loops in some cases  
   ✔ Makes Code More Readable (if used correctly)  

###Example 1: Factorial Using Recursion    

       function factorial(n) {    
       if (n === 0 || n === 1) return 1; // Base case   
       return n * factorial(n - 1); // Recursive call
                 }

     console.log(factorial(5)); // Output: 120
     
  ## 🎯 Summary

### Concept
> Closure

> Recursion
#### Key Idea
- Functions remember variables from their outer scope


- A function calls itself to solve smaller subproblems

Closures are great for data privacy and state management, while Recursion helps in breaking problems into smaller subproblems.


