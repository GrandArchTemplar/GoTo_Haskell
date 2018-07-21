# Test!

### Task 1

```
(λx.λy.x(x(y))) (+1) 5 = ?
```

### Task 2
```
(λf.λx.λy.fyx)(-) 1 2
```

### Task 3
```
(λx.λx.x)(λx.xx)(λx.x)
```

### Task 4
```
f :: (a -> b) -> Maybe a -> Maybe b
f (+1) (Just 5) = Just 6
f length (Just "xx") = Just 2
f (\x -> x + x * x `div` x + x ^ x) Nothing = Nothing
```

### Task 5
Написать функцию факториала
```
faque :: Int -> Int
faque 5 = 120
faque 4 = 24
faque 0 = 1
```
