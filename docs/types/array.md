# Arrays

```swift
names := [3]string { "Tim", "Søren", "Jane" }
namesCopy := names
```

```swift
print(names.length) // 3
print(names[0]) // "Tim"
```

# Dynamic Arrays

```swift
names := []string
names = append(names, "James")
print(names[0]) // "James"
```