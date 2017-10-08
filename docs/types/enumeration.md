## Declaration

```swift
Direction :: enum {
	up,
	down,
	left,
	right
}
```

## Variable Declaration
```swift
direction := Direction.up
```

## Control Flow
```swift
direction := Direction.down

switch direction {
case Direction.up
    print("up")

case Direction.down
	print("down")

case Direction.left
	print("left")

case Direction.right
	print("right")
}
```

!!! note
	Learn more about `Control Flow` [here](/control-flow/).

## Associated values
```swift
Mode :: enum(u8) {
	indirect = 1,
	relative,
	absolute
}
```