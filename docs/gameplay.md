# Геймплей проекта

## Физические параметры

### Глобальная гравитация

* **Physics 2D → Gravity:** X = 0, Y = -9.81 (значение по умолчанию)

### Объекты с Rigidbody2D

|Объект|Mass|Gravity Scale|Linear Drag|Angular Drag|Collision Detection|
|-|-|-|-|-|-|
|Player|10|0|1|1|discrete|



### Physics Material 2D

|Материал|Friction|Bounciness|Где используется|
|-|-|-|-|
|None|-|-|-|



## Префабы

### Препятствия

|Префаб|Компоненты|
|-|-|
|CharacterPlatformer|Animator, Rigidbody 2D, Capsule Collider 2D, <br />Player Character (Script), Character Anim (Script), Character Hold Item (Script)|
|Grass (Prefab Asset)|Sprite Rendered|
|Lever (Prefab Asset)|Sprite Renderer, Box Collider 2D, Lever (Script), Audio Source|
|TreeBackground|-|





## Параметры, влияющие на сложность

|Параметр|Где|Влияние|
|-|-|-|
|Move\_max|PlayerCharacter|Скорость игрока|
|Jump\_strenght|PlayerCharacter|Высота прыжка|
|Mass|Rigidbody2D|Инерция|
|Gravity Scale|Rigidbody2D|Сила падения|



