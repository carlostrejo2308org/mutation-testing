# Mutation testing

Mutation testing fue originalmente propuesto por Dick Lipton en los 70's.

Esta es una técnica que se enfoca en medir la calidad de los casos de prueba. Y la prueba del programa en si es un beneficio secundario.

Cabe resaltar que mutation testing no debería ser la única estrategia empleada en las pruebas, si no que se debe usar en conjunto con otras estrategias de prueba, como lo es "control flow testing" o "data flow testing".

## Actividad
Examina el archivo "minion.py" y analiza sus funciones. Notaras que algunas de ellas las hemos usado en asignaciones pasadas, si notas algún error en ellas, todavía no las corrijas.

1. Crea los casos de prueba para cada funcion
2. Ejecuta un test coverage y crea suficientes casos de prueba para obtener un coverage del 100%
3. Si tus tests fallaron, ahora si corrige los programas para que pasen todos los casos de prueba
4. Crea de forma manual 4 mutantes para solo uno de las funciones, elige el que tu quieras. (Excepto la funcion triple)
5. Corre todos los casos de prueba para cada mutante que creaste. Definiremos un mutation score del 100%.
6. Para cada mutante que no haya muerte, analízalo y define si es equivalente o matable.
7. Calcula el mutation score
8. Si el mutation score es menor al 100%, entonces crea mas casos de prueba que pase el programa original y que mate a los asesinables.

Después de hacer eso, ahora usa la libreria "mutmut" para las demás funciones. Analiza los mutantes que siguen vivos y crea suficientes casos de prueba para asesinarlos.

