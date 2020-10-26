# NeonGame
Игра-платформер на Unreal Engine 4
- Овчинникова Алина 
- hebgehogg@gmail.com
- тел: +7(950) 446-12-02

### Версия 4.25.3


# Design doc

> Concept: 

Platforms: Windows  
Technologies: Unreal Engine 4  
Languages:  английский  
Genre: 3D platformer  
Emotions: снятие стресса после работы/учебы (убийство времени)  
Rating:  12+  
User Number:  single-player  
Gameplay time:  около 20 минут  
Maine mechanic:  собирать очки  
Setting:  постоянное увеличение скорости  
Goal: собрать как можно больше очков  


> Mood: 

![Mood](https://github.com/hebgehogg/NeonGame/blob/main/photos/Visual%20references.jpg)


> Game Character: 

Персонаж - стандартнвая фигурка из UE4  
Пеередвигается на стрелочки (вправо/влево) и пробел  
Камера от 3 лица  
Имеет взаимодейсивия с объектами на карте


> Interface: 

### Окно открывающиеся при входе  

![Окно](https://github.com/hebgehogg/NeonGame/blob/main/photos/StartGame.png)

### Окно паузы  

![Окно](https://github.com/hebgehogg/NeonGame/blob/main/photos/StartGame.png)

### Окно окончания игры  

![Окно](https://github.com/hebgehogg/NeonGame/blob/main/photos/Paused.png)


> Gameplay map: 

![Gameplay map](https://github.com/hebgehogg/NeonGame/blob/main/photos/Gameplay%20map.jpg)


> Level design: 

Каждый новый уровень - это увеличение скорости, которая начинается с 600 и увеличивается до 1500 с каждой секундой.  
На каждом уровне есть "Coins', чем больше их собрал игрок - тем лучше, в игре для этого добавлен счетчик который выводит все на экран.  
Лучший счет запоминается - хранится у пользователя на устройстве.  
Все отображено в интерфейсе.  

![Level design](https://github.com/hebgehogg/NeonGame/blob/main/photos/LevelDesign.png)

Чтобы не нагружать ПК, после прохода блока персонажем - он удаляется. (максимум 10  блоков на карте)  
Тот же механизм работает с объектами на карте  

![Level design](https://github.com/hebgehogg/NeonGame/blob/main/photos/Destroy.png)


> Balance:

Количество уровней - бескончно. 
Количество жизней персонажа - 1.

# Levels

Генирация происходит по средстам рандома, каждый элемент генерируется отдельно - Разделение между блоками(дыра)/Высокая платформа/Низкая платформа/Очки.  
Видимость на 10 блоков.

Чтобы персонаж не умирал в случае спавна блока перед ним в начале игры, была добавлена проверка "если герой на 1 платформе (в начале) то отрисовка с 10 блока".  

![Levels](https://github.com/hebgehogg/NeonGame/blob/main/photos/%D0%9F%D1%80%D0%B5%D0%B4%D0%BC%D0%B5%D1%82%D1%8B.png)

# Управление

В игре есть 3 дорожки, переход между ними было решено сделать как в SF, как мне кажется в ранере при повышенной скорости эта самая удобная механника передвижения.  

* Шаг влево - стрелочка влево, очевидно даже для не продвинутого пользователя  
* Шаг вправо - стрелочка вправо, очевидно даже для не продвинутого пользователя  
* Прыжок - пробел, очевидно даже для не продвинутого пользователя
* Пауза - на "Р" тк это логично, если выход на ESC  
* Выход - ESC

![Управление](https://github.com/hebgehogg/NeonGame/blob/main/photos/%D0%A3%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5.png)


# Конец игры 

Наступает когда игрок натыкается на препядствие.

![Конец игры ](https://github.com/hebgehogg/NeonGame/blob/main/photos/%D0%A1%D0%BC%D0%B5%D1%80%D1%82%D1%8C.png)


# Дизайн

Все блоки, заставки и картинки были нарисованы и смоделированы мной.



