## Разделяй и властвуй

### Сервер: КМБ-1 edition
```
1. Сделать однопоточный сервер и клиент. С следующим алгоритмом действий:
  1.1 Клиент подключается к серверу.
  1.2 Сервер посылает константу "hello" 
  1.3 Клиент выводит эту константу(она может поменяться) на экран
  1.4 Клиент и сервер выключаются
2. То же самое, что и пункт один, но сообщение повторяется каждые 0.5 секунд и клиент соответственно выводит его каждые 0.5 секунд
3. Клиент подключается к серверу, говорит своё name и сервер говорит "Hello, %name"
4. К серверу одновременно может подключиться одновременно > 1 клиента
```
### Сервер: КМБ-(1-2) edition 
Ваш уровень КМБ равен 1 + k * 0.5, где k -- количество задач решённых ниже
```
1. broadcast server: посылка и монитор broadcast сообщений
2. общий state между клиентами
```
### Our future: 
Проблематика: 
мы проводим квест и командам нужно находить спрятанные предметы(геокеши) и это коллаборативная игра и данными нужно обмениваться: знание о некоторых предметах дают следующие подсказки, когда команды пробегают мимо

формальное условие:
написать на сокетах и CRDT GSet сервер, который умеет показывать текущий список кешей, добавлять новый кеш и синхронизироваться с другим сервером 
```
newtype Coord = (Float, Float)
get :: [Coord]
add :: Coord -> [Coord]
syn :: Server -> [Coord]
```
### Задача для нормальных посанов
Есть карта. На ней есть ил

Илососы сосут ил

Карта nxn(матрица)

Илососы видят на 1 вокруг себя

Илососы могут передавать информацию о разведанных, если они в соседних клетках

Нужно высосать ВЕСЬ ил

!NB СДЕЛАТЬ ВСЁ В STACK!!!!!
