# Лабораторные работы по дисциплине Тестирование Программного Обечпечения

## Лабораторная работа 1
- Для указанной функции провести модульное тестирование разложения функции
в степенной ряд. Выбрать достаточное тестовое покрытие.

  Заданная функция - arcsin(x).

- Провести модульное тестирование указанного алгоритма. Для этого выбрать
характерные точки внутри алгоритма, и для предложенных самостоятельно
наборов исходных данных записать последовательность попадания в
характерные точки. Сравнить последовательность попадания с эталонной.

  Программный модуль для работы c хеш-таблицей с закрытой адресацией (Hash Integer, http://www.cs.usfca.edu/~galles/visualization/OpenHash.html).

- Сформировать доменную модель для заданного текста. Разработать тестовое
покрытие для данной доменной модели.

  Описание предметной области:
  
  Поскольку Форд так и не научился произносить свое настоящее имя, его отец,
в конце концов, умер от стыда, который в некоторых частях Галактики все
еще является смертельной болезнью. В школе Форду дали прозвище Ыкс, что на
языке Бетельгейзе-5 означает: "мальчик, который не может внятно
объяснить, что такое Хрунг, и почему он решил сотрястись именно на
Бетельгейзе-7".

## Лабораторная работа 2
Провести интеграционное тестирование программы, осуществляющей вычисление
системы функций (в соответствии с вариантом):
![image](https://github.com/NikaT1/Software_testing/assets/74957274/77d5004f-533b-4ffb-872c-602c302859c8)

## Лабораторная работа 3
Сформировать варианты использования, разработать на их основе тестовое покрытие
покрытие и провести функциональное тестирование интерфейса сайта (в соответствии
с вариантом): https://new.fastpic.org/

Требования к выполнению работы:
- Тестовое покрытие должно быть сформировано на основании набора
прецедентов использования сайта.
- Тестирование должно осуществляться автоматически - с помощью системы
автоматизированного тестирования Selenium.
- Шаблоны тестов должны формироваться при помощи Selenium IDE и
исполняться при помощи Selenium RC в браузерах Firefox и Chrome.
- Предполагается, что тестируемый сайт использует динамическую генерацию
элементов на странице, т.е. выбор элемента в DOM должен осуществляться не
на основании его ID, а с помощью XPath.

## Лабораторная работа 4
С помощью программного пакета Apache JMeter провести нагрузочное и стресстестирование веб-приложения в соответствии с вариантом задания.

В ходе нагрузочного тестирования необходимо протестировать 3 конфигурации
аппаратного обеспечения и выбрать среди них наиболее дешёвую, удовлетворяющую
требованиям по максимальному времени отклика приложения при заданной нагрузке (в
соответствии с вариантом).

В ходе стресс-тестирования необходимо определить, при какой нагрузке выбранная на
предыдущем шаге конфигурация перестаёт удовлетворять требованиями по
максимальному времени отклика. Для этого необходимо построить график
зависимости времени отклика приложения от нагрузки.

- Приложение для тестирования доступно только во внутренней сети кафедры.
- Если запрос содержит некорректные параметры, сервер возвращает HTTP 403.
- Если приложение не справляется с нагрузкой, сервер возвращает HTTP 503.
  
Параметры тестируемого веб-приложения:
- URL первой конфигурации ($ 5900)
http://stload.se.ifmo.ru:8080?token=492557781&user=2129854793&config=1;
- URL второй конфигурации ($ 7200)
http://stload.se.ifmo.ru:8080?token=492557781&user=2129854793&config=2;
- URL третьей конфигурации ($ 12800)
http://stload.se.ifmo.ru:8080?token=492557781&user=2129854793&config=3;
- Максимальное количество параллельных пользователей - 14;
- Средняя нагрузка, формируемая одним пользователем - 20 запр. в мин.;
- Максимально допустимое время обработки запроса - 850 мс.
