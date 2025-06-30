# Week 05 Quiz: Conditional Logic in Postman Tests

## Multiple Choice

**1. What does `typeof` return when checking a string?**  
A) "String"  
B) "text"  
C) "str"  
D) "string"

**2. How do you check if a property exists in an object?**  
A) `obj.property !== undefined`  
B) `"property" in obj`  
C) `pm.expect(obj).to.have.property("property")`  
D) All of the above

**3. Which of the following is a correct way to write an if-statement in Postman test scripts?**  
A) `if pm.response.code == 200:`  
B) `if (pm.response.code = 200)`  
C) `if (pm.response.code === 200)`  
D) `if response.code 200 then`

## Short Answer

**4. Write a test that only runs if a field called `status` exists in the response. It should assert that `status` equals `"active"`**

**5. How would you test that an array is not empty before looping through it? Provide sample code.**

**6. Write a Postman test that checks if a `username` field is present, and if so, that it contains no spaces.**
