# Week 01: Postman Basics + First JS Tests

## Topics Covered
- Postman collections and requests
- Writing JavaScript tests in Postman
- Validating status codes, headers, and JSON bodies

## Challenge
1. Create a request to `https://jsonplaceholder.typicode.com/posts/1`
2. Add at least 3 tests:
   - Check status code
   - Check `userId` or `title`
   - Check response time < 200ms

MY CODE:

// TODO: Add your own tests here for the challenge!
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Content-Type is application/json", function () {
    pm.response.to.have.header("Content-Type");
    pm.expect(pm.response.headers.get("Content-Type")).to.include("application/json");
});

const jsonData = pm.response.json();

pm.test("Response time is less than 200ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(200);
});

pm.test("Post contains a title", function () {
    pm.expect(jsonData.title).to.be.a("string").and.to.not.be.empty;
});
