# Structs

## Declaration

```swift
Person :: struct {
	name: string
	age: u8
}
```

## Initialization

```swift
me := Person {
	"Glenn",
	30
}
```

Struct initialization can be with or without argument labels. If the labels are provided, the fields can be declared in any order. For example:

```swift
me := Person {
	age: 24,
	name: "Brett"
}
```