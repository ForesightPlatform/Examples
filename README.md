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
* [Работа с перменной типа blob](#Работа_с_перменной_типа_blob)  

<a name="Регламентные_отчеты"></a>  
## __[Регламентные отчеты](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B)__ 
1.	Для подключения алгоритма расчета к срезу регламентного отчета [используется IEaxDataAreaExternalTransformation](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B/01.1.%20%D0%9F%D0%BE%D0%B4%D0%BA%D0%BB%D1%8E%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC%D0%BE%D0%B2%20%D0%BA%20%D1%81%D1%80%D0%B5%D0%B7%D1%83.text).  Передачу параметров из среза отчета в алгоритм можно настроить с помощью [обработчика событий](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B/01.2.%20%D0%9E%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%87%D0%B8%D0%BA%20%D1%81%D0%BE%D0%B1%D1%8B%D1%82%D0%B8%D0%B9%20(%D0%BF%D1%80%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%B8%D1%82%D1%8C%20%D0%BF%D0%B0%D1%80%D0%B0%D0%BC%D0%B5%D1%82%D1%80%D1%8B).text)

2.	Примеры вставки картинки на лист регламентного отчета в качестве [гиперссылки](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B/02.%20%D0%92%D1%81%D1%82%D0%B0%D0%B2%D0%BA%D0%B0%20%D0%BA%D0%B0%D1%80%D1%82%D0%B8%D0%BD%D0%BA%D0%B8%20%D0%BA%D0%B0%D0%BA%20%D0%B3%D0%B8%D0%BF%D0%B5%D1%80%D1%81%D1%81%D1%8B%D0%BB%D0%BA%D0%B8.text) или [экспандера](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B/03.%20%D0%92%D1%81%D1%82%D0%B0%D0%B2%D0%BA%D0%B0%20%D0%BA%D0%B0%D1%80%D1%82%D0%B8%D0%BD%D0%BA%D0%B8%20%D0%BA%D0%B0%D0%BA%20%D1%8D%D0%BA%D1%81%D0%BF%D0%B0%D0%BD%D0%B4%D0%B5%D1%80%D0%B0.text)

3.	Для реляционного источника в регламентном отчете можно [настроить пагинацию](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/01.%20%D0%A0%D0%B5%D0%B3%D0%BB%D0%B0%D0%BC%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B5%20%D0%BE%D1%82%D1%87%D1%91%D1%82%D1%8B/04.%20%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%20%D0%BF%D0%B0%D0%B3%D0%B8%D0%BD%D0%B0%D1%86%D0%B8%D0%B8%20%D0%B2%20%D0%BE%D1%82%D1%87%D0%B5%D1%82%D0%B5%20%D0%BD%D0%B0%20%D1%80%D0%B5%D0%BB%D1%8F%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D0%BE%D0%BC%20%D0%B8%D1%81%D1%82%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B5.text)

<a name="Расчеты"></a>  
## __[Расчеты](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/02.%20%D0%A0%D0%B0%D1%81%D1%87%D1%91%D1%82%D1%8B)__ 

1.	Пример [запуска расчёта алгоритма](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/02.%20%D0%A0%D0%B0%D1%81%D1%87%D1%91%D1%82%D1%8B/01.%20%D0%97%D0%B0%D0%BF%D1%83%D1%81%D0%BA%20%D1%80%D0%B0%D1%81%D1%87%D0%B5%D1%82%D0%B0.text) из кода с передачей параметров

2.	Для получения информации о формуле, по которой считалась конкретная точка приемника, используется [метод GetFormulaInfo](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/02.%20%D0%A0%D0%B0%D1%81%D1%87%D1%91%D1%82%D1%8B/02.%20%D0%9F%D0%BE%D0%BB%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D1%84%D0%BE%D1%80%D0%BC%D1%83%D0%BB%D1%8B%20%D1%80%D0%B0%D1%81%D1%87%D0%B5%D1%82%D0%B0%20%D0%B8%D0%B7%20%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC%D0%B0%20(%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D1%81%D0%BA%D0%B0%D1%8F%20%D1%84%D1%83%D0%BD%D0%BA%D1%86%D0%B8%D1%8F).text)


<a name="Работа_с_отметками_измерений"></a>  
## __[Работа с отметками измерений](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/03.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B0%D0%BC%D0%B8)__  

1.	Если в кубе настроено управление измерениями (одно измерение куба перестраивается в зависимости от отметки в другом), то для построения коллекции отметок (SelectionSet-a) для такого куба нужно [учитывать отметки в управляющих измерениях](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/03.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B0%D0%BC%D0%B8/01.%20%D0%9F%D0%BE%D1%81%D1%82%D1%80%D0%BE%D0%B5%D0%BD%D0%B8%D0%B5%20selset-%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%BA%D1%83%D0%B1%D0%B0%20%D1%81%20%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D1%8F%D1%8E%D1%89%D0%B8%D0%BC%D0%B8%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%D0%BC%D0%B8.text)

2.	Пример [установки схемы отметки в пивот](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/03.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B0%D0%BC%D0%B8/02.%20%D0%9F%D1%80%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%B8%D1%82%D1%8C%20%D1%81%D1%85%D0%B5%D0%BC%D1%83%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B8%20%D0%B2%20%D0%BF%D0%B8%D0%B2%D0%BE%D1%82.text)

3.	Для работы с отметкой календарного справочника можно [использовать IDimCalendarSelection](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/03.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B0%D0%BC%D0%B8/03.%20%D0%A1%D1%85%D0%B5%D0%BC%D0%B0%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B8%20%D0%B4%D0%BB%D1%8F%20%D0%BA%D0%B0%D0%BB%D0%B5%D0%BD%D0%B4%D0%B0%D1%80%D0%BD%D0%BE%D0%B3%D0%BE%20%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B0.text)


<a name="Виртуальные_кубы_и_составные_измерения"></a>  
## __[Виртуальные кубы и составные измерения](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F)__ 

1.	По умолчанию в виртуальном кубе для измерения фактов используется составной справочник (ICompoundDimension), он «собирает» факты на основе декарта частных измерений. Если нужен не декарт, а конкретные элементы, то можно [переключиться на конструируемое измерение](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/01.%20%D0%9F%D0%B5%D1%80%D0%B5%D0%BA%D0%BB%D1%8E%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BD%D0%B0%20CustomDimension.text). 
В конструируемое измерение можно добавлять [атрибуты](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/02.%20%D0%94%D0%BE%D0%B1%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B0%D1%82%D1%80%D0%B8%D0%B1%D1%83%D1%82%D0%B0.text) и [элементы](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/03.%20%D0%94%D0%BE%D0%B1%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2.text).

2.	Частные измерения виртуального куба можно [выносить в общие](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/06.%20%D0%92%D1%8B%D0%BD%D0%B5%D1%81%D1%82%D0%B8%20%D1%87%D0%B0%D1%81%D1%82%D0%BD%D0%BE%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B2%20%D0%BE%D0%B1%D1%89%D0%B8%D0%B5%20(forcedCommonDim).text), [джойнить по заданному индексу](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/05.%20Join%20%D1%87%D0%B0%D1%81%D1%82%D0%BD%D1%8B%D1%85%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D0%B9%20%D0%BF%D0%BE%20%D0%B8%D0%BD%D0%B4%D0%B5%D0%BA%D1%81%D1%83.text), чтобы перенести из частных, [расширять отметку](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/04.%20%D0%92%D0%B8%D1%80%D1%82%D1%83%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%BA%D1%83%D0%B1%D1%8B%20%D0%B8%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F/04.%20%D0%A0%D0%B0%D1%81%D1%88%D0%B8%D1%80%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BE%D1%82%D0%BC%D0%B5%D1%82%D0%BA%D0%B8%20%D1%87%D0%B0%D1%81%D1%82%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F.text)

<a name="Работа_с_кэшем_данных"></a>  
## __[Работа с кэшем данных](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/05.%20%D0%9A%D1%8D%D1%88%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)__ 

1.	Кэш [можно делать локальным (для одного пользователя) или глобальным (для всех пользователей)](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/05.%20%D0%9A%D1%8D%D1%88%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85/01.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20GLOBAL.text)

2.	Из кода можно [работать с отдельными элементами кэша](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/05.%20%D0%9A%D1%8D%D1%88%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85/02.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D0%BC%D0%B8%20CacheSaver.text) и [«прогревать» кэш](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/05.%20%D0%9A%D1%8D%D1%88%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85/03.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B5%D0%B2%D0%BE%D0%BC.text)

<a name="Особенности_операций_с_матрицами"></a>  
## __[Особенности операций с матрицами](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/06.%20%D0%9C%D0%B0%D1%82%D1%80%D0%B8%D1%86%D1%8B)__ 
1.	Для быстрых операций над матрицами (сложение, умножение и т.д.) можно использовать [свойство OperationMatrix](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/06.%20%D0%9C%D0%B0%D1%82%D1%80%D0%B8%D1%86%D1%8B/01.%20%D0%A1%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BC%D0%B0%D1%82%D1%80%D0%B8%D1%86.text)

2.	Использование [запросов к матрицам ](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/06.%20%D0%9C%D0%B0%D1%82%D1%80%D0%B8%D1%86%D1%8B/02.%20%D0%A4%D0%B8%D0%BB%D1%8C%D1%82%D1%80%D0%B0%D1%86%D0%B8%D1%8F%20%D0%BC%D0%B0%D1%82%D1%80%D0%B8%D1%86%20(MatrixQuery).text) значительно ускоряет проход по ним

<a name="Измерения_(справочники)"></a>  
## __[Измерения (справочники)](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8))__ 

1.	Составное измерение можно [создавать](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8)/01.%20%D0%A1%D0%BE%D0%B7%D0%B4%D0%B0%D1%82%D1%8C%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D0%BE%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D0%B5.text) и [использовать](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8)/02.%20%D0%9E%D1%82%D0%BA%D1%80%D1%8B%D1%82%D1%8C%20%D1%81%D0%BE%D1%81%D1%82%D0%B0%D0%B2%D0%BD%D0%BE%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D0%B5.text) вне виртуального куба

