Benchmark de Lights Out AI Solver
Este repositorio contiene un benchmark completo para el problema de Lights Out, aplicado a un entorno de resolución de puzzles lógicos mediante Inteligencia Artificial.
El proyecto evalúa la eficiencia de distintos algoritmos de búsqueda para apagar una cuadrícula de luces de manera óptima.

📌 Objetivo del proyecto
Simular un sistema de lógica Lights Out: Implementar las mecánicas de cambio de estado de luces y sus adyacentes.

Evaluar el desempeño del sistema usando datasets de diferentes tamaños: Probar la capacidad de la IA en tableros de diversas complejidades.

Calcular el costo total (movimientos y recursos): Determinar la ruta óptima y el gasto de memoria RAM.

Facilitar la comparación entre escenarios: Analizar cómo escalan los algoritmos BFS, DFS y ATS ante problemas más difíciles.

🧠 Contexto del problema
El juego consiste en una cuadrícula de luces. El objetivo es apagar todos los focos considerando las siguientes reglas:

Al presionar una luz, esta cambia de estado (encendido/apagado).

Sus vecinos directos (arriba, abajo, izquierda y derecha) también cambian de estado.

El reto es encontrar la combinación exacta de clics que deja el tablero totalmente a oscuras.

📂 Estructura del proyecto
main.py: Código principal ejecutable que integra los algoritmos de búsqueda.

data/: Datasets con configuraciones iniciales de tableros (niveles).

README_DATASETS.md: Descripción de los archivos de entrada y niveles de dificultad.

requirements.txt: Dependencias del proyecto (bibliotecas necesarias para el análisis).

▶️ Cómo ejecutar el proyecto
Clonar el repositorio

Bash
git clone https://github.com/tu_usuario/lights-out-ai-benchmark.git
Instalar dependencias

Bash
pip install -r requirements.txt
Ejecutar el código

Bash
python main.py
📝 Resumen de Algoritmos
BFS: Encuentra la solución con menos movimientos.

DFS: Encuentra soluciones rápidamente en tableros profundos.

ATS: Optimiza el uso de memoria RAM mediante el uso de heurísticas inteligentes.
