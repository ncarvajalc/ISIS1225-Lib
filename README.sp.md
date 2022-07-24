# DISCLib
<!-- based on the repo from 
https://github.com/othneildrew/Best-README-Template

<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

**DISCLib** es una librería Python no orientada a objetos para enseñar los conceptos de estructuras de datos y algoritmos en la Universidad de los Andes, desarrollada por los profesores y personal de la Facultad de Ingeniería, Departamento de Sistemas e Ingeniería Informática #DISC.

[Ver Demo y Ejemplos][demo-url] · [Informar Errores][bugs-url] · [Solicitar Funcionalidad][issues-url]

<!-- PROJECT CONTENT -->
**Tabla de contenido (actualizada)**
- [DISCLib](#disclib)
  - [Acerca del Proyecto](#acerca-del-proyecto)
    - [Estructura](#estructura)
    - [Implementación](#implementación)
  - [Introducción](#introducción)
    - [Prerrequisitos](#prerrequisitos)
    - [Instalación](#instalación)
  - [Uso](#uso)
  - [Contacto y Soporte] (#contacto-y-soporte)
  - [Hoja de Ruta](#hoja-de-ruta)
  - [Contribuir](#contribuir)
  - [Licencia](#licencia)
  - [Autores y Reconocimiento](#autores-y-reconocimiento)

<!-- ABOUT THE PROJECT -->
## Acerca del Proyecto

Este proyecto se creó como una librería pedagógica para enseñar a los estudiantes de pregrado de la facultad de Ingenieria y en particular del programa de Ingeniería en Sistemas e Informática de la Universidad de los Andes para usar y entender las estructuras de datos y sus algoritmos relacionados. Esto incluye estructuras tales como los arreglos, las listas, los mapas, los mapas ordenados, los árboles de búsqueda binarios (BST), árboles rojos negros (RBT) y los grafos.

**IMPORTANTE** Este es un trabajo en progreso. El proyecto se centra principalmente como una herramienta pedagógica para estudiantes universitarios y no está destinado a ser utilizado como una biblioteca completamente funcional.

[Volver al inicio](#disclib)

### Estructura
<!-- #TODO to translate -->
TRABAJANDO!
<!-- 
The project is divided into four main parts:

1. [DISClib](./DISClib) Root folder with the library implementation.

    1. [ADT](./DISClib/ADT) Folder with the main Abstract Data Types (ADT) implemented in the library.
        1. [List](./DISClib/ADT/list.py) Script implementing the ADT Lists in the library, configurable by Array List, Single Linked List and Double Linked List structures.
        2. [Queue](./DISClib/ADT/queue.py) Script implementing the ADT queue based in the ADT List.
        3. [Stack](./DISClib/ADT/stack.py) Script implementing the ADT stack based in the ADT List.
        4. [Map](./DISClib/ADT/map.py) Script implementing the ADT Map using Hash Tables as data structures, configurable by collision handling method to Linear Probing and Separate Chaining.
        5. [Ordered Map](./DISClib/ADT/orderedmap.py) Script implementing the ADT Ordered Maps using binary trees as data structures, configurable to Binary Search Trees (BST) and Red Black Tree (RBT).
        6. [MinPQ](./DISClib/ADT/minpq.py) Script implementing the ADT Min Priority Queue using heap data structures.
        7. [Indexed MinPQ](./DISClib/ADT/indexminpq.py) Script implementing the ADT Indexed Min Priority Queue using heap data structures.
        8. [Graph](./DISClib/ADT/graph.py) Script implementing the ADT Graph using adjacency lists as data structures.

    2. [Algorithms](./DISClib/Algorithms) Folder with the main algorithms implemented to handle the ADTs.
        1. [Graphs](./DISClib/Algorithms/Graphs) Folder with the algorithms to handle the ADT Graph.
            1. [DFS](./DISClib/Algorithms/Graphs/dfs.py) Script implementing the Depth First Search (DFS) algorithm.
            2. [BFS](./DISClib/Algorithms/Graphs/bfs.py) Script implementing the Breath First Search (BFS) algorithm.
            3. [DFO](./DISClib/Algorithms/Graphs/dfo.py) Script implementing the Depth First Order (DFO) topological sorting algorithm.
            4. [Cycles](./DISClib/Algorithms/Graphs/cycles.py) Script implementing the Cycle Detection algorithm.
            5. [SCC](./DISClib/Algorithms/Graphs/scc.py) Script implementing the Strongly Connected Components (SCC) algorithm.
            6. [Prim](./DISClib/Algorithms/Graphs/prim.py) Script implementing the Prim's algorithm.
            7. [Dijkstra](./DISClib/Algorithms/Graphs/dijkstra.py) Script implementing the Dijkstra's algorithm.
            8. [Bellman-Ford](./DISClib/Algorithms/Graphs/bellmanford.py) Script implementing the Bellman-Ford algorithm.
        2. [Sorting](./DISClib/Algorithms/Sorting) Folder with the algorithms implementing sorting for the ADT List.
            1. [Selection Sort](./DISClib/Algorithms/Sorting/selectionsort.py) Script implementing the Selection Sort algorithm.
            2. [Insertion Sort](./DISClib/Algorithms/Sorting/insertionsort.py) Script implementing the Insertion Sort algorithm.
            3. [Shell Sort](./DISClib/Algorithms/Sorting/shellsort.py) Script implementing the Shell Sort algorithm.
            4. [Merge Sort](./DISClib/Algorithms/Sorting/mergesort.py) Script implementing the Merge Sort algorithm.
            5. [Quick Sort](./DISClib/Algorithms/Sorting/quicksort.py) Script implementing the Quick Sort algorithm.
        3. [Trees](./DISClib/Algorithms/Trees) Folder with the algorithms to handle the ADT Trees.
            1. [Traversal](./DISClib/Algorithms/Trees/traversal.py) Script implementing the Transversal algorithm for binary trees, it includes the preorder, inorder and postorder structure walkthrough.

    3. [Data Structures](./DISClib/DataStructures) Folder with the main data structures implemented to support the ADTs in the library.
        1. [Array List](./DISClib/DataStructures/arraylist.py) Script implementing the Array List data structure.
        2. [Single Linked List](./DISClib/DataStructures/singlelinkedlist.py) Script implementing the Single Linked List data structure.
        3. [Double Linked List](./DISClib/DataStructures/doublelinkedlist.py) Script implementing the Double Linked List data structure.
        4. [Heap](./DISClib/DataStructures/heap.py) Script implementing the Heap data structure.
        5. [Indexed Heap](./DISClib/DataStructures/indexheap.py) Script implementing the Indexed Heap data structure.
        6. [Indexed MinPQ Node](./DISClib/DataStructures/iminpqnode.py) Script implementing the Indexed MinPQ Node data structure to support the Indexed Heap implementation.
        7. [Separate Chaining Hash Table](./DISClib/DataStructures/chaininghashtable.py) Script implementing the Separate Chaining Hash Table data structure.
        8. [Linear Probing Hash Table](./DISClib/DataStructures/probehashtable.py) Script implementing the Linear Probing Hash Table data structure.
        9. [Map Entry](./DISClib/DataStructures/mapentry.py) Script implementing the Map Entry data structure to support the Hash Table implementation.
        10. [Binary Searhc Tree (BST)](./DISClib/DataStructures/bst.py) Script implementing the Binary Search Tree (BST) data structure for the ADT Ordered Map.
        11. [BST Node](./DISClib/DataStructures/bstnode.py) Script implementing the BST Node data structure to support the Binary Search Tree (BST) implementation.
        12. [Red Black Tree (RBT)](./DISClib/DataStructures/rbt.py) Script implementing the Red Black Tree (RBT) data structure for the ADT Ordered Map.
        13. [RBT Node](./DISClib/DataStructures/rbtnode.py) Script implementing the RBT Node data structure to support the Red Black Tree (RBT) implementation.
        14. [Adjacency List](./DISClib/DataStructures/adjlist.py) Script implementing the Adjacency List data structure for ADT Graph.
        15. [Edge](./DISClib/DataStructures/edge.py) Script implementing the Edge data structure to support the Graph's Adjacency List implementation.

    4. [Utils](./DISClib/Utils) Folder with the main utilities implemented to support the ADTs in the library.
        1. [Error Handling](./DISClib/Utils/error.py) Script implementing the Error Handling utility for all the libraries.

2. [Test](./Test) Folder with the tests for the library.
    1. [List](./Test/list) Scripts to test the ADT Lists.
    2. [Queue](./Test/queue) Scripts to test the ADT Queue.
    3. [Stack](./Test/stack) Scripts to test the ADT Stack.
    4. [Map](./Test/map) Scripts to test the ADT Map.
    5. [Ordered Map](./Test/orderedmap) Scripts to test the ADT Ordered Map.
    6. [Binary Search Tree](./Test/bst) Scripts to test the ADT Binary Search Tree.
    7. [MinPQ](./Test/minpq) Scripts to test the ADT Min Priority Queue.
    8. [Graph](./Test/graph) Scripts to test the ADT Graph.

**NOTE:** the `config.py` scripts in the API are used to configure library's  build path and allows the Python interpreter to find the relative path in any condition. -->

[Volver al inicio](#disclib)

### Implementación

Esta librería fue implementada con las siguientes tecnologías:
  * `Mac OS` y `Windows 10` para el sistema operativo.
  * `VS Code` para el IDE.
  * `Python 3.6` para el lenguaje de programación.
  * `Pytest` para librería de pruebas.

Como principio de diseño **DISClib** minimiza en su implementación el uso de librerías externas Python.

Finalmente, **DISClib** funciona entre las versiones `Python 3.6` y `Python 3.9`.

[Volver al inicio](#disclib)

<!-- GETTING STARTED -->
## Introducción

Esta sección contiene los pasos para comenzar a utilizar la librería. Como es el caso de cualquier otra librería, debe instalarla y luego importarla manualmente en su proyecto.

Como la librería no está orientada a objetos, debe importar la biblioteca del proyecto como un módulo siguiendo los pasos de [Instalación](#instalación).

[Volver al inicio](#disclib)

### Prerrequisitos

Como principio de diseño **DISClib** minimiza el uso de librerías externas de Python en su implementación.

Para ejecutar las pruebas en la carpeta 'Test', debe instalar el paquete 'Pytest'.

  ```bash
  pip install pytest
  ```

[Volver al inicio](#disclib)

### Instalación

Por el momento, la librería **DISClib** está disponible como una dependencia local para su proyecto. Para instalarlo y usarlo debe seguir los siguientes pasos:

1. Cree una nueva carpeta de proyecto.
2. Clone el repositorio con el comando:

   ```sh
   git clone https://github.com/ISIS1225DEVS/ISIS1225-Lib.git
   ```

3. Mueva la carpeta **DISClib** a la carpeta del proyecto.
4. Cree un nuevo archivo Python en la carpeta del proyecto.
5. Importe los módulos ADT **DISClib** necesarios en su proyecto con las lineas de codigo:

   ```python
    from DISClib.ADT import list as lt
    from DISClib.ADT import map as mp
   ```

6. ¡Empieza a programar!

[Volver al inicio](#disclib)

<!-- USAGE EXAMPLES -->
## Uso

**DISCLib** es una librería que proporciona un conjunto de ADT para ayudar a implementar y usar estructuras de datos y algoritmos. Su intención es ser una herramienta de enseñanza en el curso [ISIS1225-Estructuras de Datos y Algoritmos][uniandes-url].

Para consultar el uso de la librería puede ver los repositorios de los laboratorios, en los siguientes enlaces:

  * [ISIS1225-SampleMVC][sample-mvc-url] Laboratorio introductorio al patrón MVC.
  * [ISIS1225-SampleConflicts][sample-conflicts-url] Laboratorio para solucionar conflictos de GitHub.
  * [ISIS1225-SampleList][sample-list-url] Laboratorio introductorio al ADT listas.
  * [ISIS1225-SampleSorts][sample-sort-url] Laboratorio para algoritmos de ordenamiento para ADT listas.
  * [ISIS1225-sampleMap][sample-map-url] Laboratorio introductorio de ADT mapas.
  * [ISIS1225-SampleCollision][sample-collision-url] Laboratorio para manejo de colisiones de ADT mapas.
  * [ISIS1225-SampleTree][sample-tree-url] Laboratorio introductorio de los Mapas Ordenados (BST and RBT).
  * [ISIS1225-sampleGraph][sample-graph-url] Laboratorio intorductorio para ADT Grafos.
  * [ISIS1225-SampleAlgorithm][sample-algorithm-url] Laboratorio para algoritmos usados en el ADT Grafos

[Volver al inicio](#disclib)

<!-- CONTACT -->
## Contacto y Soporte

Para más información y contactarnos, utilice los siguientes enlaces:

  * Repositorio Oficial [DISClib][disclib-url].
  * Repositorio para [Demo y Ejemplos][demo-url].
  
Si necesita más información, póngase en contacto con nosotros [en este correo](mailto:isis1225@uniandes.edu.co)


[Volver al inicio](#disclib)

<!-- ROADMAP -->
## Hoja de Ruta
<!-- #TODO to translate -->
TRABAJANDO!
<!-- 
The Road so far lead us to complete the following features:

* [ ] To include examples for all modules in the repository [Demo y Ejemplos][demo-url].
* [ ] To clean some code and make it more readable.
* [ ] To standarize the functions and variables names throughout the library.
* [ ] To improve the library the documentation.
* [ ] To implement the Adjacency Matrix data structure for the ADT Graph.

See the [open issues](https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues) for a full list of proposed features (and known issues). -->

[Volver al inicio](#disclib)

<!-- CONTRIBUTING -->
## Contribuir
<!-- #TODO to translate -->
TRABAJANDO!

<!-- 
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request -->

[Volver al inicio](#disclib)

<!-- LICENSE -->
## Licencia
<!-- #TODO to translate -->
TRABAJANDO!

<!-- Copyright 2020, Departamento de sistemas y Computación, Universidad de Los Andes.
Developed for the class _"ISIS1225 - Estructuras de Datos y Algoritmos"_ or _"ISIS1225 - Data Structure and Algorithms"_ in english.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU General Public License](LICENSE) for more information go to [GNU ORG][gnu-url]. -->

[Volver al inicio](#disclib)

<!-- ACKNOWLEDGMENTS -->
## Autores y Reconocimiento
<!-- #TODO to translate -->
TRABAJANDO!

<!-- * [Dario Correal][dariocorreal-url] is the original author and main developer of the library.
* [Santiago Arteaga][phillipus85-url] is a contributor and repository administrator. 
* [Luis Florez][le99-url] is a contributor and developed examples and tutorials for the library. -->

[Volver al inicio](#disclib)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/ISIS1225DEVS/ISIS1225-Lib.svg?style=for-the-badge
[contributors-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ISIS1225DEVS/ISIS1225-Lib.svg?style=for-the-badge
[forks-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/network/members
[stars-shield]: https://img.shields.io/github/stars/ISIS1225DEVS/ISIS1225-Lib.svg?style=for-the-badge
[stars-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/stargazers
[issues-shield]: https://img.shields.io/github/issues/ISIS1225DEVS/ISIS1225-Lib.svg?style=for-the-badge
[issues-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues
[license-shield]: https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge
[license-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/blob/master/LICENSE
<!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png -->
[uniandes-url]: https://cursos.virtual.uniandes.edu.co/isis1225/
[organization-url]: https://github.com/ISIS1225DEVS/
[disclib-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib
[demo-url]: https://github.com/ISIS1225DEVS/ISIS1225-Examples
[bugs-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues
[issues-url]: https://github.com/ISIS1225DEVS/ISIS1225-Lib/issues
[gnu-url]: http://www.gnu.org/licenses/
<!-- contributors  -->
[dariocorreal-url]: https://github.com/dariocorreal
[phillipus85-url]: https://github.com/phillipus85
[le99-url]: https://github.com/le99
<!-- EDA lab repository -->
[sample-mvc-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleMVC
[sample-conflicts-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleConflicts
[sample-list-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleList
[sample-sort-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleSorts
[sample-map-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleMap
[sample-collision-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleCollision
[sample-tree-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleTree
[sample-graph-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleGraph
[sample-algorithm-url]: https://github.com/ISIS1225DEVS/ISIS1225-SampleAlgorithm