<h1 align="center">DefectDetect</h1>
<h1 align="center">2023</h1>

[Документация к API](docs/APIDOCS.md)

## Содержание

1. Введение
   1. Название
   1. Назначение
   1. Определения, акронимы и сокращения
   1. Краткий обзор
1. Общее описание
   1. Взаимодействие продукта с системой
   1. Функции продукта
   1. Характеристики пользователя
   1. Ограничения
1. Детальные требования
   1. Требования к внешним интерфейсам
      1. Основной интерфейс приложения
      1. Интерфейсы диалоговых окон
   1. Функциональные требования
      1. Особенности хранения данных
      1. Описание основных алгоритмов
      1. Описание функций отдельных элементов
   1. Требования к производительности
1. Дополнения



## Введение

### 1. Название

DefectDetect - [ˈdiːfekt diˈtekt] - ДифектДетэкт

### 2. Назначение

Данное приложение рассчитано на специалистов по проверке квартир на поиск дефектов, с интуитивно понятным интерфейсом, позволяющий беспроблемно, понятно и доступно создавать отчеты о дефектах в квартире.

### 3. Определения, акронимы и сокращения

Дефекты, обнаружение, отчёт.

### 4. Краткий обзор

Данное приложение с интуитивно понятным интерфейсом позволит вам легко создавать отчеты о дефектах в квартире, позволяя вам просматривать их в любое время, а также сразу отправлять отчеты на сервер. 

Вы можете: Создавать/сортировать/отправлять отчёты о квартирах. Также, можно получать эти отчеты с сервера.

## Общее описание

### 1. Взаимодействие продукта с системой

Для запуска приложения требуется устройство с ОС Android 7.0 или выше.

Приложение обладает своей хронологией папок на физическом носителе, к которым имеет полные права на изменения. 
Приложение способно к считыванию сигналов с сенсорного экрана, а также способно выводить информацию через Устройства вывода (конкретно, через тот же экран).

### 2. Функции продукта

При первом запуске приложения (описание алгоритмов/функций см. п. “Детальные требования”) пользователь увидит главное меню.

Приложение будет сохранять данные о добавленных пользователем объектах внутри самого приложения, а также отправлять и сохранять отчеты, созданные пользователем.

Пользователю в основном окне предоставляются следующие кнопки:

> - Кнопка "Добавить объект"
> - Кнопка объекта, добавленного пользователем

После нажатия кнопки "добавить объект", пользователя перенаправляет на страницу добавления объекта.

При нажатии кнопки дома, пользователя перенаправит на страницу объекта, где будет указана информация о добавленных пользователем квартирах.

Находясь на любой из вкладок, пользователю всегда будет

представлена одна простая кнопка добавления какого-либо объекта (зависит от того, на какой странице находится пользователь).
Меню обладает следующим функционалом

> - Кнопка "Добавить объект"
> - Кнопка объекта (который был ранее добавлен пользователем)

Пользователь может добавить объект на странице добавления объекта(объектом может быть как Дом, Квартира, так и Отчет о дефектах в квартире). Для этого, пользователю надо нажать на кнопку добавления объекта, которая находится внизу экрана и его направит на страницу со специальной формой.

На всех типах таких страниц, присутствуют следующая кнопка:

> - Кнопка "Добавить"

Которая требуется для сохранения действий пользователя на данной странице.

Страница дома/квартиры представляет собой список добавленных пользователем объектов, а также кнопки “Добавить объект" и “Удалить".

"Удалить": При нажатии на соответствующую кнопку пользователь может удалить данный(ую) дом/квартиру из списка.

### 3. Характеристика пользователя

Пользователь должен быть специалистом в сфере проверки квартир на предмет дефекта, но каких-либо выдающихся способностей для использования приложения не требуется.

### 4. Ограничения
1. Приложение должно быть полностью безопасным для личных данных пользователя.
1. Приложение не должно пагубно влиять на физическое и психологическое здоровье пользователя.
1. В приложении не должно быть моментов, которые могут пагубно повлиять на физическое и психологическое состояние пользователя. В случае, если без таких моментов не обойтись, должно(ы) быть соответствующее(ие) предупреждение(ия).
1. Приложение не должно нести никакого вреда системе пользователю, а также должно рационально использовать ее ресурсы.
1. Приложение должно быть максимально оптимизировано и оттестировано на критических ситуациях.

1. Приложение должно работать как в режиме оффлайн, так и онлайн.

## Детальные требования

### 1. Требования к внешним интерфейсам
#### 1.1. Основной интерфейс приложения

Приложение должно быть достаточно лёгким для понимания, а также с простым функционалом. Интерфейс для пользователя должен быть интуитивно понятен.


К дизайну могут быть применены изменения, при согласовании их с заказчиком.

#### 1.2. Интерфейсы страниц приложения
В приложении должны присутствовать следующие страницы:
> - Страница для добавления какого-либо объекта
> - Страницы списка объектов


#### Макеты страниц:
<table>
   <tr>
      <td>
         <img width="450px" height="500px" src="https://user-images.githubusercontent.com/69642892/229340268-6747808c-75ba-458c-b9c0-654fa75c5573.jpg">
      </td>
      <td>
         <img width="300px" height="500px" src="https://user-images.githubusercontent.com/69642892/229340275-f1c77645-c3a5-4731-8111-98ab69b6676c.jpg">
      </td>
   </tr>
</table>




### 2. Функциональные требования
#### 2.1. Особенности хранения данных

Хранение информации о жанрах композиций, составах альбомов, а также самих композиций должно быть реализовано с использованием базы данных(далее БД).

#### Структура БД

Локальная БД:

![Aspose Words a9f95431-fe29-4189-be99-8003f81f57bd 003](https://user-images.githubusercontent.com/69642892/229340670-21cc811c-d1cb-427e-8075-1084de8142c8.png)

Серверная БД:

![Aspose Words a9f95431-fe29-4189-be99-8003f81f57bd 004](https://user-images.githubusercontent.com/69642892/229340680-ae9ef694-18cf-4715-b3fd-52fdd1356c83.png)

#### 2.2. Описание основных алгоритмов

Главная цель приложения – упростить работу специалистов, а также уменьшить количество обманов и сговоров между подрядчиком и специалистом.
Должна быть реализована возможность добавлять фотографии в приложение, чтобы в дальнейшем отправлять фото на сервер.
Должна быть реализована возможность составлять отчеты, через специальную страницу.

Должен быть реализован алгоритм, который автоматически формирует отчеты на сервере, на основе предоставленных данных, введенных пользователем.

По возможности реализовать все алгоритмы, которые работают с данными, с использованием БД и соответственно запросов.	

#### 2.3. Описание функций отдельных элементов

По возможности, приложение должно быть построено на функциях и классах с их описаниями, для дальнейшей поддержки продукта.

Дизайн приложения должен быть рассчитан как можно на большее количество типов разрешения экрана.
Элементы интерфейса не должны "сползать” или быть недоступными из-за особенности системы.

### 3. Требования к производительности

#### 3.1. Приложение должно запускаться как можно на большем разнообразии конфигурации Систем.

Приложение не должно требовать от Системы пользователя дискретный видеоадаптер (дискретную видеокарту/GPU).
По возможности протестировать продукт на наличие утечек памяти, при долгом или ненадлежащем использовании продукта.
Приложение должно использоваться пространство на физическом накопителе экономно. Другими словами, приложение не должно записывать одни и те же данные по несколько раз, а также, по возможности, использовать общий вид (формулы, особенности разрешений файлов) для получения информации.

## Дополнения

Настоящее Техническое Задание может уточняться/дополняться/изменяться в период создания и поддержки продукта




