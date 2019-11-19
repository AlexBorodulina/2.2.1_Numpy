# Работа с массивом `numpy`

## Задания

В задании требутеся решить все подзадачи. Они должны быть реализованы в виде функции в файле `main.py`. Далее приведён список требуемых функции.

### `t1_file_stat`

Считайте из файла массив действительных чисел (числа записаны в виде столбца). Найдите для этого массива среднее, максимальное и минимальное значения, среднеквадратичное отклонение и пятый центральный момент.

+ Функция принимает аргумент `filename` - имя файла, в котором лежит массив.
+ Функция должна возвращать словарь, где по соответствующим ключам лежат нужные значения:
  + `mean` - среднее значение,
  + `max` - максимальное значение,
  + `min` - минимальное значение,
  + `std_dev` - [среднеквадратичное отклонение](https://ru.wikipedia.org/wiki/%D0%A1%D1%80%D0%B5%D0%B4%D0%BD%D0%B5%D0%BA%D0%B2%D0%B0%D0%B4%D1%80%D0%B0%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%B5_%D0%BE%D1%82%D0%BA%D0%BB%D0%BE%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5),
  + `5th_central_moment` - пятый [центральный момент](https://ru.wikipedia.org/wiki/%D0%9C%D0%BE%D0%BC%D0%B5%D0%BD%D1%82%D1%8B_%D1%81%D0%BB%D1%83%D1%87%D0%B0%D0%B9%D0%BD%D0%BE%D0%B9_%D0%B2%D0%B5%D0%BB%D0%B8%D1%87%D0%B8%D0%BD%D1%8B).

### `t2_sort_int`

Отсортируйте массив целых чисел по возрастанию.

+ Функция принимает аргумент `array` - массив `numpy` с целыми числами.
+ Функция должна вернуть отсортированный массив `numpy` (не важно, исходный или новый).

### `f3_sort_complex`

Отсортируйте массив комплексных чисел *а)* по модулю *б)* по убыванию действительной части.

+ Функция принимает аргумент `complex_array` - массив `numpy` с комплексными числами.
+ Функция должна вернуть кортеж с двумя отсортированными массивами `numpy` (стабильность сортировки не требуется).

### `f4_sort_string_len`

Отсортируйте список строк по длине строки.

+ Функция принимает аргумент `string_array` - массив `numpy` со строками.
+ Функция должна вернуть отсортированный массив `numpy` (стабильность сортировки не требуется).

### `f5_sort_string`

Отсортируйте кортеж строк в [лексикографическом порядке](https://ru.wikipedia.org/wiki/%D0%9B%D0%B5%D0%BA%D1%81%D0%B8%D0%BA%D0%BE%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%BF%D0%BE%D1%80%D1%8F%D0%B4%D0%BE%D0%BA) (тот порядок, в котором строки сортируются в питоне по-умолчанию).

+ Функция принимает аргумент `string_tuple` - кортеж со строками.
+ Функция должна вернуть отсортированный кортеж строк.
+ Можно не использовать `numpy`.

## Тестирование

Для тестирования нужны пакеты `pytest` и `numpy`.

```bash
pip install -r requirements.txt
```

Запустить тесты можно так:

```bash
python -m pytest -sv
```
