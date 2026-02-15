IA para Lights Out: Solucionador con Algoritmos de Búsqueda
Este proyecto utiliza Inteligencia Artificial para resolver el juego de lógica Lights Out. El objetivo es encontrar la secuencia de movimientos necesaria para apagar todas las luces de un tablero, analizando la eficiencia de diferentes estrategias de búsqueda en términos de tiempo y memoria RAM.

Sobre el Juego:
Lights Out es un puzzle de cuadrícula donde:

Al presionar una luz, esta cambia de estado (de encendido a apagado, o viceversa).

Sus vecinos directos (arriba, abajo, izquierda, derecha) también cambian de estado.

El juego se gana cuando todas las luces están apagadas.

Algoritmos Implementados:
Para resolver el problema, se comparan tres enfoques clásicos de la Inteligencia Artificial:

BFS (Búsqueda en Anchura): Explora todas las posibilidades nivel por nivel. Garantiza la solución más corta (menos movimientos), pero consume mucha memoria RAM en tableros grandes.

DFS (Búsqueda en Profundidad): Explora un camino hasta el fondo antes de probar otro. Es rápido para encontrar una solución, aunque a veces da más vueltas de las necesarias.

ATS (Algoritmo A-Star / A-Estrella): El método más inteligente. Utiliza una heurística (pistas sobre cuántas luces quedan prendidas) para guiar la búsqueda, logrando un equilibrio perfecto entre rapidez y ahorro de memoria.

Resultados del BenchmarkEl proyecto incluye un análisis comparativo basado en pruebas reales con tableros de 5x5 de alta dificultad:AlgoritmoVentaja PrincipalUso de RAM (Promedio)¿Solución Óptima?BFSMínimos movimientosMuy Alto (>2000 MB)SíDFSVelocidad de hallazgoMedio (~500 MB)NoATSEficiencia InteligenteBajo (~35 MB)Sí

Nota técnica: Según los datos obtenidos, el algoritmo ATS es significativamente más eficiente para resolver tableros complejos sin saturar los recursos del sistema, mientras que BFS es el que más recursos exige.

Estructura del Repositorio:
/src: Contiene la lógica del juego (LightsOutGame) y los algoritmos de búsqueda.

/data: Niveles de prueba en archivos de texto.

LightsOut_BenchMark.csv: Datos detallados del rendimiento de cada algoritmo.

Exploracion.ipynb: Cuaderno interactivo para ejecutar las pruebas en Google Colab o Jupyter.

Cómo ejecutarlo
Clona este repositorio.

Asegúrate de tener Python 3 instalado.

Ejecuta el archivo principal o el cuaderno de notas para ver a la IA resolviendo los tableros en tiempo real.

Proyecto desarrollado para el estudio de algoritmos de búsqueda y resolución de problemas de espacios de estados en Inteligencia Artificial.



