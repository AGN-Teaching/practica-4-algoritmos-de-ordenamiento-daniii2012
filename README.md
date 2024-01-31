[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ke8zCzPd)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-7f7980b617ed060a017424585567c406b6ee15c891e84e1186181d67ecf80aa0.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=13517812)

![uamcua](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/5429fc6a-4532-4f92-9632-426cedf21a92)

# UNIVERSIDAD AUTÓNOMA METROPOLITANA "UNIDAD CUAJIMALPA"
## LICENCIATURA: INGENIERÍA EN COMPUTACIÓN
# PRÁCTICA 4
## ALGORITMOS DE ORDENAMIENTO


UEA: **ESTRUCTURA DE DATOS LINEALES**



*ESTUDIANTE:*


NAVA MARTÍNEZ DANIELA                 2223028762



*PROFESOR:*


GARCÍA NÁJERA ABEL


# OBJETIVO 
<p align="justify">
El propósito central de esta investigación es llevar a cabo una evaluación experimental para verificar el tiempo de ejecución de distintos "algoritmos de ordenamiento", entre ellos: el algoritmo de inserción, el algoritmo de selección, el algoritmo de burbuja, el merge sort y el quicksort. A través de la implementación y ejecución de estos algoritmos, se busca analizar y comparar su rendimiento temporal. La medición del tiempo de ejecución se llevará a cabo en condiciones controladas, utilizando conjuntos de datos de diversos tamaños. Este análisis tiene como objetivo identificar patrones de eficiencia y comportamiento específicos de cada algoritmo en diferentes contextos, proporcionando información valiosa sobre su desempeño relativo y contribuyendo así a la comprensión práctica de su utilidad en el procesamiento de datos.
</p>



# RESÚMEN
<p align="justify">
En la UEA "Estructura de Datos Lineales", esta sección se enfoca en el estudio de "Algoritmos de ordenamiento", son procedimientos computacionales que organizan elementos de una lista en un orden específico, como ascendente o descendente. Que sirven para facilitar la búsqueda y recuperación eficiente de datos.
</p>

<p align="justify">
Los códigos se centran en la implementación y experimentación de algoritmos de ordenamiento. El programa principal en "orden.cpp" realiza experimentos con varios algoritmos, incluyendo Merge Sort, Quick Sort, Bubble Sort, Insertion Sort y Selection Sort. Los experimentos involucran la creación de arreglos aleatorios, la medición del tiempo de ejecución de cada algoritmo y el cálculo de promedios y desviaciones estándar.
</p>

<p align="justify">
Además, se proporcionan implementaciones de los algoritmos en archivos separados ("ordenamiento_t.h" y "ordenamiento_rec_t.h"). Estos archivos contienen funciones para realizar el ordenamiento utilizando enfoques recursivos en el caso de Merge Sort y Quick Sort, y enfoques iterativos para los otros algoritmos.
</p>

<p align="justify">
En resumen, los códigos permiten analizar y comparar el rendimiento de diferentes algoritmos de ordenamiento mediante experimentos controlados, proporcionando flexibilidad para seleccionar los algoritmos a evaluar y generando información sobre tiempos de ejecución promedio y desviaciones estándar.
</p>



# ANTECEDENTES

<p align="justify">
El problema de ordenamiento se define como sigue:
</p>

<p align="justify">
Entrada: Una secuencia A=〈a1, a2, , an〉 de n números.
</p>

<p align="justify">
Salida: Una permutación A'=〈a'1, a'2, , a'n〉 de los números de la secuencia de A, tal que a'1a'2a'n.
</p>

<p align="justify">
La tarea de ordenar una secuencia de números es fundamental en el procesamiento de datos y ha sido objeto de amplia investigación. En este contexto, se aborda el desafío de diseñar algoritmos eficientes que logren el ordenamiento óptimo de manera rápida y efectiva.
</p>

<p align="justify">
Dentro de la diversidad de enfoques para abordar este problema, se han desarrollado diversos algoritmos de ordenamiento, cada uno con características particulares y rendimientos variables. La distinción entre estos algoritmos radica principalmente en su eficiencia, medida a través del tiempo de ejecución en función del tamaño de la entrada.
</p>

<p align="justify">
En el marco académico, se han estudiado y comparado diferentes algoritmos de ordenamiento. En particular, durante el curso se analizaron cinco algoritmos específicos: insertion sort, selection sort, bubblesort, merge sort y quicksort. Se observó que, en el caso promedio, los algoritmos de insertion sort, selection sort y bubblesort presentan un tiempo de ejecución de orden cuadrático O(n2)mientras que los algoritmos merge sort y quicksort exhiben un rendimiento proporcional a O(n log n).
</p>

<p align="justify">
Esta distinción en la complejidad temporal entre los algoritmos estudiados proporciona un contexto valioso para investigaciones adicionales sobre el rendimiento comparativo de estos enfoques en situaciones específicas, contribuyendo así a una comprensión más profunda de sus ventajas y limitaciones prácticas.
</p>



# ANÁLISIS DEL PROBLEMA

