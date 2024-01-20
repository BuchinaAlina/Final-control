# Итоговая контрольная работа
## Задача:
Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

**Примеры:**

[“Hello”, “2”, “world”, “:-)”] → [“2”, “:-)”]

[“1234”, “1567”, “-2”, “computer science”] → [“-2”]

[“Russia”, “Denmark”, “Kazan”] → []

## Решение:

1. Составить алгоритм решения задачи.
2. Нарисовать блок-схему алгоритма.
3. Написать программу, решающую поставленную задачу.

## Алгоритм:
1. Начало.

2. Создайте исходный массив.

3. Определите размер исходного массива.

4. Создайте новый массив, чтобы хранить элементы длиной меньше или равной 3 символам.

5. Установите счетчик для нового массива в 0.

6. Пройдитесь по каждому элементу исходного массива.

7. Для каждого элемента в исходном массиве проверьте его длину.

8. Если длина текущего элемента меньше или равна 3 символам, то добавьте этот элемент в новый массив и увеличьте счетчик на 1.

9. Вывод нового массива.

10. Конец.

## Блок-схема:
![Блок-схема]("C:\Users\пользователь\Desktop\2024-01-20_15-38-11.png")


## Программа:

1. Ввод массива с клавиатуры:

Здесь программа запрашивает у пользователя ввод элементов массива, разделенных пробелом, с клавиатуры. Эти элементы сохраняются в массив inputArray.

2. Формирование нового массива:

Вызывается метод FilterArrayByLength, который фильтрует массив inputArray по длине строк. Результат сохраняется в массиве resultArray.

3. Метод FilterArrayByLength:

Этот метод принимает в качестве аргументов входной массив строк inputArray и максимальную длину строки maxLength. Он сначала вычисляет количество строк, которые удовлетворяют условию (длина меньше или равна maxLength). Затем создается новый массив resultArray нужного размера, и в него копируются строки из inputArray, удовлетворяющие условию.

4. Вывод нового массива:

Новый массив resultArray выводится на экран с использованием Console.WriteLine, а string.Join используется для объединения элементов массива в строку с пробелами между ними.

Эта программа фактически фильтрует строки в массиве по их длине и выводит новый массив на экран.

Для запуска программы введите команду через терминал:

dotnet run 

Далее введите значения через пробел, например:

Введите значения через пробел: 276 hello sun 333 world

Вывод нового массива: 276 sun 333