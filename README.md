# amxx-physxmod

EN:
===
What is PhysXMOD?
PhysXMOD is an AMXModX (http://www.amxmodx.org/ ) module (note: my module does not use the Metamod API).
PhysXMOD enables developers to utilize the external Nvidia PhysX 4 physics engine.
The currently used version of PhysX 4 does not support CUDA hardware acceleration on Linux. Physics calculations will be performed exclusively on the CPU. On Windows, hardware acceleration is supported and functional.

Requirements:
1) AMXModX (version appears to be irrelevant, but I have only tested with versions 1.9.0 and 1.10.0).
2) Ability to copy the PhysX libraries into the server's root directory—the directory from which the server is launched (i.e., not the game mod folder, but the server's root folder). If your hosting provider does not allow access to the server's root directory, you may attempt to copy the PhysX libraries there via a plugin (however, this does not work on certain hosts, such as MyArena).

How does it work?
The module allows you to create and interact with objects within the PhysX world, including dynamic, static, and kinematic objects.
After creating an object, you can set and retrieve its properties. This enables you to apply PhysX physics to entities within the game world.

Usage Examples:
1) *Photo of a pile of chickens*
2) *Photo of Aztec bridge*
3) *Video 1*
4) *Video 2*
5) *Video 3*

Hello World?
This is a simple example demonstrating how to:
1) Initialize PhysX and calculate physics simulation steps.
2) Create and delete static objects (world), dynamic objects (spheres and chickens), and kinematic objects (player).
3) Retrieve and assign object properties, and convert quaternion angles (used in PhysX) into Euler angles (used in the game).
4) Detect collisions
```Pawn
CODE
```

Documentation?
To view the documentation, open the latest .inc file. All PhysXMOD features are described there.

Installation:
1) Copy the PhysX libraries into the server's root directory.
2) Place the module file into the amxmodx/modules/ folder.
3) Place example_physxmod.amxx into the amxmodx/plugins/ folder.
4) In the amxmodx/configs/ directory, add the module and plugin entries to modules.ini and plugins.ini files, respectively.

Building:

Future Plans:

RU:
===
Что такое PhysXMOD?
PhysXMOD - это AMXModX (http://www.amxmodx.org/) модуль (кстати, мой модуль не использует Metamod API).
PhysXMOD позволяет разработчикам использовать внешний физический движок Nvidia PhysX 4.
Текущая используемая версия версия PhysX 4 не поддерживает аппаратное ускорение CUDA на Linux. Физика будет рассчитываться исключительно на CPU. На Windows аппаратное ускорение работает.

Требования: 
1) AMXModX (похоже, что версия не имеет значения, но я тестировал только на 1.9.0 и 1.10.0)
2) Возможность копирования библиотек PhysX в корневую папку сервера, из которой запускается сервер (то есть, не в папку мода игры, а в корневую папку сервера). Если на вашем хостинге корневая папка сервера недоступна для доступа, то можно попробовать скопировать туда библиотеки PhysX плагином (но это не работает на некоторых хостингах, например, на MyArena).

Как это работает? 
Модуль позволяет вам создавать и работать с объектами в мире PhysX, включая динамические, статические и кинематические объекты.
После создания объекта, вы можете задавать и считывать его свойства. Таким образом, вы можете использовать PhysX физику для ентити в мире игры.

Примеры работы:
1) *фото кучи куриц*
2) *фото моста Aztec*
3) *Видео 1*
3) *Видео 2*
3) *Видео 3*

Hello world?
Это простой пример, где вы можете изучить как работают:
1) Инициализация PhysX и расчёт шагов обработки физики.
2) Создание и удаление статических объектов (мир), динамических объектов (сферы и курицы), кинематичных объектов (игрок).
3) Получение и задание свойств объектам, преобразование углов кватернионов (используются в PhysX) в углы Эйлера (используются в игре).
4) Отлов коллизий
```Pawn
CODE
```

Документация?
Для просмотра документации, вы можете открыть последний .inc файл. Все возможности PhysXMOD описаны там.

Установка: 
1) Переместить библиотеки PhysX в корневую папку сервера
2) Переместить файл модуля в папку amxmodx/modules/
3) Переместить example_physxmod.amxx в папку amxmodx/plugins/
4) В папке amxmodx/configs/ в файлах modules.ini и plugins.ini указать модуль и плагин.

Сборка:

Будущие планы:
