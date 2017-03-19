# The Basics

Kai is a new programming language that aims to be C with a touch of modernism. Kai is about the freedom and speed. Write code how you want, we'll stay out of your way. If you're new here, [Install Kai](/install) to get started!

## Getting Started

As per tradition, let's start with a hello world application.

```swift
print("Hello, world!")
```

!!! warning
    Statements in global scope are temporarily disabled. As global scope is limited to declarations, please define a [main](/entry-point) procedure.

## Simple Declarations
```swift
myInt := 15
myIntCopy := myInt
```

```swift
myString := "👋"
🔒 := true
```

## Type Annotation
```swift
x: int = 5
```

!!! note
	Continue [here](/types/basic/) to learn more about Kai types.

## Compile-Time Type Annotation
```swift
age: int : 32
```

!!! note
	Learn more about `Compile Time Execution` [here](/compile-time).