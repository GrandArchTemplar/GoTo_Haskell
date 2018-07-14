## λ calculus

### Exercize 1
Find value 
```
(λx.🥕)🍋 = ?
(λx.x)🥕 = ?
(λ🥕🍋.🥕)🍋 = ? 
(λx.λy.x)(λx.x) = ?
```

### Exercize 2
Find value
```
(λx.λy.λz.z(z(y))(λx.λy.λz.x(y(z))
```

### Exercize 3
```
let f = λs.λz.s(s(z))
let m = λx.λy.λs.λz.x(y(s))z
let g = m f f
```
Find

g in λ-evaluation

### Exercize 4
```
let f = λs.λz.s(s(s(s(z))))
let g = λs.λz.s(s(s(z))
let p = λx.λy.λs.λz.xysz
```

### Exercize 5
```
let t = λt.λf.t
let f = λt.λf.f
let o = λa.λb.?r
let a = λa.λb.?n

o f f = f | a f f = f
o f t = t | a f t = f
o t f = t | a t f = f
o t t = t | a t t = t
```
Find ?r and ?n 

## Haskell

### Implement:

```haskell
double :: String -> String
-- double :: Vec n Char -> Vec (2*n) Char
-- double "xx" = "xxxx"

mow :: String
-- mow = "mow"
```

---

A DNA nucleobase type, an enumeration of Adenine, Cytosine, Guanine and Thymine, and a function to get a complementary nucleobase.

```haskell
data DNAN = ...

complementary :: DNAN -> DNAN
```

---

Walk through:

- `Course.ExactlyOne`
- `Course.Validation`
- `Course.Optional`

from data61/fp-course.
