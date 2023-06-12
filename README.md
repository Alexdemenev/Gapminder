# Проект Gapminder

Предсказание дохода по фото.

**Основные этапы проекта**

* Выгрузка данных
* Построение baseline (первоначальная модель)
* Улучшение модели
* Интерпретация

### Выгрузка данных

Парсер, извлекающий фото в формате матриц numpy, расположен [здесь](parser.ipynb)

Источник данных - [Dollar-Street](https://www.gapminder.org/dollar-street)

**Описание процесса**

Данные извлекаются циклично в соответствии с выбранными темами. 

В pd.DataFrame сохраняются следующие переменные: доход, страна, регион, ссылка на фото, тема.

Далее фото преобразовываются в формат np.array и сохраняются. Доход распределяется по квартилям и сохраняется в виде категорий.
