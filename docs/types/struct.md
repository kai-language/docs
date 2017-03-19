# Structs

## Declaration

```swift
Person :: struct {
	name: string
	age: i8
}
```

## Initialisation

```swift
me: Person = {
	name = "Glenn",
	age = 30
}
```

## Default Values

```swift
Car :: struct {
	model: string
	maker: string
	wheels: i8 = 4
}

modelS: Car = {
	model = "Model S"
	maker = "Tesla"
}
```