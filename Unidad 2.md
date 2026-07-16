# Métodos de Simplificación de Expresiones Lógicas

<details>
<summary><strong> 📖 Introducción </strong></summary>

El propósito de este portafolio académico es consolidar y presentar los conocimientos clave adquiridos en el **diseño de circuitos digitales**, enfocándome en los métodos esenciales para simplificar expresiones lógicas. Dominar estos procedimientos es clave para cualquier estudiante de computación, ya que nos permite diseñar sistemas mucho más eficientes al reducir al mínimo el número de compuertas lógicas necesarias para construir una función booleana.

En el ámbito de la electrónica digital y la arquitectura de computadoras, la simplificación lógica es un pilar fundamental. Gracias a ella, no solo logramos optimizar el diseño de los circuitos, sino que también reducimos los costos de hardware y mejoramos significativamente el rendimiento de los sistemas.

En este repositorio encontrarás la base teórica y práctica de los dos métodos de optimización más utilizados:

- **Álgebra Booleana** (simplificación algebraica usando leyes y axiomas).
- **Mapas de Karnaugh** (simplificación visual y sistemática).

Además de sus definiciones y principios fundamentales, se detallan sus propiedades y aplicaciones reales en la creación de circuitos digitales.

</details>

---

<details>
<summary><strong> 🧮 Simplificación mediante Álgebra Booleana </strong></summary>

## ¿Qué es el Álgebra Booleana?

Es un sistema matemático que se utiliza para simplificar y analizar circuitos lógicos (digitales). A diferencia del álgebra común (donde usas números reales), en el Álgebra Booleana las variables solo pueden tener dos valores posibles: **Verdadero (1)** o **Falso (0)**.

Sus operaciones fundamentales equivalen a las compuertas lógicas básicas en electrónica:

