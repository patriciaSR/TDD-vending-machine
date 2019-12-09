# TDD- tutorial

Follow this repository: [learn-tdd](https://github.com/dwyl/learn-tdd)

> The test is the question you are asking
> your code is the answer to the question.
> By having a clear question, you can always check that your code is working,
> because it consistently gives you the same answer(s) ... no surprises, even when you're working with a large, inter-dependent code base!

## Proyect
Imagine you are building a Vending Machine that allows people to buy any item it contains. The machine accepts coins and calculates the change to be returned to the customer, given the item price and the cash received.


## Understand what is needed
Create a function called getChange that accepts two parameters: totalPayable and cashPaid
For a given totalPayable (the total amount an item in the vending machine costs) and cashPaid (the amount of cash the customer paid into the vending machine), getChange should calculate the change the machine should return to the customer
getChange should return change as an array of coins (largest to smallest) that the vending machine will need to dispense to the customer.

## Check the coverage of code 
The coverage is executed (in the browser) using Blanket.js.
Visit: http://localhost:8000/?coverage in your web browser to see coverage.

## Node.js (server-side) Tests 
Install the following node.js modules by running 

`npm install qunitjs qunit-tap istanbul --save-dev`

* QUnit node.js module
* qunit-tap (for command line output)
* Istanbul for server-side code coverage

Run the tests in your terminal:

`node test.js`

And run Istanbul to see the server-side code coverage:

`./node_modules/.bin/istanbul cover test.js`

Execute 
`open ./coverage/lcov-report/index.html` to view the detailed coverage report on your browser.

## Continuous Integration with Travis CI 
To quickly add CI support to your project:
1) Visit: https://travis-ci.org/profile and Login with your GitHub account
2) Enable Travis for your project (Note: The project will need to be hosted on GitHub).
3) Add a `.travis.yml` file to your project's root directory and include the following lines in it:

```
language: node_js
node_js:
  - "node"
```

4) Ensure that you have a `package.json` file with test script.
5) Commit your changes and push them to GitHub
6) Visit the page on Travis-CI for your project to see the build results:

https://travis-ci.org/patriciaSR/TDD-vending-machine