2.	Можно настроить пользовательский календарь, [сделав календарным](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8)/03.%20%D0%A1%D0%B4%D0%B5%D0%BB%D0%B0%D1%82%D1%8C%20%D0%B8%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BA%D0%B0%D0%BB%D0%B5%D0%BD%D0%B4%D0%B0%D1%80%D0%BD%D1%8B%D0%BC%20(DimAsCalendar).text) подходящий справочник

3.	В справочниках НСИ есть возможность создавать не только обычные вычисляемые атрибуты, но и [атрибуты на запросах](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8)/04.%20%D0%A1%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B0%D1%82%D1%80%D0%B8%D0%B1%D1%83%D1%82%D0%B0%20%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B0%20%D0%9D%D0%A1%D0%98%20%D0%BD%D0%B0%20%D0%B7%D0%B0%D0%BF%D1%80%D0%BE%D1%81%D0%B5.text)

4.	Для справочника можно [создавать группы элементов](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/07.%20%D0%98%D0%B7%D0%BC%D0%B5%D1%80%D0%B5%D0%BD%D0%B8%D1%8F%20(%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8)/05.%20%D0%9F%D0%BE%D0%B4%D0%BA%D0%BB%D1%8E%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BE%D1%82%D0%B1%D0%BE%D1%80%D0%B0%20%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2%20%D0%B2%20%D0%B3%D1%80%D1%83%D0%BF%D0%BF%D1%83%20%D0%BD%D0%B0%20%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D0%B5%20%D0%BC%D0%B0%D0%BA%D1%80%D0%BE%D1%81%D0%B0.text)