* **Suma lógica (OR):** Representada por el signo más (`+`). Equivale a la disyunción ($p \vee q$).
* **Producto lógico (AND):** Representado por un punto (`·`) o simplemente uniendo las variables. Equivale a la conjunción ($p \wedge q$).
* **Negación (NOT):** Representada por una barra superior ($\bar{A}$) o un apóstrofe ($A'$). Invierte el valor del bit.


</details>

---

<details>
<summary><strong> 📌 Principales Leyes  </strong></summary>

## Leyes Principales del Álgebra Booleana

Estas leyes son las reglas algebraicas que nos permiten simplificar expresiones complejas para diseñar circuitos con la menor cantidad de compuertas posibles.

| Ley | Suma (OR) | Producto (AND) | Descripción |
| :--- | :---: | :---: | :--- |
| **Identidad** | $A + 0 = A$ | $A \cdot 1 = A$ | Operar con el elemento neutro no altera la variable. |
| **Nulo (Acotación)** | $A + 1 = 1$ | $A \cdot 0 = 0$ | El $1$ domina en la suma y el $0$ en el producto. |
| **Idempotencia** | $A + A = A$ | $A \cdot A = A$ | Operar una variable consigo misma da la misma variable. |
| **Inverso (Complemento)** | $A + \bar{A} = 1$ | $A \cdot \bar{A} = 0$ | Una variable operada con su negación. |
| **Doble Negación** | $\bar{\bar{A}} = A$ | - | Negar dos veces una variable la deja en su estado original. |
| **Conmutativa** | $A + B = B + A$ | $A \cdot B = B \cdot A$ | El orden de los factores no altera el resultado. |
| **Asociativa** | $A + (B + C) = (A + B) + C$ | $A \cdot (B \cdot C) = (A \cdot B) \cdot C$ | El agrupamiento no altera el resultado. |
| **Distributiva** | $A \cdot (B + C) = (A \cdot B) + (A \cdot C)$ | $A + (B \cdot C) = (A + B) \cdot (A + C)$ | Distribuye una operación sobre la otra. |
| **Absorción** | $A + (A \cdot B) = A$ | $A \cdot (A + B) = A$ | Simplifica términos redundantes de forma directa. |
| **Leyes de De Morgan** | $\overline{A + B} = \bar{A} \cdot \bar{B}$ | $\overline{A \cdot B} = \bar{A} + \bar{B}$ | Permite cambiar una suma negada por un producto de negados, y viceversa. |

</details>

---

<details>
<summary><strong> 🗺️ Simplificacion de Mapas de Karnaugh </strong></summary>

---

<details>
<summary><strong> 🗺️ QUE ES </strong></summary>

Un **Mapa de Karnaugh** es un método gráfico utilizado para simplificar funciones booleanas de forma visual y sistemática. A diferencia del álgebra booleana tradicional, este método reduce la probabilidad de cometer errores algebraicos al agrupar celdas adyacentes.

---

</details>

<details>
<summary><strong> 🗺️ ESTRUCTURA </strong></summary>

* **Estructura:** Consiste en una cuadrícula (tabla de dos dimensiones) donde cada celda representa un minitérmino (combinación de las variables de entrada). 

* **Código Gray:** Las filas y columnas se ordenan siguiendo el código Gray (donde solo cambia un bit a la vez entre celdas consecutivas, por ejemplo: `00`, `01`, `11`, `10`). Esto asegura la adyacencia física y lógica.

---

</details>

<details>
<summary><strong> 🗺️ Simplificación </strong></summary>
  
## Simplificación con Mapas de Karnaugh

Para simplificar una función usando este método, se siguen estos pasos fundamentales:

1. **Llenar el Mapa:** Se coloca un **1** en las celdas correspondientes a las combinaciones donde la función de salida es verdadera, y un **0** (o se deja vacío) en las demás.
2. **Agrupar los Unos (Leyes de Agrupación):** * Se deben crear grupos con potencias de 2 (grupos de 1, 2, 4, 8 o 16 elementos).
   * Los grupos deben ser lo más grandes posibles.
   * Se permite el solapamiento (un **1** puede pertenecer a más de un grupo si eso ayuda a agrandar otro grupo).
   * El mapa es "esférico": los extremos izquierdo-derecho y superior-inferior son adyacentes y se pueden agrupar.
3. **Eliminar Variables:** Para cada grupo, se observan las variables de entrada:
   * Si una variable cambia de valor dentro del grupo (pasa de 0 a 1 o viceversa), **se elimina**.
   * Si una variable mantiene su valor constante, **se conserva** (si se mantiene en 1 se escribe normal, si se mantiene en 0 se escribe negada).
4. **Obtener la Función Simplificada:** Se realiza la suma (OR) de los términos resultantes de cada grupo.

---

</details>

<details>
<summary><strong> 🗺️ Clasificación </strong></summary>

## Clasificación de los Mapas de Karnaugh

Los mapas de Karnaugh se clasifican principalmente según el **número de variables de entrada** de la función lógica que se desea simplificar. A mayor número de variables, mayor es la cantidad de celdas en la cuadrícula ($2^n$ celdas, donde $n$ es el número de variables):

* **Mapa de 2 Variables:** 
  * Consta de **4 celdas** ($2^2$).
  * Ideal para funciones muy sencillas con entradas como $A$ y $B$.
* **Mapa de 3 Variables:** 
  * Consta de **8 celdas** ($2^3$), organizadas usualmente en una cuadrícula de $2 \times 4$.
  * Permite mapear entradas como $A$, $B$ y $C$.
* **Mapa de 4 Variables:** 
  * Consta de **16 celdas** ($2^4$), distribuidas en una cuadrícula simétrica de $4 \times 4$.
  * Es el más utilizado en ejercicios académicos de diseño de circuitos digitales (entradas $A$, $B$, $C$ y $D$).
* **Mapa de 5 Variables:** 
  * Consta de **32 celdas** ($2^5$).
  * Se suele trabajar de forma tridimensional, utilizando dos mapas contiguos de 16 celdas superpuestos lógicamente para analizar la adyacencia espacial.

</details>


</details>

---

<details>
<summary><strong> ⚙️ Tabla Comparativa: Álgebra Booleana vs. Mapas de Karnaugh </strong></summary>

| Criterio | Álgebra Booleana | Mapas de Karnaugh (K-Maps) |
| :--- | :--- | :--- |
| **Enfoque** | Método puramente analítico y matemático. | Método gráfico, visual y sistemático. |
| **Complejidad de Uso** | Requiere memorizar y aplicar correctamente muchas leyes lógicas. | Requiere seguir un conjunto de reglas visuales de agrupación de celdas. |
| **Facilidad de Error** | Alta. Es fácil equivocarse en un paso algebraico o no ver una simplificación posible. | Baja. Al ser un método visual y estructurado, la posibilidad de error es mínima. |
| **Número de Variables** | No tiene un límite teórico (funciona con cualquier número de variables). | Ideal para $2$, $3$ o $4$ variables. Con $5$ o más variables se vuelve muy complejo de visualizar. |
| **Resultado obtenido** | No siempre garantiza llegar a la forma más simplificada si se pasa por alto alguna ley. | Siempre garantiza obtener la expresión más simplificada posible (Suma de Productos mínima). |
| **Tiempo de Resolución** | Puede ser lento y tedioso para funciones muy largas. | Muy rápido y mecánico una vez que se domina la técnica de agrupación. |


</details>

</details>

</details>

</details>

---

<details>
<summary><strong> 🎯 Objetivo del Portafolio </strong></summary>

El estudio de los métodos de simplificación de expresiones lógicas constituye una parte esencial en la formación de los futuros profesionales de la ingeniería, ya que proporciona las herramientas matemáticas necesarias para optimizar funciones lógicas y diseñar circuitos digitales más eficientes, reduciendo la complejidad del software y optimizando el uso de recursos de hardware.

Los ejercicios y casos prácticos desarrollados en este portafolio tienen como finalidad demostrar la aplicación de los conceptos teóricos mediante la resolución de problemas paso a paso, fortaleciendo la comprensión de las Leyes de Equivalencia Lógica, el Álgebra de Boole y los Mapas de Karnaugh como herramientas fundamentales para el análisis y diseño de sistemas lógicos.

</details>

---

<details>
<summary><strong> 📂 Actividades del Curso </strong></summary>

En esta sección se encuentran organizadas las actividades desarrolladas durante el curso. Cada apartado contiene un enlace al repositorio correspondiente en Google Drive, donde se almacenan los archivos elaborados en grupo.

---

<details>
<summary><strong> 📘 Actividad Autónoma (AA) </strong></summary>

**Descripción**

Actividad colaborativa correspondiente al segundo bloque de aprendizaje autónomo.

🔗 **Link para la actividad**

https://drive.google.com/drive/folders/1FTKjoga1fPar5jPmI7mvtN4jazDNtx-W?usp=drive_link


</details>

---

<details>
<summary><strong> 👨‍🏫 Actividad en Contacto con el Docente (ACD) </strong></summary>

**Descripción**

Actividad desarrollada con el acompañamiento del docente durante el segundo bloque.

🔗 **Link para la actividad**

https://drive.google.com/drive/folders/1fLHPF5p1fxefQmgxoGBqdapgsUiNuZpj?usp=drive_link

</details>

---

<details>
<summary><strong> 🧩 Aprendizaje Practico Experimental (APE) – Fases 1 a 6 </strong></summary>

**Descripción**

Compilación de las actividades correspondientes al Aprendizaje Práctico Experimental (APE), desarrolladas de forma grupal durante las diferentes fases de la asignatura.

### 📌 Fases 1 – 2

[📁 Link para la carpeta en Google Drive]

https://drive.google.com/drive/folders/1mo1deKAtf1gYF3m7195UPDQRrAuqDyCK?usp=drive_link

---

### 📌 Fases 3 – 4

[📁 Link para la carpeta en Google Drive]

https://drive.google.com/drive/folders/15trE6Bz8hx1lusW1h4yWRauZUDlWxXiM?usp=drive_link

---

### 📌 Fases 5 – 6

[📁 Link para la carpeta en Google Drive]:

https://drive.google.com/drive/folders/1t2UE3WtD2waEuCsTohqOyTD2nAUAjpmT?usp=drive_link

---

</details>
