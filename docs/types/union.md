## Declaration

```swift
Career :: union {
	case engineer(field: string)
	case accountant(field: string, favouriteNumber: f64)
	case none
}
```

## Variable Declaration
```swift
myCareer: Career = .engineer(field: "Software")
```

## Comparison
```swift
myCareer: Career = .engineer(field: "Software")
herCareer: Career = .accountant(field: "General", favouriteNumber: 3.14)

print(myCareer == herCareer) // false
```

## Associated Values

```swift hl_lines="3"
hisCareer: Career = .engineer(field: "Civil")
if hisCareer = .engineer {
	print(hisCareer.field) // Civil
}
```