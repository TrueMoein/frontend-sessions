# Chapter 1

### Why Functional Programming?
This first chapter's purpose is to answer questions like :
 - Why should I use FP style with my code?
 - How does Functional-Light JavaScript compare to what others say about FP?

#### At a Glance [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#at-a-glance)
quick remarks about this code comparison:

 - the former snippet feels closer to comfortable/readable/maintainable
 **BUT**
 that second snippet will eventually become a lot more natural, maybe even preferable! 
 - The goal is to illustrate the pros/cons of various patterns and enable you to make those decisions

#### Confidence [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#confidence)
 - code that you cannot trust is code that you do not understand
 **OR**
  code that you don't understand is code you can't trust.
 - I don't mean to suggest tests are bad. But I do think we should aspire to be able to understand our code well enough that we know the test suite will pass before it runs. 
 - When we using FP, Someone who understands FP can read and verify that the program will do what they want
 - avoid the most common causes of program bugs!
  
#### Communication [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#communication)
 - code is as a means of communication with other human beings.
 - It's widely estimated that developers spend **70%** of code maintenance time on reading to understand it.
 - For example, once you learn what map(..) does, you'll be able to almost instantly spot and understand it when you see it in any program. But every time you see a for loop, you're going to have to read the whole loop to understand it.
 
 
#### Readability [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#readability)
  - Readability is not a binary characteristic. It's a largely subjective human factor describing our relationship to code.
  
#### Perspective [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#perspective)
   - this book will try to focus more on the base concepts and less on the fancy fluff.
#### How to Find Balance [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch1.md/#how-to-find-balance)
 - "You aren't gonna need it" **(YAGNI)** is a principle of extreme programming (XP) that states a programmer should not add functionality until deemed necessary.
 - Remember, every single line of code you write has a reader cost associated with it.
 
 
 # Chapter 2
 
 ### The Nature Of Functions
 
 ##### What Is a Function? [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#what-is-a-function)
  ###### function is a collection of code that can be executed one or more times.
##### Brief Math Review [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#brief-math-review)
 - we can define functions with all sorts of input(s) and output(s)
 
##### Function vs Procedure [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#function-vs-procedure)
 - procedure is a set of coded instructions that tell a computer how to run a program or calculation.
 - function takes input(s) and definitely always has a return value.

##### Function Input [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#function-input)
 - Arguments are the values you pass in, and parameters are the named variables inside the function that receive those passed-in values.
 
##### Defaulting Parameters [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#defaulting-parameters)
 - As of ES6, parameters can declare default values. In the case where the argument for that parameter is not passed,
 or it's passed the value undefined, the default assignment expression is substituted.
 
##### Counting Inputs [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#counting-inputs)
 - Arity is the number of parameters in a function declaration
 - a function with arity 1 is also called "unary"
 - a function with arity 2 is also called "binary"
  - a function with arity 3 or higher is called "n-ary".
  - So, if you really want to design a function that can account for an arbitrary number of arguments to be passed in, use ...args (or whatever name you like) on the end.

##### Arrays of Arguments [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#arrays-of-arguments)
 -  multiple values and ... spreading can be interleaved,
 
##### Parameter Destructuring [Link](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch2.md/#parameter-destructuring)
 - Destructuring is a way to declare a pattern for the kind of structure (object, array, etc.) that you expect to see,
 and how decomposition (assignment) of its individual parts should be processed. 

 

 
 