<p align="justify">
En términos generales, los algoritmos de ordenamiento se utilizan para organizar elementos en una secuencia de manera ascendente o descendente. Estos son fundamentales en ciencias de la computación y son aplicados en diversas áreas, como bases de datos, algoritmos de búsqueda, y en general, en cualquier escenario donde se necesite manejar datos de manera eficiente.
</p>

<p align="justify">
El programa orden.cpp consta de dos archivos de encabezado (ordenamiento_t.h y ordenamiento_rec_t.h) que contienen las declaraciones de funciones relacionadas con los algoritmos de ordenamiento. El código principal se encuentra en orden.cpp, donde se implementan funciones para generar arreglos aleatorios, realizar experimentos con diferentes algoritmos de ordenamiento, calcular tiempos promedio y desviaciones estándar.
</p>

<p align="justify">
La función principal main interactúa con el usuario para ingresar parámetros como el tamaño del arreglo, el número de repeticiones y la lista de algoritmos a evaluar. Luego, según las preferencias del usuario, se ejecutan experimentos que generan arreglos aleatorios, los ordenan con los algoritmos seleccionados y registran los tiempos de ejecución. Estos resultados se presentan al final del programa, incluyendo el tiempo promedio y la desviación estándar para cada algoritmo.
</p>

<p align="justify">
Los algoritmos de ordenamiento implementados incluyen merge_sort, quicksort, bubblesort, insertion_sort y selection_sort. Cada uno de estos algoritmos tiene su propia función dedicada para realizar la ordenación en un arreglo dado.
</p>

<p align="justify">
En resumen, el código orden.cpp proporciona una plataforma para comparar y evaluar diferentes algoritmos de ordenamiento mediante la medición de sus tiempos de ejecución y desviaciones estándar, lo que permite a los usuarios comprender y comparar la eficiencia relativa de estos algoritmos en distintos escenarios.
</p>



# IMPLEMENTACIÓN
<ol>
  <li>orden.cpp</li>
  Programa principal que realiza experimentos con algoritmos de ordenamiento. Se incluyen los archivos de encabezado ordenamiento_t.h y ordenamiento_rec_t.h, que contienen las declaraciones de funciones relacionadas con los algoritmos de ordenamiento. Interactúa con el usuario para ingresar parámetros como el tamaño del arreglo, el número de repeticiones y la lista de algoritmos a evaluar. 
  <li>ordenamiento_rec_t.h</li>
  Este archivo contiene las declaraciones de las funciones relacionadas con algoritmos de ordenamiento recursivos, como merge_sort y quicksort. También incluye las funciones auxiliares necesarias para realizar experimentos con estos algoritmos.
  <li>ordenamiento_t.h</li>
  El archivo de encabezado ordenamiento_t.h contiene las declaraciones de las funciones relacionadas con algoritmos de ordenamiento no recursivos, como bubblesort, insertion_sort y selection_sort. Al igual que ordenamiento_rec_t.h, este archivo incluye funciones auxiliares para realizar experimentos con estos algoritmos.
  <li>ordenamiento_rec_t.cpp</li>
  Este archivo de implementación contiene las definiciones de las funciones relacionadas con algoritmos de ordenamiento recursivos. Aquí se encuentran las implementaciones de merge_sort y quicksort. Cabe destacar que estas funciones son utilizadas en el programa principal (orden.cpp) para ordenar los arreglos.
  <li>ordenamiento_t.cpp</li>
  Este archivo de implementación contiene las definiciones de las funciones relacionadas con algoritmos de ordenamiento no recursivos. Aquí se encuentran las implementaciones de bubblesort, insertion_sort y selection_sort. Al igual que ordenamiento_rec_t.cpp, estas funciones son utilizadas en el programa principal (orden.cpp) para ordenar los arreglos.
</ol>



# DESCRIPCIÓN DE LAS FUNCIONES DE ORDENAMIENTO
<ol>
  <li>merge_sort: Ordena un arreglo usando el algoritmo Merge Sort de manera recursiva.</li>
  <li>quicksort: Ordena un arreglo usando el algoritmo Quicksort de manera recursiva.</li>
  <li>bubblesort: Ordena un arreglo usando el algoritmo Bubblesort.</li>
  <li>insertion_sort: Ordena un arreglo usando el algoritmo Insertion Sort.</li>
  <li>selection_sort: Ordena un arreglo usando el algoritmo Selection Sort.</li>
</ol>



# GRÁFICAS DE LOS RESULTADOS INDIVIDUAL

![grafica1](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/546a9814-d928-4bb7-a87e-0cad6605d83f)

![grafica2](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/0be1bf0c-b860-47fc-8731-5bf4ee3a4546)

![grafica3](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/79af6fa3-1b2c-4884-9ff6-45a154ae8ef2)

![grafica4](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/b4fc45d3-2dd0-434d-9112-37748d906b87)

![grafica5](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/c05fd7cd-9836-47e3-9471-5fbdb2c94193)

![grafica6](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/10ef77f9-740f-465b-b8ae-bbdedb463038)

![grafica7](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/2dd855c5-1657-4639-88cb-5cecbc5440d4)

![grafica8](https://github.com/AGN-Teaching/practica-4-algoritmos-de-ordenamiento-daniii2012/assets/125592302/3c11a925-1313-415e-9d1d-55ce5c16919e)



# CONCLUSIONES
