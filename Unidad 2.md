# Estructuras de Datos No Lineales: Grafos y Árboles

<details>
<summary><strong> 📖 Introducción </strong></summary>

El presente portafolio académico tiene como propósito consolidar y exponer los conocimientos adquiridos en el área de las **estructuras de datos**, elementos fundamentales para el diseño de algoritmos eficientes y la resolución de problemas complejos en el desarrollo de software.

Dentro de este ámbito, el estudio de las **estructuras no lineales** cobra una relevancia crítica, ya que permiten modelar relaciones complejas que superan las limitaciones de las estructuras lineales convencionales, como arreglos, listas o pilas.

En este repositorio se presenta una fundamentación teórica de las dos estructuras no lineales más representativas de las Ciencias de la Computación:

- **Grafos**
- **Árboles**

Además, se describen sus definiciones, propiedades y principales clasificaciones, sirviendo como base para el desarrollo de ejercicios y aplicaciones prácticas.

---

</details>

---

<details>
<summary><strong> 🕸️ Definición y Tipología de Grafos </strong></summary>

## ¿Qué es un grafo?

Un grafo es una estructura matemática y de datos que se utiliza para representar relaciones entre elementos. 

**Está compuesto por dos partes fundamentales:**

- Vértices (o Nodos): Los objetos o puntos del sistema.

- Aristas (o Arcos): Las líneas o conexiones que unen a esos puntos.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/5d2c7db6-a6f3-44c5-b670-ee73747f755f" />

Donde:

| Símbolo | Descripción |
|---------|-------------|
| **V** | Conjunto no vacío de vértices o nodos que representan objetos o entidades. |
| **E** | Conjunto de aristas o conexiones que relacionan los vértices. |

---

</details>

---

<details>
<summary><strong> 📌 Clasificación de los Grafos </strong></summary>

Los grafos se pueden clasificar en:

<details>
<summary><strong> 📌 Grafos Dirigidos (Dígrafos) </strong></summary>
  
Las aristas tienen una dirección específica indicada por una flecha. La relación es unidireccional a menos que se indique lo contrario.

```text
(A) ----> (B)
```

La relación únicamente es válida desde el nodo origen hacia el nodo destino.

### Características de los Grafos Dirigidos

* **Relaciones Unidireccionales:** 

* **Grados de Entrada y Salida:** A diferencia de los grafos comunes, en los dirigidos el grado de cada nodo se divide en dos:
  * *Grado de Entrada (In-degree):* 
  * *Grado de Salida (Out-degree):* 

* **Caminos Restringidos (Conectividad):** 

---

</details>

---

<details>
<summary><strong> 📌 Grafos No Dirigidos </strong></summary>

Las aristas no tienen un sentido o dirección definida. La relación es bidireccional por defecto. Si hay una conexión entre $A$ y $B$, se puede viajar en ambos sentidos.


```text
(A) <---> (B)
```

No existe una dirección definida entre los nodos.

### Características de los Grafos No Dirigidos

* **Relaciones Bidireccionales (Simetría):**

* **Grado Único por Vértice:**
  
* **Matriz de Adyacencia Simétrica:** 

Su simplicidad los convierte en una de las estructuras más utilizadas en programación.

---

</details>

---

<details>
<summary><strong> 📌 Grafos Ponderados </strong></summary>

Cada arista tiene un valor numérico asignado llamado peso o costo. Este número puede representar distancias, tiempo, consumo de ancho de banda, etc.

</details>

---

<details>
<summary><strong> 📌 Grafos No Ponderados </strong></summary>

Todas las aristas tienen el mismo valor o simplemente representan la existencia de una conexión (no hay costos asociados).

---

</details>

---

</details>

---

</details>

<details>
<summary><strong> 🌲 Definición y Tipologia de Árboles </strong></summary>

---

<details>
<summary><strong> 🌲QUE ES </strong></summary>

En matemáticas discretas y teoría de grafos, un árbol es un tipo especial de grafo que cumple con dos condiciones fundamentales:

**Es conexo:** Todos los nodos están conectados por al menos un camino.

**Es acíclico:** No contiene ciclos (es decir, no hay caminos cerrados que regresen al mismo nodo sin repetir aristas).

**🌲 Regla de oro: Si un árbol tiene $n$ vértices (nodos), siempre tendrá exactamente $n - 1$ aristas (conexiones).**

</details>

<details>
<summary><strong> 🌲 ESTRUCTURA </strong></summary>

**Su estructura esta formada por:**

- *Raíz (Root): El nodo superior*

- *Padre (Parent): Un nodo que tiene conexiones hacia abajo*

- *Hijo (Child): Un nodo conectado directamente con otro que está en un nivel superior.*

- *Hoja (Leaf): Nodos terminales que no tienen hijos*

