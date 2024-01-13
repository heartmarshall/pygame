# Happy ogre

Rouglike игра про похождение огра в подземелье. Игра разрабатывается студентами МКН СПбГУ:

* Фомин Никита Павлович [github](https://github.com/heartmarshall)  
* Стас Михайлов [github]()

## Общие сведения об игре:

"Happy ogre" это игра в жанре rouglike с пошаговой боевой системой, в которой игроку предстоит управлять боевым огром, которого отправили на спасение вождя деревни. На своём пути огр должен преодолеть подземелье великого мага Универсетиума. Воин готов к встрече с любыми противниками, но готов ли он к тому, чтобы поумнеть?

## Ключевые особенности игры:

* Процедурная генерация карт, противников и предметов.
* Развитый набор игровых механик, сочетающихся друг с другом.
* Запуск в терминале, текстовая графика. 
* Тактическое планирование боев и пошаговое продвижение по уровням подземелья.
* Возможность огра "поумнеть" в процессе прохождения.

## Stakeholders:
* **Игроки:** основные пользователи игры, которые ожидают интересный и увлекательный геймплей, а также высокое качество контента.
* **Разработчики:** команда разработчиков, ответственных за создание и поддержку игры. 
* **Моддеры и сообщество разработчиков:** люди, заинтересованные в создании модификаций для игры, расширяющих её функциональность и добавляющих новый контент.


## Architectural Drivers
* Репетативность геймплея
* Выполнение внутри терминала
* Простота добавления нового контента
* Пошаговый геймплей

Рассмотрим каждый из них подробнее:

### Репетативность геймплея
Жанр rouglike предполагает, что во время прохождения, игрок будет умирать и начинать всё заново раз за разом. Поэтому очень важно, чтобы каждое новое прохождение было для игрока чем-то уникальным и интересным. 

### Выполнение внутри терминала
Игра разрабатывается для работы в стандартном терминале с использованием клавиатуры для управления. Возможно, будет добавлена поддержка мыши для более удобного ввода.

### Простота добавления нового контента
Основываясь на концепции легкости модификации, игра должна обеспечивать простоту в добавлении нового контента. Мы стремимся к тому, чтобы разработчики могли легко внедрять модификации, добавляющие новые предметы или противников, без необходимости в сложных процедурах.

### Пошаговый геймплей
Игра разделена на ходы - в рамках одного хода активные действия могут совершаться только одним игровым персонажем/мобом

## Viewpoints


## Map
Игровой мир представлят из себя прямоугольную сетку (`карту`), координаты которой начинаюстя в левом верхнем углу. Элемент сетки называется `ячейка`. Рассмотрим классы, которые определяют сущности `карта` и `ячейка`:
***TODO: диаграмма с классами*** 


## Неформальное описание внутреннего устройства игры

## Игровой мир
Описание того, что из себя представляет карта игрового мира (Сетка HxW, состоящая из клеток. Что такое клетка) 


## Описание сущностей
Основные сущности нашей игры.

### Entity


### Item


### Cell


### Event


### Buff


## Как устроен искуственный интеллект мобов

Описание внутреннего устройства класса MobEntity 

Из чего состоит моб:

* Goal Selector
* Move Controller
* Sensors
* Navigator
* Brain (Memory)


### Как работает Goal Selecotor


### Как работают Sensors, пример работы


### 