# Basic Types

## Integers

```swift
x: int = 5
```

```swift
x: int 5
y: i64 = x
```

```swift
z: i8 = 0
```

## Reals

```swift
pi: float = 3.14
tau: f64 = 6.28
```

## Strings

```swift
name: string = "John"
```

## Unconstrained Types
```swift
myproc :: (anI32: i32) -> Void {
	// ...
}

// could be any integer type and will default to i64 if not constrained.
unconstValue := 5


// calling this procedure constrains the value to type i32.
myproc(anI32: unconstValue)
```