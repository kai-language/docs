## Import a File

```swift
#import "strings.kai"
```

## Import from Git

```swift
// github
#import git("author/repo")

// external
#import git("https://external.com/author/repo")
```

## Alias an Import

```swift
#import "math" mathy
print(mathy.pi)
```

## Import a C Header

```swift
#import "stdio.h"
```

!!! note
	Learn more about `Working with C` [here](/c).

## Pre-Compiled Library

```swift
// include and link against glibc
#library "/path/to/umbrella.h" glibc
```
