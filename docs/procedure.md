```swift
sum :: (a: i32, b: i32) -> i32 {
	return a + b
}
```

```swift
mul :: (a, b: i32) -> i32 {
	return a * b
}
```

```swift
sumAndMul :: (a, b: i32) -> i32, i32 {
	sum := a + b
	prod := a * b
	
	return sum, prod
}
```