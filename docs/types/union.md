## Declaration

```swift
Data :: union {
	i: i64,
	f: f64,
	s: string
}
```

```swift
data := Data
data.f = 3.14159
printf("data.f: %f\n".raw, data.f)
printf("data.i: %d\n".raw, data.i)
printf("data.s: %s\n".raw, data.s)
```


```swift
data := Data

data.i = 100
printf("data.i: %d\n".raw, data.i)

data.f = 3.14159
printf("data.f: %f\n".raw, data.f)

data.s = "Unions!"
printf("data.s: %s\n".raw, data.s)
```