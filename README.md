# TALLER_05
Implementar y comparar tres algoritmos de ordenación in-place sobre arreglos pequeños, y validar su funcionamiento con trazas y casos de prueba reproducibles.

**Autores:**

* Soledad Buri
* Gyna Yupanqui 

--- 
# Decisiones de Diseño 

* **Clases de Utilidad:** Se implementaron InsertionSort, SelectionSort y BubbleSort como clases finales con métodos estáticos, ya que no es necesario crear objetos  de ellas para ordenar un arreglo. 
* **Trazas Opcionales:** Se añadió un parámetro boolean trace en cada método sort. Esto permite usar el algoritmo de forma "silenciosa".
* **Manejo de Datos:** En la clase principal SortingDemo, se uso el método .clone() antes de enviar los arreglos a ordenar lo que asegura que el arreglo original nunca se modifique, permitiendo reutilizar los datos de prueba para los diferentes algoritmos sin interferencias.

----

# Modo de ejecución 

**Modo 1**
1. Buscar la carpeta src/ed/u2/sorting/
2. Compilar 
3. Ejecutar (Se mostrata en la salida los casos requeridos)

**Modo 2**
1. Clonar el repositorio
2. Abirir en un IDE
3. Ejecutar **SortingDemo**
4. Se mostrara en consola los algoritmos de ordenación requeridos

---
##  Casos Borde 
* **Arreglos Nulos:** Se incluyó una validación inicial (if (a == null) return;) en todos los algoritmos para evitar errores de tipo NullPointerException si se recibieran datos vacíos.
* **Arreglos Ya Ordenados:** Se probó específicamente BubbleSort con un arreglo ordenado ([1, 2, 3, 4, 5]) para verificar que la optimización de "corte temprano" detuviera el algoritmo en la primera pasada.
* **Elementos Duplicados:** Se realizaron pruebas con arreglos como [2, 2, 2, 2] para confirmar que los algoritmos no entran en bucles infinitos y manejan correctamente la igualdad de valores.

