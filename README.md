## 1 Продолжение знакомства с jupyter notebook

### Лекция
- Эффективная работа в jupyter notebook
- Модуль Random
- Детали Dict и функций
- Генераторы
- list, set, dict comprehensions

1.1 Соедините два словаря в один

    ```
    dict1 = {'One': 1, 'Two': 2, 'Three': 3}
    dict2 = {'Four': 4, 'Five': 5, 'Six': 6}
    ```
    
1.2 Напишите функцию, которая на вход принимает два словаря и возвращает один объединенный словарь

2.1 Напишите функцию, которая из двух списков, делает один словарь, где элементы из первого списка - ключи, а элементы из второго списка - значения. Используя цикл for

    ```
    keys = ['One', 'Two', 'Three']
    values = [1, 2, 3]
    ```

2.2 Используя dict comprehensions

3.1 Извлеките только два ключа `name` и `age` из представленного словаря. Напишите функцию с циклом for.   

```python
client_dict = {
    "name": "John",
    "age": 25,
    "salary": 5000,
    "city": "Moscow"
}
```

3.2 Используя dict comprehensions

4.1 Сгенерируйте случайные целые числа от 0 до 100 в количестве 5 штук с помощью модуля random.
Зафиксируйте псевдогенерацию, чтобы сгенерированные значения всегда были одинаковые.
Используйте list comprehensions

4.2 Напишите генератор
Генератор на вход принимает список с данными о клиенте (данные из пункта 4.1). Внутри генератора реализуйте обход по списку с данными. На каждой итерации генератор будет возвращать кортеж из двух элементов:
* данные по клиенту (в зависимости от итерации, на 0 итерации вернется 0 элемент, на 1 итерации вернется 1 элемент и тд)
* целочисленное значение, которое показывает, сколько секунд прошло с предыдущей итерации.<br>
Примечание: секунды, которые возвращаются должны показывать время не с начала запуска генератора, а именно то время, которое прошло с предыдущей итерации. А значит время на первой итерации должно равняться 0.
Используйте функцию time из модуля time для подсчета времени.
Чтобы проверить работу таймера, запустите проход по генератору в цикле с time.sleep(2)

5.1 Найдите картинку в интернете и прикрепите её в ячейку с текстом

5.2 Создайте следующую таблицу в ячейке с текстом

<img src='https://cdn.playcaliber.com/site/media/news/2021/06/01/4-%D0%A2%D0%B0%D0%B1%D0%BB%D0%B8%D1%86%D0%B0-%D0%BC%D0%B0%D0%BB%D0%B5%D0%BD%D1%8C%D0%BA%D0%B0%D1%8F-%D0%BF%D0%BE-%D1%80%D0%B5%D0%B6%D0%B8%D0%BC%D0%B0%D0%BC-1280%D1%85853.jpg' width=500>

6. Напишите функцию, которая может принимать любое количество трат пользователя и считать сумму и среднее.
На вход поступают целочисленные значения в любом количестве
На выходе словарь с ключами суммы трат и средней траты


## 2 Анализ датасета с помощью Pandas

### Лекция

- Анализ табличных данных
- Статистики таблиц
- Фильтрация данных
- Сортировка данных
* Задание 1.

    Скачать данные по ссылке https://www.kaggle.com/datasets/ionaskel/laptop-prices.
    Считать данные с помощью pandas.
    Вывести на экран первые 5 строк.
    Посмотреть на описание признаков и на их содержание.
* Задание 2.

    Проведите первичный анализ данных.
    Изучите типы данных.
    Найдите количество пропущенных ячеек в данных.
    Посчитайте основные статистики по всем признакам и поизучайте их.
* Задание 3.

    Ответьте на несколько вопросов

    3.1 Ноутбуков от какой компании больше всего в наборе данных?

    3.2 Какая минимальная и максимальная стоимость у ноутбуков в данных?

    3.3 Какой самый дорогой ноутбук в данных?
* Задание 4.

    Ответьте на несколько вопросов

    4.1 Найдите ноутбуки с самой маленькой диагональю в данных?
    Выведите только следующие характеристики:

    1. Компания
    2. Тип ноутбука
    3. Диагональ
    4. Стоимость

    Если таких ноутбуков несколько, то выводите их всех

    4.2 Сколько стоит самый дорогой ноутбук у компании HP?

    4.3 Как много ноутбуков Ultrabook с 8GB RAM?
* Задание 5.
    
    5.1 Выберите ноутбук клиенту.
    Клиент хочет подобрать ноутбук с 8GB или 16GB ОЗУ на Windows 10 в стоимости до 500 евро, сколько у него вариантов?

    5.2 Выберите ноутбук клиенту.
    Клиент хочет подобрать ноутбук от MSI, с видеокартой Nvidia GeForce GTX 1050 Ti и главное не с диагональю 15.6. В какой ценовой категории вышли подобные ноутбуки?

    5.3 Что дешевле?
    В среднем дешевле ноутбуки с CPU Intel Core i7 7700HQ 2.8GHz или с Intel Core i7 7600U 2.8GHz?
* Задание 6.

    Найдите самый легкий ноутбук.
    Но обратите внимание на тип и представление данных в признаке Weight, если что, замените в строке 'kg' на пустую строку через метод .str.replace()



## 3 Изменение таблиц в Pandas

### Лекция

- Создание, изменение и удаление признаков
- Группировки данных
- Объединение таблиц
- Встроенные визуализации

* 1 задача

    Создание, изменение и удаление признаков. Группировки данных. Объединение таблиц. Встроенные визуализации

    1.1 Создать новый признак Cpu_Company, который будет содержать только название фирмы, которая произвела CPU

    1.2 Создать новый признак Memory_Amount, который будет содержать только количество Gb памяти без указания типа носителя

    1.3 Создать новый признак Memory_Type, который будет содержать только тип носителя (HDD/SDD/др.)

    1.4 Удалите признаки Memory и ScreenResolution

* 2 задача

    2.1 Создайте признак SSD, который изначально равен 0

    2.2 Поставьте в признаке SSD 1, если ноутбук действительно с типом носителя SSD

    2.3 Уберите в признаке Weight значения 'kg' и поменяйте его тип данных на вещественный

* 3 задача

    Создайте датафрейм с клиентами:

    ```
    clients = pd.DataFrame({
    'client_id': [45, 32, 67, 33, 43],
    'laptop_id': [506, 398, 710, 120, 1999]
    })
    ```
    3.1 Присоедините к таблице clients данные по ноутбукам через метод join

    3.2 Присоедините к таблице clients данные по ноутбукам через метод merge

* 4 задача

    Составьте несколько сводных таблиц

    4.1 Найдите среднюю стоимость ноутбуков в зависимости от компании производителя. Отсортируйте от меньшей стоимости к большей

    4.2 Найдите минимальную, среднюю и максимальную стоимости ноутбуков в зависимости от производителя процессора

    4.3 Постройте таблицу с подсчетом количества ноутбуков в данных в зависимости от производителя CPU и ОЗУ

    4.4 Постройте таблицу с подсчетом средней стоимости ноутбуков в данных в зависимости от операционной системы и GB памяти

* 5 задача*

    Ответьте на несколько вопросов

    5.1 Ноутбуков каких компаний и с каким процессором больше?

    5.2 С каким типом памяти и с каким объемом памяти больше ноутбуков?
