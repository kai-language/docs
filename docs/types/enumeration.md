## Declaration

```swift
Direction :: enum {
	case up
	case down
	case left
	case right
}
```

## Variable Declaration
```swift
direction: Direction = .up
```

## Control Flow
```swift
direction: Direction = .down

switch direction {
case .up
    print("up")

case .down
	print("down")

case .left
	print("left")

case .right
	print("right")
}
```

!!! note
	Learn more about `Control Flow` [here](/control-flow/).