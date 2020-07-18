# CSDR среда

<h3>Предисловие</h3>

CSDR среда предназначена для визуального построения модульного кода в согласии с <a href="https://github.com/it-architector/right.csdr">порядком CSDR</a>.

![](./Картинки/konstruktory.jpg)

**Внимание!** Так как порядок CSDR не готов, нижеперечисленный текст не является завершённым.

<h3>Навигация</h3>

1. <a href="#Среда">Среда</a>

     1.1. <a href="#Развёртка">Развёртка</a>
     
     1.2. <a href="#Области">Области</a>
     
     1.3. <a href="#Аутентификация">Аутентификация</a>
     
2. <a href="#Построение">Построение</a>

    2.1. <a href="#Планирование">Планирование</a>

    2.2. <a href="#Действия">Действия</a>
    
    2.3. <a href="#Компиляция">Компиляция</a>
    
![---------------------](./Картинки/hr.png)

<h2>Среда</h2>

<h3>Развёртка</h3>

Среда построения модуля должна разворачиваться в виде программы на операционные системы: windows, mac, nix, android и ios.

<h3>Области</h3>

Для построения модуля заданы такие области среды:
1. Модули
2. Конструкции
3. Архитектура
4. Дизайн
5. Ход построения

![](./Картинки/program/shablon1.png)

> В области **модули** можно будет:
> 1. Управлять модулями
> 2. Управлять замыслом

> В области **конструкции** можно будет:
> 1. Управлять конструкциями

> В области **архитектуры**:
> 1. Управлять рефлексией

> В области **дизайна**:
> 1. Управлять местом
> 2. Управлять связью
> 3. Управлять реакцией

> В области **хода построения** можно увидеть лог всех действий.

<h3>Аутентификация</h3>

Без авторизации все области заблокированы. Здесь будет форма для идентификации и получение прав доступа к областям.
    
![---------------------](./Картинки/hr.png)

<h2>Построение</h2>

<h3>Планирование</h3>

Для взаимодействия между областями нужны такие непрерываемые этапы: создание конструкции → делигирование → ознакомление → выполнение  →  сделано / сделать.

> Где, создание конструкции - постановка цели.
>
> Где, делигирование - перевод цели в следующую область.
>
> Где, ознакомление - сбор данных, изучение дополнительных материалов.
>
> Где, выполнение - выполнение цели.
>
> Где, сделано - цель выполнена.

В итоге получится такое планирование:

Область конструкции

1 → создание конструкции

2 → делигирование

Область архитектуры

3 → ознакомление

4 → выполнение

5 → делигирование

Область дизайна

6 → ознакомление

7 → выполнение

8 → сделано

> При этом возможен реверс с комментарием, на случай недоработки:
> 1) ознакомление → создание конструкции
> 2) выполнение  →  ознакомление
> 3) сделано  →  создание конструкции
> 4) создание конструкции  →  сделано

<h3>Действия</h3>

Под действиями будем считать манипуляции в таких областях: конструкции, архитектура и дизайн.

У каждого действия будет отмечено:

1. **Тип действия**:

     1.1. Добавить
     
     1.2. Изменить
     
     1.3. Удалить

2. **Компонент**:

     1.1. Замысел

     1.2. Конструкция

     1.3. Рефлекс
     
     1.4. Место
     
     1.5. Связь
     
     1.6. Реакция

3. **Значение** // значение для компонента
     
4. **Авторство** // кто сделал
     
5. **Дата** // дата совершенного действия

<h3>Компиляция</h3>

По кнопке компиляции создаётся новая версия модуля, которая будет включать в себя сделанные конструкции. Описание новой версии это лог проведённого планирования.


