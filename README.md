# Proyecto de Unity

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.



## Reglas de escritura
- El máximo número de caracteres para una línea está limitada a 80 (El editor de código es capaz de mostrar una guía para respetar este límite).

- Todos los atributos de clase deben declararse al principio y debajo de la llave de apertura `{`

- Todos los métodos propios de Unity como `start()`, `update()`, `FixedUpdate()`, etc... deben declararse antes que los métodos nuestros.

- Los comentarios son imprescindibles para explicar qué hace cada parte que pueda interpretarse de forma errónea.

- Las variables se deben declarar en camelCase
	```
	addForce
	destroyObject
	cubeDimension
	```
	
- Las constantes se deben declarar en mayúsculas y como variables globales (atributos de clase)
	```
	MAXVELOCITY
	PI
	```
	
- Todas las variables deben declararse en private excepto aquellas que deben aparecer en el editor de Unity, en ese caso deben ser public.

- Todos los métodos de clase deben declararse en private excepto aquellas que sean usadas fuera de la clase.

- Todas las funciones, métodos, condicionales y bucles (control de flujo) deben ser representadas de las siguiente forma.
	```
	if  (true)
	{
		// ...
	}
	```
	
- Si la condicional es una sola línea se permite omitir las llaves
	```
	if (true)
		// ...
	```

## Log

#### 11 - 4 - 22

- Añadido modelo Cube dentro de carpeta Models y cuatro texturas difusas para el modelo Cube.

- Añadido cuatro materiales dentro de carpeta Materials para usar con el modelo cubo
  - Onion, Mushroom, Water, Turtle

#### 12 - 4 - 22

- Añadido clase Player que contiene el control del movimiento y del salto (incompleto)
  - Para moverse pulsar las teclas de flecha izquierda y derecha
  - Para saltar pulsar la tecla de flecha arriba

#### 13 - 4 - 22

- Renombrado método PlayerControl() a MovementControl()
- Añadido componente Box Collider a la malla default del gameObject Onion (Onion → Model → default)
- Añadido componente RigidBody al gameObject Onion
- Añadido componente Box Collider al gameObject Floor
- Añadido restricción en la posición del eje Z para el gameObject Onion
- Añadido restricción en la rotación del eje X, Y, Z para el gameObject Onion
- Añadido control de la aceleración pulsando la tecla Shift
- Los siguientes valores para el Script player han sido establecidos en:
	- Speed: 5
	- MaxSpeed: 12
	- Acceleration: 6
	- JumpForce: 1000
	- Gravity: 48