- *Nodos Internos: Aquellos que tienen al menos un hijo*

- *Altura: La longitud del camino más largo desde la raíz hasta una hoja.*

</details>

<details>
<summary><strong> 🌲 TIPOS DE ARBOLES </strong></summary>

<details>
<summary><strong> 🌲 Árboles Generales (N-arios) </strong></summary>

Cada nodo puede tener un número indefinido de hijos.

Se utilizan para representar estructuras jerárquicas como:

- Sistemas de archivos
- Organigramas
- Árboles genealógicos

---

</details>

<details>
<summary><strong> 🌲 Árboles Binarios </strong></summary>

Cada nodo puede tener como máximo **dos hijos**:

- Subárbol izquierdo.
- Subárbol derecho.

Su simplicidad los convierte en una de las estructuras más utilizadas en programación.

---

</details>

<details>
<summary><strong> 🌲 Árboles Binarios de Búsqueda (BST) </strong></summary>

Son árboles binarios que mantienen una propiedad de ordenamiento.

Para cualquier nodo:

```text
Izquierda < Nodo < Derecha
```

Gracias a esta característica permiten realizar búsquedas de forma eficiente.

---

</details>

<details>
<summary><strong> 🌲 Árboles AVL </strong></summary>

Los árboles AVL son árboles binarios de búsqueda **auto-balanceados**.

Su principal característica consiste en mantener equilibrada la altura entre sus subárboles.

La diferencia de alturas nunca puede ser mayor que:

```text
1
```

Esto garantiza un rendimiento eficiente en operaciones de:

- Inserción
- Eliminación
- Búsqueda

---

</details>

---

</details>

---

</details>

---

<details>
<summary><strong> 🎯 Objetivo del Portafolio </strong></summary>

El análisis, diseño e implementación de las estructuras de datos no lineales constituye un pilar fundamental en la formación de futuros profesionales de la ingeniería.

Los ejercicios y casos prácticos desarrollados en este portafolio tienen como finalidad demostrar la aplicación de los conceptos teóricos mediante la resolución de problemas reales, fortaleciendo la comprensión de algoritmos y promoviendo el diseño de sistemas de información eficientes y escalables.

---

</details>

---

<details>
<summary><strong> 📂 Actividades del Curso </strong></summary>

En esta sección se encuentran organizadas las actividades desarrolladas durante el curso. Cada apartado contiene un enlace al repositorio correspondiente en Google Drive, donde se almacenan los archivos elaborados en grupo.

---

<details>
<summary><strong> 👨‍🏫 Actividad en Contacto con el Docente (ACD) </strong></summary>

**Descripción**

Actividad desarrollada en conjunto bajo la orientación del docente.

🔗 **Link de la carpeta**

https://drive.google.com/drive/u/1/folders/1Try-_f5gqfEo6DHEY4VUZU3YDRXZQrM6

---

</details>

---

<details>
<summary><strong> 📘 Actividad Autónoma (AA) </strong></summary>

**Descripción**

Actividad colaborativa correspondiente al segundo bloque de aprendizaje autónomo.

🔗 **Acceder a la actividad**

https://drive.google.com/drive/folders/1FTKjoga1fPar5jPmI7mvtN4jazDNtx-W?usp=sharing

---

</details>

---

<details>
<summary><strong> 👨‍🏫 Actividad en Contacto con el Docente (ACD) N.º 2 </strong></summary>

**Descripción**

Actividad desarrollada con el acompañamiento del docente durante el segundo bloque.

🔗 **Acceder a la actividad**

https://drive.google.com/drive/folders/1fLHPF5p1fxefQmgxoGBqdapgsUiNuZpj?usp=drive_link

---

</details>

---

<details>
<summary><strong> 🧩 Aprendizaje Practico Experimental (APE) – Fases 1 a 6 </strong></summary>

**Descripción**

Compilación de las actividades correspondientes al Aprendizaje Práctico Experimental (APE), desarrolladas de forma grupal durante las diferentes fases de la asignatura.

### 📌 Fases 1 – 2

🔗 **Acceder a la actividad**

[📁 Abrir carpeta en Google Drive]

https://drive.google.com/drive/folders/1mo1deKAtf1gYF3m7195UPDQRrAuqDyCK?usp=drive_link

---

### 📌 Fases 3 – 4

🔗 **Acceder a la actividad**

[📁 Abrir carpeta en Google Drive]

https://drive.google.com/drive/folders/15trE6Bz8hx1lusW1h4yWRauZUDlWxXiM?usp=drive_link

---

### 📌 Fases 5 – 6

🔗 **Acceder a la actividad**

[📁 Abrir carpeta en Google Drive]:

https://drive.google.com/drive/folders/1t2UE3WtD2waEuCsTohqOyTD2nAUAjpmT?usp=drive_link

---

</details>
