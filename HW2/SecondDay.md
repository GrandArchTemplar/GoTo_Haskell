## λ-исчисление вечно

```
(λx.λx.λx.x) (λx.λx.λx.xx) (λx.λx.λx.xx) (λx.λx.λx.xx) (λx.λx.λx.λx.xx) = ?
(λxyz.xy)(λxyz.yx)(λx.x)(λx.x)(λx.x) = ?
```

## Сворачиваемся!

### Бесконечные максимальные работы
```
unlimitedMaxWorks :: [Integer] -> Integer
unlimitedMaxWorks [1,2, 1000000, 4, 5] = 1000000
```

### Разница взглядов
```
f a b = a * 10 + b * 2 - 7 `div` a

посмотреть на разницу между
foldr f 0 [1..10] и foldl f 0 [1..10]
```

### Делимся!
Реализовать via foldr
```
ghci> splitOn '/' "path/to/file"
["path", "to", "file"]
```

### Соединяемся!
Реализовать via foldr
```
ghci> joinWith '/' ["path", "to", "file"]
"path/to/file"

LAW : splitOn x . joinWith x = x
```


## М-м-м-моноиды
### Возможная связка
Реализуйте ф-цию
```
maybeConcat :: [Maybe [a]] -> [a]
ghci> maybeConcat [Just [1,2,3], Nothing, Just [4,5]]
[1,2,3,4,5]
```

### Эндом-м-м-м-морфизмы
newtype Endo a = Endo { getEndo :: a -> a }
реализовать следующее:
```
mempty' :: Endo a 
mappend' :: Endo a -> Endo a -> Endo a
```

## Компьютерная грамотность

### Вы мои джигиты

1. разобраться как установить git
2. сделать репу в гитхабе/гитлабе/любой другой git системе

### Stack воспрянет из могилы
1. поставить стек
2. создать проект с темплейтов отсюда: https://raw.githubusercontent.com/GrandArchTemplar/stack-templates/master/academic.hsfiles(сделать так чтобы он появился на вашем гитлабе/гитхабе/любой другой системе связанной с git)
3. реализовать в main вызов функции fib
```
fib :: Integer -> [Integer]
fib n -- функция которая возвращает список чисел фиббоначи от 1 до n
```

### Stack -- наше всё!
https://github.com/commercialhaskell/hindent
Соберите этот или какой-либо другой равный или выше по рангу проект

Сделайте так чтобы оно работало
Если выбрали `hindent`, то проверьте его работоспособность на вашем файле с домаш-ш-ш-ш-шкой


### Теория это важно!

Быть готовым ответить что делают следующие команды и какова их семантика
```
stack new
stack install
stack build
stack exec
stack repl
stack upgrade
stack update
```
