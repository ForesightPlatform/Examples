# Examples
Подборка примеров скриптов для решения различных задач на языке Fore.

## Оглавление
* [Регламентные отчеты](#Регламентные_отчеты)  
* [Расчеты](#Расчеты)  
* [Работа с отметками измерений](#Работа_с_отметками_измерений)  
* [Виртуальные кубы и составные измерения](#Виртуальные_кубы_и_составные_измерения)  
* [Работа с кэшем данных](#Работа_с_кэшем_данных)  
* [Особенности операций с матрицами](#Особенности_операций_с_матрицами)  
* [Измерения (справочники)](#Измерения_(справочники))  
* [Кубы](#Кубы)  
* [Загрузка и трансформация данных](#Загрузка_и_трансформация_данных)  

<a name="Регламентные_отчеты"></a>  
## __[Регламентные отчеты](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE)__ 
1.	Для подключения алгоритма расчета к срезу регламентного отчета [используется IEaxDataAreaExternalTransformation](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE/MOD_SETALGO_TOSLICE.text).  Передачу параметров из среза отчета в алгоритм можно настроить с помощью [обработчика событий](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE/MOD_REPORT_EVENTHANDLER_SETALGOPARAMS.text)

2.	Примеры вставки картинки на лист регламентного отчета в качестве [гиперссылки](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE/MOD_IMAGE_AS_HYPERLINK.text) или [экспандера](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE/MOD_IMAGE_AS_EXPANDER.text)

3.	Для реляционного источника в регламентном отчете можно [настроить пагинацию](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_REPORTS_EXAMPLE/MOD_REPORT_EVENTHANDLER_PAGES.text)

<a name="Расчеты"></a>  
## __[Расчеты](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_CALC_EXAMPLE)__ 

1.	Пример [запуска расчёта алгоритма](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CALC_EXAMPLE/MOD_CALC_ALGO.text) из кода с передачей параметров

2.	Для получения информации о формуле, по которой считалась конкретная точка приемника, используется [метод GetFormulaInfo](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CALC_EXAMPLE/MOD_GETFORMULAINFO.text)


<a name="Работа_с_отметками_измерений"></a>  
## __[Работа с отметками измерений](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_SELECTION_EXAMPLE)__  

1.	Если в кубе настроено управление измерениями (одно измерение куба перестраивается в зависимости от отметки в другом), то для построения коллекции отметок (SelectionSet-a) для такого куба нужно [учитывать отметки в управляющих измерениях](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_SELECTION_EXAMPLE/MOD_SELSET_CONTROL.text)

2.	Пример [установки схемы отметки в пивот](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_SELECTION_EXAMPLE/MOD_SETPIVOTSELECTION.text)

3.	Для работы с отметкой календарного справочника можно [использовать IDimCalendarSelection](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_SELECTION_EXAMPLE/MOD_CALENDARSCHEMA.text)


<a name="Виртуальные_кубы_и_составные_измерения"></a>  
## __[Виртуальные кубы и составные измерения](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE)__ 

1.	По умолчанию в виртуальном кубе для измерения фактов используется составной справочник (ICompoundDimension), он «собирает» факты на основе декарта частных измерений. Если нужен не декарт, а конкретные элементы, то можно [переключиться на конструируемое измерение](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_CUSTOMCONTAINER.text). 
В конструируемое измерение можно добавлять [атрибуты](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_ADDATTR_TO_CUSTOMDIM.text) и [элементы](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_ADDELEMENT_TO_CUSTOMDIM.text).

2.	Частные измерения виртуального куба можно [выносить в общие](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_FORCEDCOMMONDIM.text), [джойнить по заданному индексу](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_JOIN_DIMS.text), чтобы перенести из частных, [расширять отметку](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_VIRTCUBES_EXAMPLE/MOD_ADDSELECTION.text)

<a name="Работа_с_кэшем_данных"></a>  
## __[Работа с кэшем данных](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_CACHE_EXAMPLE)__ 

1.	Кэш [можно делать локальным (для одного пользователя) или глобальным (для всех пользователей)](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CACHE_EXAMPLE/MOD_GLOBALMATRIX.text)

2.	Из кода можно [работать с отдельными элементами кэша](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CACHE_EXAMPLE/MOD_CACHE_ELEMENTS.text) и [«прогревать» кэш](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CACHE_EXAMPLE/MOD_GETCACHE.text)

<a name="Особенности_операций_с_матрицами"></a>  
## __[Особенности операций с матрицами](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_MATRIX_EXAMPLE)__ 
1.	Для быстрых операций над матрицами (сложение, умножение и т.д.) можно использовать [свойство OperationMatrix](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_MATRIX_EXAMPLE/MOD_MATRIX_APPEND.text)

2.	Использование [запросов к матрицам ](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_MATRIX_EXAMPLE/MOD_MATRIXQUERY.text) значительно ускоряет проход по ним

<a name="Измерения_(справочники)"></a>  
## __[Измерения (справочники)](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_DIMENSIONS_EXAMPLE)__ 

1.	Составное измерение можно [создавать](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_DIMENSIONS_EXAMPLE/MOD_CREATE_COMPOUND_DIM.text) и [использовать](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_DIMENSIONS_EXAMPLE/MOD_OPEN_COMPOUND_DIM.text) вне виртуального куба

2.	Можно настроить пользовательский календарь, [сделав календарным](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_DIMENSIONS_EXAMPLE/MOD_DIM_AS_CALENDAR.text) подходящий справочник

3.	В справочниках НСИ есть возможность создавать не только обычные вычисляемые атрибуты, но и [атрибуты на запросах](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_DIMENSIONS_EXAMPLE/MOD_CREATE_CALC_ATTR.text)

<a name="Кубы"></a>  
## __[Кубы](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_CUBES_EXANPLE)__ 
1.	Автокуб на другом кубе [можно создать без репозитория НСИ](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CUBES_EXANPLE/MOD_CREATE_AUTOCUBE.text) из кода

2.	Стандартный куб поддерживает возможность подключения коллбэков [на запрос данных](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CUBES_EXANPLE/MOD_DATASET_SQL_CALLBACK.text)  (от редактирования до полной подмены SQL-запроса) и коллбэков на [сохранение данных](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_CUBES_EXANPLE/MOD_SAVECUBE_CALLBACK.text), где можно редактировать сохраняемые матрицы

<a name="Загрузка_и_трансформация_данных"></a>  
## __[Загрузка и трансформация данных](https://github.com/ForesightPlatform/Examples/tree/main/FLD_EXAMPLE_MOD/FLD_ETL_EXAMPLE)__ 
1.	Аналитическая платформа Форсайт позволяет посылать HTTP-запросы к различным веб-сервисам и интегрироваться со специализированными службами, например, с [брокером сообщений RabbitMQ](https://github.com/ForesightPlatform/Examples/blob/main/FLD_EXAMPLE_MOD/FLD_ETL_EXAMPLE/MOD_RABBITMQ_HTTP.text)


***
<!-- Лого  -->
<img src="https://www.fsight.ru/wp-content/uploads/2021/05/fs.png" alt="drawing" width="200"/>
