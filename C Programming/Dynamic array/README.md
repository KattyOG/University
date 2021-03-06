### Цель работы
1. Научиться работать с одномерными динамическими массивами, использовать функции стандартной библиотеки malloc, calloc, realloc, free.
2. Научиться создавать сценарии make для многофайловых проектов.
3. Закрепить навык создания модульных тестов.
#### Общее задание:
Принять с клавиатуры положительное целое n и последовательность n действительных
чисел, которые следует записать в динамический массив A.
Вычислить в соответствии с вариантом число μ1 = μ1(A).
Получить массив A1 , удалив в соответствии с вариантом из динамического массива A
набор элементов по признаку. Обратите внимание: даже если на этом шаге несколько раз
используется уже вычисленное μ1 , то оно не вычисляется заново. Если массив A 1 сформировать невозможно, или он формируется пустым, считать ситуацию исключительной.
Вычислить в соответствии с вариантом число μ2 = μ2 (A1).
Получив с клавиатуры номер позиции p, сформировать массив A2 , вставив с сохра-
нением порядка сначала на позицию p массива A1 , а затем добавив в начало и в конец
число μ2 . Обратите внимание: даже если на этом шаге используется несколько раз уже
вычисленное μ2 , то оно не вычисляется заново. Если на момент вставки на позицию p в
массиве меньше, чем p + 1 элементов, считать ситуацию исключительной.
Распечатать на экран массив A2 .
#### Примечания
1. В методических целях при обработке массивов запрещается использовать квадратные скобки. Длину массива разрешается использовать только в функциях работы с
памятью.
2. Принять, что под корнем из числа подразумевается арифметический корень из числа.
3. Принять, что под вводом и выводом массива подразумеваются «классические», насколько тут уместно это слово, ввод и вывод элементов массива в строку.
4. Использовать при решении числа двойной точности. Переполнение не контролировать.
5. Для каждой структуры данных в первую очередь реализовать набор подпрограмм
группы CDIO — подпрограммы создания, удаления, ввода и вывода.
6. Вынести подпрограммы для каждой структуры данных в отдельный модуль.
7. Следовать правилу Тараса Бульбы для памяти: «Если в подпрограмме есть запрос
динамической памяти, то либо в ней же должно осуществляться освобождение памяти, либо в имени подпрограммы должно быть указание для программиста на наличие
запроса памяти внутри подпрограммы.» В качестве указаний, например, можно использовать слова и словосочетания: «allocate», «create», «set length», «new» и другие.
#### Вариант вычисления μ1:
<img src="https://github.com/KattyOG/University/blob/master/C%20Programming/Dynamic%20array/XiXblzjIJ_8.jpg"> 

#### Вариант удаления:
Удалить из массива A два элемента, имеющих максимальную разницу с заранее вычисленным числом μ 1 = μ 1 (A).
Если обнаружены одинаковые кандидаты на удаление, удалять в порядке следования. 

#### Вариант вычисления μ2:
μ2(x) = max(x);
