Я тут подумал, что зачем мне писать статью, если это сделал уже кто-то другой. Вот вам ссылка - https://www.youtube.com/watch?v=tCYEr1uPQmg
а я пошел. Пока!

.

.


.


.

.


.

.
.
.


.
.
.
.

.
.
.
.
.
.
.
.
.
.

.
.


.



.

.

.

.


.

.


.


.

.

.

Ладно, это была шутка.

![Alt-текст](https://w7.pngwing.com/pngs/353/1022/png-transparent-el-risitas-graphy-laughter-laugh-miscellaneous-microphone-photography.png "Орк")

# Алгоритм сортировки массива простым включением

Массив:
5 -4 0 3 2

n=0

SIZE - Размер массива


Алгоритм:

1. Выбираем наименьший элемент с ячейки >=n и меняем местами с n-ной ячейкой.

5 [-4] 0 3 2

{-4} 5 0 3 2

2. Увеличиваем n на один: n=n+1

3. Переходим на 1-ый пункт, пока n<SIZE-1.


Визуальный пример:                                

{-4} 5 [0] 3 2

{-4} 0 5 3 2

{-4} {0} 5 3 [2]

{-4} {0} 2 3 5

{-4} {0} {2} 3 5

{-4} {0} {2} [3] 5

{-4} {0} {2} {3} 5

Результат:
-4 0 2 3 5


# Алгоритм сортировки массива простым выбором
 
Массив:
-1 0 -4 3 2

max - Индекс максимального числа

N=5 - Размер массива

Алгоритм:

1. i=0, max=0. 
Идем по массиву пока i<N. То есть Сравниваем i-тый элемент с max. Если arr[i]>arr[max], то max=i. 

[-1] 0 -4 3 2: i=0, max=0

-1 [0] -4 3 2: i=1, max=0

-1 [0] -4 3 2: i=1, max=1

-1 0 [-4] 3 2: i=2, max=1

-1 0 -4 [3] 2: i=3, max=1

-1 0 -4 [3] 2: i=3, max=3

-1 0 -4 3 [2]: i=4, max=3

2. Дальше меняем местами max и N-1

-1 0 -4 3 2

-1 0 -4 2 3

3. Уменьшаем N на единицу: N=N-1
4. Переходим на 1-ый пункт пока N>0

Визуальный пример:

[-1] 0 -4 2 {3}: i=0, max=0

-1 [0] -4 2 {3}: i=1, max=0

-1 [0] -4 2 {3}: i=1, max=1

-1 0 [-4] 2 {3}: i=2, max=1

-1 0 -4 [2] {3}: i=3, max=1

-1 0 -4 [2] {3}: i=3, max=3

-1 0 -4 2 {3}

-1 0 -4 2 {3}

[-1] 0 -4 {2} {3}: i=0, max=0

-1 [0] -4 {2} {3}: i=1, max=0

-1 [0] -4 {2} {3}: i=1, max=1

-1 0 [-4] {2} {3}: i=2, max=1

-1 0 -4 {2} {3}

-1 -4 0 {2} {3}

[-1] -4 {0} {2} {3}: i=0, max=0

-1 [-4] {0} {2} {3}: i=1, max=0

-1 -4 {0} {2} {3}

-4 -1 {0} {2} {3}

Результат:
-4 -1 0 2 3

# Алгоритм сортировки массива "пузырьком"

Массив:
5 -4 0 3 2


N - Размер массива

Алгоритм:

1. i=0, j=1.
Сравниваем i-тый и j-тый элемент. 

[5] [-4] 0 3 2

Если arr[i]>arr[j], то меняем элементы местами

5 -4 0 3 2

-4 5 0 3 2

2. Увеличиваем i и j на единицу и переходим на 1-ый пункт, пока j<N: i=i+1, j=j+1

Визуальный пример:

-4 [5] [0] 3 2

-4 5 0 3 2

-4 0 5 3 2

-4 0 [5] [3] 2

-4 0 5 3 2

-4 0 3 5 2

-4 0 3 [5] [2]

-4 0 3 5 2

-4 0 3 2 5

-4 0 3 2 {5}

3. Дальше уменьшаем N на единицу и переходим на 1-ый пункт, пока N>0: N=N+1

Визуальный пример:

[-4] [0] 3 2 {5}

-4 [0] [3] 2 {5}

-4 0 [3] [2] {5}

-4 0 3 2 {5}

-4 0 2 3 {5}

-4 0 2 {3} {5}

[-4] [0] 2 {3} {5}

-4 [0] [2] {3} {5}

-4 0 {2} {3} {5}\

[-4] [0] {2} {3} {5}

-4 {0} {2} {3} {5}

Рузультат: -4 0 2 3 5



# На этом всё!

Спасибо за внимание.

Я постарался максимально кратко и без лишних слов объяснить алгоритмы. Сразу извиняюсь за оформление. Оно не идиально, да. Но думаю более чем понятно. Просто нет времени с оформлением возиться XD

Всем добра.
