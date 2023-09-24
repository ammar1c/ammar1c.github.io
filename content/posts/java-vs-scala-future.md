+++
title = 'Async processing in Java vs Scala'
date = 2023-09-23T21:55:42+02:00
draft = true
+++


transforming a future in scala:
```scala
val f = Future(1).map(x => x+1)
```
in java:
```java
var x = CompletableFuture.completedFuture(1);
x.thenApply(y -> y+1);
```

