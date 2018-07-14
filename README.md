# GoTo_Haskell
GoTo Haskell Learn

Всем приветики! 

UPD: Домашки надо делать!
Появится третья оценка от них

### Время делать домашки (16.07.2018)
https://github.com/GrandArchTemplar/GoTo_Haskell/blob/master/HW/FirstDay.md
### Время делать домашки (17.07.2018)
https://github.com/GrandArchTemplar/GoTo_Haskell/blob/master/HW/SecondDay.md
### Время делать домашки (18.07.2018)
https://github.com/GrandArchTemplar/GoTo_Haskell/blob/master/HW/ThirdDay.md
### Время делать домашки (19.07.2018)
https://github.com/GrandArchTemplar/GoTo_Haskell/blob/master/HW/FourthDay.md

## Как писать код

Слева текстовый редактор (Sublime Text, VS Code, whatever), справа `ghci`. Написали код в редакторе, сохранили (C-S), подгрузили новое в `ghci` (`:reload`).

Маленькие штуки можно писать в просто одном файле и загружать его как `ghci a.hs` или `ghci` `:load a.hs`; для проектов следует использовать `stack`.

## Как писать data61/fp-course

1. Скачать из https://github.com/data61/fp-course; далее в директории:
2. Если дальше ошибка, `chmod go-w .ghci ./`
3. `ghci`: подгрузит весь код
4. Можно открывать конкретные модули в `src/Course/Module.hs` и смотреть!

Общая концепция: нужно открывать модули в [этом порядке](https://github.com/data61/fp-course#progression), читать, и реализовывать там функции.

В любой непонятной ситуации - `:type`.
