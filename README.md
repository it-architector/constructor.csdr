# Framework CSDR

<h3>Предисловие</h3>

Framework CSDR (Conditions, Space, Distribution и Realization) переведёт программирование на уровень сконцентрированной сборки проекта, результатом которого станет структурированный код.

![](./Картинки/samostoatelnaia-sborka-3d-printera.jpg)


<h3>Навигация</h3>

1. <a href="#Среда-сборки">Среда сборки</a>

     1.1. <a href="#Развёртка">Развёртка</a>
     
     1.2. <a href="#Области">Области</a>
     
2. <a href="#Ход-сборки">Ход сборки</a>

    2.1. <a href="#Действия">Действия</a>
    
    2.2. <a href="#Компиляция">Компиляция</a>
    
![---------------------](./Картинки/hr.png)

<h2>Среда сборки</h2>

<h3>Развёртка</h3>

Среда сборки должна разворачиваться в виде программы на операционные системы: windows, mac и *nix.

<h3>Области</h3>

Для сборки проекта пределены такие области среды:
1. Программист
2. Проект
    1. Архитектура
    2. Дизайн
3. Ход сборки

![](./Картинки/program/shablon1.png)

<h2>Ход сборки</h2>

<h3>Действия</h3>

Каждые действия будут записываться в файл проекта, последовательно, где у каждого действия будет отмечено:

1. **Тип действия**:

     1.1. Добавить
     
     1.2. Изменить
     
     1.3. Удалить
     
     1.4. Зафиксировать // чтобы убрать возможность удаления
     
     1.5. Разафиксировать
2. **Компонент**:

     1.1. Рефлекс
     
     1.2. Место
     
     1.3. Связь
     
     1.4. Реакция

3. **Индификатор** //номер для компонента

4. **Значение**

     - у рефлекса это ориентир (текст), расчёты (текст), места (массив индификаторов мест (для мест с ролями "запросы" и "ожидание" можно дополнять внутренним списком индификаторов мест)), права (код).
    
     - у мест это смысл (текст), роль (массив), связи (индификатор связи), вложение (для роли "атрибутов" текст, массив).
     
     - у связей это тип (текст), возможности и приобретение (два списка для индификаторов мест (или массив array("название_переменной" => "индефикатор_места") при типе "глобальное")), образцы возможности и приобретение (массив), реакция (индификатор реакции).
    
     - у реакций это способность (код).
     
5. **Авторство** // определение программиста
     
6. **Дата** // Дата совершенного действия

<h3>Компиляция</h3>

Это итог программирования, по запросу будет создан код проекта. В коде будут автоматически добавлены функции отмеченных ролей.
