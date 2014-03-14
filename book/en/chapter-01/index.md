# Introduction

## About

This is a book about Scala. An approachable book, with clear writing and simple examples, with minimal ivory tower academic overtones about functional programming. If you're here for the functional programming, don't worry! I began writing this book with the interest in producing a manuscript similar to Learn You a Haskell [@lipovaca11]. In fact I'm essentially copying the topic layout of Learn You a Haskell and covering functional programming in Scala first.

I've been writing Scala for a very short time - a year as of 2014. I don't consider myself an expert. I have been programming computers for two decades so that counts for something. Writing this book is all about the learning process - how to write a book, what tools to use, how self publishing works, and most importantly becoming an expert in Scala.

I hope you find this book as fun to read and informative as I [really hope I] had writing it and learning along the way!

## What is Scala?

Scala is a hybrid object-oriented and functional programming language that runs on the Java Virtual Machine (JVM). It supports functional programming paradigms like pattern matching, immutability, and higher order functions as well as the pillars of object oriented design: encapsulation, abstraction, polymorphism, and inheritance.

Scala is also a statically typed language and in many cases the compiler can infer types based on usage. The type system is incredibly powerful but at times can be difficult to wrap one's head around. Scala's type system is also unified; that is, unlike Java which has both a primitive `int` and an `Integer` class, Scala only has an `Integer`.

The syntax for Scala is similar to C-style languages with curly braces though semicolon line endings are both optional and strongly discouraged.

As it runs on the JVM and is interoperable with Java one might expect certain Java requirements be met, like type erasure and support for checked exceptions. Scala provides a feature called a manifest that gets around type erasure by carrying type information at runtime, and Scala does not require checked exceptions be handled and even shields the programmer when working with external Java libraries where a checked exception may be required.
