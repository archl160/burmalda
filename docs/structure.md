# Структура проекта

## Сцены проекта

|Название сцены|Путь|Краткое описание|
|-|-|-|
|PlatformerDemo|Assets/IndieMarc/PlatformerDemo|Содержит игрока,траву,освещение,задний фон,сетку уровня.|



## Основная игровая сцена: PlatformerDemo

### Все объекты на сцене

|Объект|Является префабом?|Примечание|
|-|-|-|
|Main Camera|Нет|Камера, следует за игроком|
|CharacterPlatformer|Да|Управляемый персонаж|
|TilemapGrid|Нет|Сетка|
|TreeBackground|Да|Задний фон|
|Grass|Да|Трава|



### Объект CharacterPlatformer

**Компоненты:**

|Компонент|Параметры (что можно настроить в Inspector)|
|-|-|
|Transform|Position, Rotation, Scale|
|Sprite Renderer|Sprite, Color, Sorting Layer, Order in Layer|
|Rigidbody2D|Mass, Gravity Scale, Linear Drag, Angular Drag, Collision Detection|
|BoxCollider2D|Size, Offset, Material|
|PlayerController (Script)|Speed, Jump Force, Ground Check|
|Animator|Controller, Avatar|

**Что можно настроить через Inspector:**

* Скорость передвижения (Speed)
* Сила прыжка (Jump Force)
* Масса персонажа (Mass)
* Масштаб гравитации (Gravity Scale)

### Скрипты проекта

|Скрипт|Где прикреплён|Что делает (по названию)|
|-|-|-|
|PlayerController.cs|Player|Управляет движением и прыжками игрока|
|CarryItem|Hand|Поднимает предмет|
|CharacterAnim|CharacterPlatformer|Анимация персонажа|
|CharacterHoldItem|CharacterPlatformer|Держит предмет|
|FollowCamera|MainCamera|Следует за персонажем|
|Lever|Lever|Взаимодействует с объектами|
|ParallaxBackground|Background|Отвечает за фон|
|TheAudio|Objects|Отвечает за звук|



