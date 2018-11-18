So, I recently started learning [Elixir][1] and, I want to share some of the quirks of a functional programming language and functional paradigm in general


## What the heck is Functional Programming anyways?

Wikipedia puts it this way,
>In computer science, functional programming is a programming paradigm--a style of building the structure and elements of computer programs--that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. It is a declarative programming paradigm, which means programming is done with expressions or declarations, instead of statements.

It's actually well put together. In simple terms, functional programming is a way of thinking about problems in terms of small, composable functions.

But, that's not convincing enough for me to care about any of these, you might say. I'd say, hold your horses there, as I've yet to show you some of the cool features functional paradigm has up it's sleeve. Let's get on with it then, shall we?

- Functions as first class citizens

    What it means is that functions are a data type just like integers or strings. They have a literal representation, can be stored in variables, can be passed as arguments, and so on.

- Functions without side effects

    Functions are deterministic. You can infer what a function does based on it's inputs and output. They don't modify it's inputs. So, now the order of execution of side-effect-free functions is not important. This makes your program concurrent in a very transparent way. neat!

- Declarative Style Programming

    This is one of the cool ones. Programs are trees of expressions, each of which returns a value. Simply put, Functional programming languages allows us to express our intent clearly. It allows us to express what we want to achieve rather than how it's implemented. This is quite a contrast to imperative languages where we explicitly express how to achieve something in terms of statements.

I think you should give it a try. Regardless of weather you end up using it daily or not, it'll surely make you a better programmer. It'll give you a different perspective, And learning radically different perspectives helps you approach problems from new directions, potentially leading to novel solutions.


Alright the, In the next post, I'll go over some of specific features of [elixir][1]. 

> akash

[1]: https://elixir-lang.org/
