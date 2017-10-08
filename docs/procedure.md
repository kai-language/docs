```swift
sum :: (a: i32, b: i32) -> i32 {
	return a + b
}
```

!!! TIP
	Just like variable declarations, multiple parameters of the same type can be declared as a list followed by their type. Example: `mul :: (a, b: i32) -> i32`

Kai also supports multiple returns.
```swift
sumAndMul :: (a, b: i32) -> i32, i32 {
	sum := a + b
	prod := a * b
	
	return sum, prod
}
```