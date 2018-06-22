---
layout: page
title: Pre-Work
subheading: Day 1: Integers and Floats
---

## Integers & Floats

Integers and floats are both what we could call numbers in everyday life. In programming it helps us to be a little more specific. The quickest way to distinguish between an integer and a float is that a float has a decimal and some digits after that decimal. This is true even if those digits after the decimal are 0's. With that in mind:

* Integers include:
    * 1
    * 5
    * 10
    * 100
    * -100
    * 0
    * 5_489_920 (in this case the `_` character replaces commas)
* Floats include:
    * 1.0
    * 5.4780
    * 10.234789
    * 100.1
    * -100.429
    * 0.0
    * 5_489_920.43820

## So what?

### Overview

Integers and floats can seem very familiar since we use numbers so frequently in everyday life. However, in Ruby there are some interesting things we can do with even these simple tools.

### A Brief Introduction to Ruby

Ruby is language that was developed to allow and encourage programmers who used it to write their code in an 'object oriented' paradigm. You may have heard of 'object oriented programming' or 'object oriented design' before, but what does that really mean?

This sounds like a very simple and straightforward question, but many people have had much to say about this particular topic. You will learn much more in your time at Turing and beyond. For right now, here are some basics:

* Everything in Ruby nearly everything is an object. So, `1` is an object. So is `"Hello!"`. So are `nil`, and `true`, and `[]`, and `{name: "Fred", age: 23, occupation: "Plumber"}`.
* In Ruby, you can call methods on objects. Some people talk about sending messages to an object. We do this using 'dot notation'.
* For example, if we wanted to find out the class of a particular object (i.e. what kind of thing it is), we can usually call the method `class` on that thing. More specifically, we could type `5.class` into one of our Ruby programs and Ruby would tell us that 5 is an instance of the `Integer` class. Another way to say this is that we called the *method* `#class` on `5` and the method *returned* `Integer`.
* Instances of different classes respond to different methods, or, less technically, you can call different methods on different types of things. To give a specific example, you can call the method `#odd?` on an Integer like `5`, but you can't call it on a String like `"Hello!"`

### Back to Integers & Floats

Each of these classes allow you to do basic mathematical operations on them. Open a Pry session by typing `pry` in your terminal window and hitting enter. Then enter the following commands and see what they return. In each case below we're calling a method on an Integer or a Float.

It might help to arrange your windows so that you can see both the list below and your terminal window so that you don't have to switch back and forth between the two. Be sure to see if you can describe in your own words what each method does when you see the result.

```ruby
1.class
1.0.class
0.class
1000.class
1_000.class
1_000.234.class
1 + 1
1 + 1.0
1.0 + 1
(1 + 1).class
(1.0 + 1).class
4 / 2
4 / 2.0
(4 / 2.0).class
(4 / 2).class
3 / 1.5
3 / 2
3 % 2
4 % 2
5 % 2
0 % 5
1 % 5
2 % 5
3 % 5
4 % 5
5 % 5
6 % 5
5 * 5
5 ** 2
5.0 ** 2
2 ** 2
4 ** 4
4.even?
4.odd?
3.odd?
3.odd?.class
4.0.to_i
5.to_f
```

### Synthesize

In your own words what does each of the following methods do?

* `#class`
* `#even?`
* `#odd?`
* `#+` (this is tricky! If you look at the examples above, `+` is actually a method that you're calling on the number before the plus sign)
* `#/` (similar thing!)
* `#**` (you're getting the picture)

What will be the class of the thing that each of the methods below returns.

For example: `1 + 1` returns 2, which is an Integer. If you're ever unsure, use pry to determine the answer by wrapping the expression below in parenthesis and then calling `#class` on the result (e.g. `(1 + 1).class` would return Integer).

* 1 + 1
* 1 + 1.0
* 1.0 / 1
* 1.odd?
* 5.even?
* 4.275.to_i
* 5.to_f
* 4 % 3
* 6 / 2
* 6 / 4
* 6 / 4.0