<a name="Кубы"></a>  
## __[Кубы](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/08.%20%D0%9A%D1%83%D0%B1%D1%8B)__ 
1.	Автокуб на другом кубе [можно создать без репозитория НСИ](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/08.%20%D0%9A%D1%83%D0%B1%D1%8B/01.%20%D0%A1%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B0%D0%B2%D1%82%D0%BE%D0%BA%D1%83%D0%B1%D0%B0%20%D0%B1%D0%B5%D0%B7%20%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D1%8F%20%D0%9D%D0%A1%D0%98.text) из кода

2.	Стандартный куб поддерживает возможность подключения коллбэков [на запрос данных](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/08.%20%D0%9A%D1%83%D0%B1%D1%8B/02.%20%D0%9A%D0%BE%D0%BB%D0%BB%D0%B1%D1%8D%D0%BA%20%D0%B4%D0%BB%D1%8F%20%D1%80%D0%B5%D0%B4%D0%B0%D0%BA%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20SQL-%D0%B7%D0%B0%D0%BF%D1%80%D0%BE%D1%81%D0%B0%20%D0%BA%20%D0%B4%D0%B0%D1%82%D0%B0%D1%81%D0%B5%D1%82%D1%83%20%D0%BA%D1%83%D0%B1%D0%B0.text)  (от редактирования до полной подмены SQL-запроса) и коллбэков на [сохранение данных](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/08.%20%D0%9A%D1%83%D0%B1%D1%8B/03.%20%D0%9A%D0%BE%D0%BB%D0%BB%D0%B1%D1%8D%D0%BA%20%D0%BD%D0%B0%20%D1%81%D0%BE%D1%85%D1%80%D0%B0%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BA%D1%83%D0%B1%D0%B0.text), где можно редактировать сохраняемые матрицы

