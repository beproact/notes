### Function Definitions
```haskell
name arg1 arg2 = <expr>
```


### Types
```haskell
name :: type
```
Integer, Bool Float

```haskell
in_range :: Integer -> Integer -> Integer -> Bool
```
### Recursion

Guards
```haskell
fac n
| n<= 1  = 1
| otherwise = n * fac (n-1)
```

Pattern Matching
```haskell
is_zero 0 = True
is_zero _ = False
```
_ is a wildcard

#### Higher Order Functions
Functions that take a function as an argument
```haskell
app :: (a->b) -> a -> b
app f x = f x
```

Anonymous Functions
```haskell
--(\<args> -> \<expr>)
add3 = (\x y z -> x+y+z)
```

Map
```haskell
map :: (a -> b) -> [a] -> [b] -- Applies function to all of a
filter :: (a -> Bool) -> [a] -> [a] -- Leaves only elements of a that return true
```

### Currying
We can rewrite any multiple argument function as a function that only has one argument and returns a function
```haskell
f::a -> b -> c -> d
f::a -> (b -> (c -> d))
```

##### Partial Function Application
``` haskell
add :: Int -> Int -> Int
add 1 :: Int -> Int
```
add 1 effectively returns a function where (add 1)

```haskell
map :: (a -> b) -> [a] -> [b]
doubleList = map (\x -> 2*x)
```

### Composition
``` haskell
(.) :: (b -> c) -> (a -> b) -> a -> c -- 
-- (f . g) is equivalent to (\x -> f (g x))
descSort = reverse . sort
map2D :: (a -> b) -> [[a]] -> [[b]]
map2D = map . map
($) :: (a -> b) -> a -> b
```

### Folding
``` haskell
foldr :: (a -> b -> b) -> b -> [a] -> b
```