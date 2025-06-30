# Week 04 Quiz: Postman Variables & Chaining

## Multiple Choice

**1. Which variable type is only available in the currently selected environment?**  
A) Global  
B) Environment  
C) Collection  
D) Local

**2. What does `pm.environment.set("foo", "bar")` do?**  
A) Sets a global variable  
B) Sets a variable only for the current request  
C) Sets an environment variable  
D) Creates a local constant

**3. What is the correct way to use a variable inside a request URL?**  
A) `https://api.com/{{variable}}`  
B) `https://api.com/$variable`  
C) `https://api.com/::variable::`  
D) `https://api.com/variable={}`

**4. In which tab would you typically use `pm.environment.get()`?**  
A) Pre-request Script  
B) Headers  
C) Tests  
D) Both A and C

## Short Answer

**5. Write a test to check that the value of a variable called `userToken` is not undefined.**

**6. After a POST request returns a JSON body, write code to store the `id` field in a variable called `createdId`.**

**7. How can you use the `createdId` variable in the body of a future POST request? Provide a JSON example.**