<a name="Загрузка_и_трансформация_данных"></a>  
## __[Загрузка и трансформация данных](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/09.%20%D0%97%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D0%B8%20%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)__ 
1.	Аналитическая платформа Форсайт позволяет посылать HTTP-запросы к различным веб-сервисам и интегрироваться со специализированными службами, например, с [брокером сообщений RabbitMQ](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/09.%20%D0%97%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D0%B8%20%D1%82%D1%80%D0%B0%D0%BD%D1%81%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85/01.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%B1%D1%80%D0%BE%D0%BA%D0%B5%D1%80%D0%BE%D0%BC%20RabbitMQ%20(HTTP-%D0%B7%D0%B0%D0%BF%D1%80%D0%BE%D1%81%D1%8B).text)


<a name="Работа_с_перменной_типа_blob"></a>  
## __[Работа с переменной типа blob](https://github.com/ForesightPlatform/Examples/tree/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/10.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%82%D0%B8%D0%BF%D0%B0%20blob)__ 
1.	Данные типа Blob (массив двоичных, либо символьных данных, например, изображения) можно [сохранять](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/10.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%82%D0%B8%D0%BF%D0%B0%20blob/%D0%A1%D0%BE%D1%85%D1%80%D0%B0%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D1%81%D0%BA%D0%B8%D1%85%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85.text) и [читать](https://github.com/ForesightPlatform/Examples/blob/main/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2%20%D0%BF%D0%BE%20%D1%80%D0%B0%D0%B7%D0%B4%D0%B5%D0%BB%D0%B0%D0%BC/10.%20%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%20%D1%81%20%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D0%BE%D0%B9%20%D1%82%D0%B8%D0%BF%D0%B0%20blob/%D0%A7%D1%82%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D1%81%D0%BA%D0%B8%D1%85%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85.text).


***
<!-- Лого  -->
<img src="https://www.fsight.ru/wp-content/uploads/2021/05/fs.png" alt="drawing" width="200"/>
