# Быстрее бы на землю


Самолёт - один из самых удобных видов транспорта, его преимущества - это скорость, удобство и безопасность. Если перелёт совершается на слишком большое расстояние, то нам необходима посадка на дозаправку, поэтому давайте найдём ближайшее место посадки.
Для этого мы напишем программу, которая будет показывать самый ближайший аэропорт.


### Формат ввода
- В первой строке записаны координаты самолёта ( для простоты считаем, что мы летим по плоской поверхности и максимаьные координаты - это +-10000(км) )
- Во второй строке записано направление самолёта - в градусах от оси Oy
- В третьей строке текущая скорость(км/ч), расстояние, которое возможно пролететь(км)
- В четвёртой число N - количество аэропортов, о которых нам известно
- В следующих N строках идут координаты аэропортов

### Формат вывода 
- Координаты ближайшего аэропорта, до которого мы можем долететь,
если такого нет, вывести "Критическая ситуация"


#### Пример 1
----------
##### Ввод
70.46 -40.55

45

800 200

3

44.55 -50.23

59.11 45.12

55.44 -40.1

##### Вывод
55.44 -40.1

### Теоретическая справка
Самолёт не может поворачивать моментально для разворота ему необходимо начать вираж, радиус виража высчитывается по формуле $$R = \frac{V^2}{g \tg(\gamma)}$$
Где $\gamma$ - угол наклона во время виража, значение угла может быть в диапазоне от 0 до 20 градусов
g = 9.81
