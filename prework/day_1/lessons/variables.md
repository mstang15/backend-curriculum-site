---
layout: page
title: Pre-Work
subheading: Day 1: Variables
---

## Storing Things

Every now and again we want to store values so that we can use them later. In order to do this, we use variables. Variables provide us the opportunity to name a concept, giving it meaning so that our code is easier to decipher by other developers or even our future selves (reading your own code and not knowing what it means is officially *the worst*).

There is a single operator that allows us to do this: `=`. A single equals sign will assign the value of a particular expression to a variable. It may seem strange at first, but assignment (the act of assigning a value to a variable) goes from right to left. Thus:

```ruby
current_age = 5
```

assigns the value `5` to the variable `current_age`.

Variables can also hold the value of expressions that Ruby will need to evaluate. For example:

```ruby
age_next_year = 5 + 1
```

A better way to calculate the `age_next_year` value would be to use `current_age` in the calculation itself.

```ruby
age_next_year = current_age + 1
```


Once a variable has been assigned, you can use that variable in place of the value it holds. For example, if we start with the `current_age` variable we defined above, we could then use it to calculate how many years until the person would be eligible for a driver's license. The code would look something like the following:

```ruby
current_age = 5

legal_age_of_driver = 16
years_until_eligible = legal_age_of_driver - age
```
