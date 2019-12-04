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