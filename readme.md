![GitHub watchers](https://img.shields.io/github/watchers/immelstorun/primitive_num_predictor?label=watchers&logo=GitHub&logoColor=yellow&color=yellow)
![TG profile](https://img.shields.io/badge/my_telegram-blue?logo=telegram&logoColor=yellow)
![Python ver](https://img.shields.io/badge/python-3.10.9-blue)

# Проект "Быстрый предиктор чисел"
Дя начала запусти **RUN_ME.ipynb**

## Оглавление
[1. Описание проекта](#описание-проекта)

[2. Описание данных](#описание-данных)

[3. Этапы](#этапы )

[4. Результаты](#результаты)

[5. Выводы](#выводы)

### Описание проекта
Алгоритм генерирует целое число от 1 до 100. 

Необходимо реализовать второй алгоритм, который будет за минимальное количество попыток определять сгенерированное число. 

Максимально допустимое количество попыток - 20. 

Качество созданного алгоритма нужно сравнить с двумя алгоритмами, данными в baseline.

**Метрика качества:**
Результаты оцениваются по среднему количеству попыток при 1000 повторений.

**Критерии оценивания**
| Бал  | Критерий  | Отметка |
|:------------- |:---------------| :-------------|
| 1 | Программа находит число меньше чем за 20 попыток. Если данное условие не выполняется, выставляется 0 баллов за это и все остальные условия.        | ✔        |
| 2 | Код решения загружен на GitHub        | ✔        |
| 3 | GitHub оформлен соответствующим образом       | ✔        |
| 4 | Код соответствует стандарту PEP8  | ✔        |
| 5 | Код воспроизводим: зафиксированы версии библиотек в виде файла requirements.txt или иного формата файлов конфигураций  | ✔        |

### Описание данных
Все данные генерируются случайно. random seed = 42

### Этапы
| Этап | Описание  | Отметка |
|:------------- |:---------------| :-------------|
| 1 | Написать алгоритм предсказания | ✔        |
| 2 | Провести Рэнкинг с бейзлановыми алгоритмами | ✔        |
| 3 | Зафиксировать версии использованных библиотек и окружения| ✔        |
| 4 | Сделать визуал для представления результатов| ✔        |






### Результаты
Был написан алгоритм бинарного поиска. Все три алгоритма и функция рэнкинга были помещены в файл **predictors.py**, который импортируется в начале выполнения основного ноутбука **RUN_ME.ipynb**
Лучший результат показал алгоритм бинарного поиска. В среднем он находит ответ за 6-7 попыток
Для лучшей визуализации построена диаграмма. Ее код вызывается из отдельного файла **plotter.py**

Для воспроизводимости окружение и библиотеки зафиксированы в файлах
* requrements.txt
* environment.yml

### Выводы

Было проведено исследование по производительности трех алгоритмов поиска загаданного числа: простого поиска, поиска большего или меньшего и бинарного поиска.

В ходе исследования мы нашли, что бинарный поиск является самым быстрым алгоритмом. Бинарный поиск является мощным алгоритмом, широко используемым в различных областях, включая информатику и структуры данных. Он особенно полезен при работе с отсортированными данными или при поиске конкретного значения в большом наборе данных.

Причина, по которой бинарный поиск быстрый, заключается в том, что он уменьшает объем поиска вдвое при каждом шаге. Эта особенность делает его более эффективным по сравнению с другими алгоритмами, такими как простой поиск, который проверяет все элементы в наборе данных, и поиск большего или меньшего, который проверяет элементы по одному до тех пор, пока не будет найдено желаемое число.

[К оглавлению](#оглавление)
