# Basic Types

## Integers

```swift
x: int = 5
```

```swift
x: int = 5
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

## Boolean

```swift
hasValue := true
doesNotHaveValue := false
```

## Strings

```swift
name: string = "John"
```

## Unconstrained Types
```swift hl_lines="6 10"
myproc :: (anI32: i32) -> void {
	// ...
}

// could be any integer type and will default to i64 if not constrained.
unconstValue := 5


// calling this procedure constrains the value to type i32.
myproc(anI32: unconstValue)
```
