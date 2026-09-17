Generador Procedural de Contenido (PCG)

Versión del motor
Unity 6.

Instrucciones para ejecutar
1. Abrir el proyecto en UnityHub
2. Abrir la escena `PCG_Basic`.
3. Seleccionar el GameObject `LevelGenerator`.
4. Verificar que los Prefabs `Floor`, `Wall`, `Start`, `Goal` y `Reward` estén asignados en el Inspector.
5. Presionar *Play* para ejecutar el generador.
6. Para realizar pruebas, modificar los parámetros del generador desde el Inspector y volver a ejecutar la escena.

Semilla de prueba
*12345*
La semilla se encuentra en el parámetro `Seed` del objeto `LevelGenerator`.

Reglas implementadas
* Los bordes del mapa se generan como muros.
* El inicio y la meta se generan en celdas transitables.
* Se genera un corredor entre el inicio y la meta para garantizar una ruta.
* Las recompensas solamente se colocan en celdas transitables.

Restricciones implementadas
* El mapa debe tener un mínimo de 5 × 5 celdas.
* El inicio no puede ocupar una celda con muro.
* La meta no puede ocupar una celda con muro.
* Las recompensas no pueden colocarse en muros.
* Las recompensas no pueden ocupar las posiciones de inicio o meta.
* La cantidad de recompensas se limita a las posiciones transitables disponibles.
