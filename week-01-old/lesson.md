# Week 01: Intro to API Testing in Postman with JavaScript

Welcome to Week 01! This lesson will introduce you to basic API testing in Postman using JavaScript.

## ✅ Learning Objectives

- Create a GET request in Postman
- Write simple test assertions in JavaScript
- Understand basic Postman collection structure

---

## 🔧 Task: Send a GET Request

1. Open Postman.
2. Create a new **Collection**: `Week 01 - Basic API Testing`.
3. Add a **Request**:
   - **Method**: `GET`
   - **URL**: `https://jsonplaceholder.typicode.com/posts/1`

---

## 🧪 Task: Add JavaScript Tests

In the **Tests** tab of the request, add this:

```javascript
pm.test("Status code is 200", function () {
  pm.response.to.have.status(200);
});

pm.test("Body contains userId", function () {
  var jsonData = pm.response.json();
  pm.expect(jsonData).to.have.property("userId");
});
