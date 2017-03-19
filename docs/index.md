# The Basics

Kai is a new programming language that aims to be C with a touch of modernism. Kai is about the freedom and speed. Write code how you want, we'll stay out of your way. If you're new here, [Install Kai](/install) to get started!

## Getting Started

As per tradition, let's start with a hello world application.

```swift
print("Hello, world!")
```

!!! warning
    Statements in global scope are temporarily disabled. As global scope is limited to declarations, please define a [main](/entry-point) procedure.

Unlike many other programming languages, Kai doesn't require you to explicitly define a [`main()`](/entry-point/) or import any [modules](/module/) to build an application.

## Variables and Constants
Variables and constants match a name to a value (similar to `x` in algebra). Variables are values that are allowed to change (`mutable`/`runtime`) while constants are values that aren't allowed to change (`immutable`/`compile-time`).

### Simple Declarations
The syntax for declaring a variable is quite straightforward. Simply provide a name followed by `:=` and a value.

Here's an example:

```swift
x := 15
```

The previous line created a variable named `x` and set its value to `15`.

It's also possible to declare a variable using another variable (or constant) as its value. The following example will create a variable `a` with the value `1` and another variable `b` with the value of `a` (also `1`).

```swift
a := 1
b := a
```

You can combine the previous example into a single line.
```swift
a, b := 1, 1
```

As a variable is a mutable value, you can change its value by using the [assignment operator](/operator/) (`=`)

```swift
x := 0
x = 7
```

`x` will now have the value `7`. Try printing it:

```swift
print(x)
```

If you want to declare a value as a constant, you can use the [constant declaration operator](/operator/) (`::`).

```swift
seven :: 7
```

Since a constant is immutable, the following code will cause an error:

```swift hl_lines="2"
seven :: 7
seven = 2 // error
```

### Type Annotation
In most cases, the compiler is smart enough to infer the type of variable you want to use, but in certain cercumstances you may be required to give it a hint/annotation. Doing so is quite similar to a normal variable declaration.

First, let's start with annotating a variable value:

```swift
age : int = 23
```

Now, a constant value:

```swift
five : int : 5
```

!!! note
	Learn more about `Kai Types` [here](/types/basic/)
	 and `Compile Time Execution` [here](/compile-time).

## Naming
Variables and constants can be named just about any unicode character other than whitespace and mathematical symbols. When a value is named, that name cannot be used again within the same [scope](#scope). Names (`identifiers`) cannot start with a number, but a number can be included within the name.

```swift
이름 := "만세"
🔒  := true
τ   := 6.28
```

## Scope and Shadowing
Blocks of code are organised as scopes. A scope is defined as the code in-between `{` and `}`. You are entering a scope when you see `{` and exiting when you see `}`. Variables and constants are allowed to enter a scope, but they are not allowed to leave the scope they are declared in.

For example:

```swift
message := "Hello!"

{
	print(message) // Prints "Hello!"
}
```
is allowed because `message` is going deeper in scope. But:

```swift hl_lines="5"
{
	message := "Hello!"
}

print(message) // Error "Unknown identifier `message`"
```

is not allowed because `message` is not allowed to exit the scope it was declared in. When entering a new scope, you are allowed to reuse names. This feature is known as `shadowing`.

```swift
aValue := 8675309
{
	aValue := "I shadowed a value."
	print(aValue) // Prints "I shadowed a value."
}

print(aValue) // Prints "8675309"
```

