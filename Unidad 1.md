#  Lógica

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
<summary><strong>  Definición y Clasificacion de una Proposición </strong></summary>

## ¿Qué es una Proposición?

En lógica matemática, una **proposición** es una oración declarativa (un enunciado) de la cual se puede afirmar, de manera inequívoca, si es **verdadera (V)** o **falsa (F)**, pero nunca ambas cosas a la vez. El valor de verdad de una proposición no depende de interpretaciones o dudas.

### Ejemplos Claros:
* **Es proposición:** *"Hoy es lunes"* (puede ser verdadero o falso).
* **Es proposición:** *"El número 10 es par"* (es verdadero).
* **NO es proposición:** *"¡Qué calor hace!"* (es una exclamación, no afirma nada con un valor de verdad).
* **NO es proposición:** *"¿Cómo te llamas?"* (es una pregunta).

---

## Clasificación de las Proposiciones

Las proposiciones se dividen en dos tipos según su estructura:

* **Proposiciones Simples (Atómicas):** Son aquellas que expresan una sola idea de forma directa y no contienen conectores lógicos. 
  * *Ejemplo:* "La Tierra es un planeta." (Se representa típicamente con variables como $p$, $q$, $r$).
* **Proposiciones Compuestas (Moleculares):** Son aquellas que se forman al unir dos o más proposiciones simples utilizando conectores lógicos (como "y", "o", "si... entonces"). Su valor de verdad depende de los valores de las proposiciones simples que la componen.
  * *Ejemplo:* "La Tierra es un planeta **y** gira alrededor del Sol." (Representado simbólicamente como $p \wedge q$).

</details>

---

<details>
<summary><strong> 📌 Conectores Lógicos </strong></summary>

## Conectores Lógicos y Tablas de Verdad

Los **conectores lógicos** son operadores que nos permiten unir proposiciones simples para formar proposiciones compuestas. Su comportamiento matemático se define mediante las siguientes reglas:

| Conector Lógico | Operación | Símbolo | Lectura Común | Regla de Oro (Valor de Verdad) |
| :--- | :--- | :---: | :---: | :--- |
| **Negación** | NOT | $\sim$ o $\neg$ | "No..." | Invierte el valor de verdad original (si es $V$ pasa a $F$, y viceversa). |
| **Conjunción** | AND | $\wedge$ | "... y ..." | Solo es **Verdadero** si **ambas** proposiciones son verdaderas. |
| **Disyunción Inclusiva** | OR | $\vee$ | "... o ..." | Solo es **Falso** si **ambas** proposiciones son falsas. |
| **Condicional** | Implicación | $\rightarrow$ | "Si..., entonces..." | Solo es **Falso** cuando el antecedente es **Verdadero** y el consecuente es **Falso** ($V \rightarrow F$). |
| **Bicondicional** | Equivalencia | $\leftrightarrow$ | "... si y solo si ..." | Es **Verdadero** únicamente cuando ambos lados tienen el **mismo** valor de verdad ($V \leftrightarrow V$ o $F \leftrightarrow F$). |
| **Disyunción Exclusiva** | XOR | $\underline{\vee}$ o $\oplus$ | "O bien... o bien..." | Es **Verdadero** solo cuando los valores de verdad son **diferentes** ($V \oplus F$ o $F \oplus V$). |


</details>

---

<details>
<summary><strong>  Tablas de Verdad </strong></summary>


## Tablas de Verdad

Una **tabla de verdad** es una representación gráfica y matemática que muestra todos los posibles escenarios de verdad para una proposición compuesta, analizando cada combinación de valores de sus variables de entrada.

### ¿Cómo se construye una tabla de verdad?

1. **Determinar el número de filas:** Se calcula con la fórmula $2^n$, donde $n$ es el número de proposiciones simples (variables).
   * Con **2 variables** ($p, q$): $2^2 = 4$ filas.
   * Con **3 variables** ($p, q, r$): $2^3 = 8$ filas.
2. **Distribuir los valores:** En la primera columna se alternan las mitades (ej. para 4 filas: 2 verdaderas y 2 falsas); en la siguiente columna se reduce a la mitad (1 verdadera y 1 falsa), y así sucesivamente.
3. **Resolver por jerarquía:** Se operan primero los paréntesis más internos, luego los corchetes y finalmente el operador principal de la expresión.

---

## Clasificación de las Tablas de Verdad

Una vez resuelta la tabla, el resultado obtenido en la columna del operador principal determina su tipo:

* **Tautología:** Se presenta cuando **todos los resultados** de la última columna son **Verdaderos ($V$)**, sin importar los valores individuales de las variables de entrada. Representa una verdad lógica absoluta.
* **Contradicción (Falsa):** Se presenta cuando **todos los resultados** de la última columna son **Falsos ($F$)**. Representa un absurdo o imposibilidad lógica.
* **Contingencia:** Se presenta cuando en el resultado final hay una **mezcla de valores Verdaderos ($V$) y Falsos ($F$)**. Indica que el valor de verdad final depende directamente de las circunstancias de las variables de entrada.

## Tabla de Verdad de Lógica Proposicional

### 1. Negación
| $p$ | $\sim p$ |
| :---: | :---: |
| V | F |
| F | V |

---

### 2. Conjunción (Y)
| $p$ | $q$ | $p \wedge q$ |
| :---: | :---: | :---: |
| V | V | **V** |
| V | F | F |
| F | V | F |
| F | F | F |

---

### 3. Disyunción (O)
| $p$ | $q$ | $p \vee q$ |
| :---: | :---: | :---: |
| V | V | V |
| V | F | V |
| F | V | V |
| F | F | **F** |

---

### 4. Disyunción Exclusiva
| $p$ | $q$ | $p \ \underline{\vee} \ q$ |
| :---: | :---: | :---: |
| V | V | F |
| V | F | V |
| F | V | V |
| F | F | F |

---

### 5. Condicional
| $p$ | $q$ | $p \rightarrow q$ |
| :---: | :---: | :---: |
| V | V | V |
| V | F | **F** |
| F | V | V |
| F | F | V |

---

### 6. Bicondicional
| $p$ | $q$ | $p \leftrightarrow q$ |
| :---: | :---: | :---: |
| V | V | **V** |
| V | F | F |
| F | V | F |
| F | F | **V** |

</details>

---

<details>
<summary><strong> Principales Leyes Lógicas </strong></summary>

Las **leyes lógicas** (o equivalencias notables) son reglas formales que nos permiten simplificar proposiciones compuestas complejas sin necesidad de construir una tabla de verdad completa. Son el equivalente directo a las leyes del álgebra común.

| Nombre de la Ley | Equivalencia en Conjunción ($\wedge$) | Equivalencia en Disyunción ($\vee$) |
| :--- | :---: | :---: |
| **Idempotencia** | $p \wedge p \equiv p$ | $p \vee p \equiv p$ |
| **Conmutativa** | $p \wedge q \equiv q \wedge p$ | $p \vee q \equiv q \vee p$ |
| **Asociativa** | $(p \wedge q) \wedge r \equiv p \wedge (q \wedge r)$ | $(p \vee q) \vee r \equiv p \vee (q \vee r)$ |
| **Distributiva** | $p \wedge (q \vee r) \equiv (p \wedge q) \vee (p \wedge r)$ | $p \vee (q \wedge r) \equiv (p \vee q) \wedge (p \vee r)$ |
| **Identidad** | $p \wedge V \equiv p \quad \text{y} \quad p \wedge F \equiv F$ | $p \vee F \equiv p \quad \text{y} \quad p \vee V \equiv V$ |
| **Complemento** | $p \wedge \sim p \equiv F$ | $p \vee \sim p \equiv V$ |
| **Doble Negación** | $\sim(\sim p) \equiv p$ | - |
| **Leyes de De Morgan** | $\sim(p \wedge q) \equiv \sim p \vee \sim q$ | $\sim(p \vee q) \equiv \sim p \wedge \sim q$ |
| **Absorción** | $p \wedge (p \vee q) \equiv p$ | $p \vee (p \wedge q) \equiv p$ |
| **Condicional** | $p \rightarrow q \equiv \sim p \vee q$ | - |

</details>

---

<details>
<summary><strong> Reglas de Inferencia Lógica </strong></summary>

A continuación se presentan las reglas formales de inferencia utilizadas para las demostraciones lógicas:

### 1. Modus Ponendo Ponens
$$\frac{p \rightarrow q, \quad p}{\therefore q}$$

---

### 2. Modus Tollendo Tollens
$$\frac{p \rightarrow q, \quad \neg q}{\therefore \neg p}$$

---

### 3. Silogismo Hipotético
$$\frac{p \rightarrow q, \quad q \rightarrow r}{\therefore p \rightarrow r}$$

---

### 4. Modus Tollendo Ponens
$$\frac{p \vee q, \quad \neg p}{\therefore q}$$

---

### 5. Dilema Constructivo
$$\frac{(p \rightarrow q) \wedge (r \rightarrow s), \quad p \vee r}{\therefore q \vee s}$$

---

### 6. Dilema Destructivo
$$\frac{(p \rightarrow q) \wedge (r \rightarrow s), \quad \neg q \vee \neg s}{\therefore \neg p \vee \neg r}$$

---

### 7. Simplificación
$$\frac{p \wedge q}{\therefore p}$$

---

### 8. Conjunción
$$\frac{p, \quad q}{\therefore p \wedge q}$$

---

### 9. Adición
$$\frac{p}{\therefore p \vee q}$$

---

### 10. Conmutación
$$\frac{p \vee q}{\therefore q \vee p}$$

---

### 11. Ley de Absorción
$$\frac{p \rightarrow q}{\therefore p \rightarrow (p \wedge q)}$$

</details>

</details>

</details>

</details>

---

<details>
<summary><strong> 📂 Actividades del Curso </strong></summary>

En esta sección se encuentran organizadas las actividades desarrolladas durante el curso. Cada apartado contiene un enlace al repositorio correspondiente en Google Drive, donde se almacenan los archivos elaborados en grupo.

---

<details>
<summary><strong> 📘 Actividad Autónoma (AA) N.º 1 </strong></summary>

**Descripción**

Actividad desarrollada de forma colaborativa como parte del aprendizaje autónomo.

🔗 **Link de la carpeta**

https://drive.google.com/drive/u/1/folders/1HR13MeR_peho4W_L75XOIpiLsLLmDVXu

---

</details>

---

<details>
<summary><strong> Contrucción de tablas de verdad </strong></summary>

**Descripción**

🔗 **Link de la carpeta**

https://drive.google.com/drive/folders/1Rzh7yVSuEeYruj5YoQ7DzJuXKswm0hlY?usp=drive_link

---

</details>

---

<details>
<summary><strong> Identificacion de Tautologías </strong></summary>

**Descripción**

🔗 **Acceder a la actividad**

https://drive.google.com/drive/folders/1VmWDFUbVpSeLzDz_xVSlO9FtZC6Z-k-G?usp=drive_link

---

</details>

---

<details>
<summary><strong> 👨‍🏫 Actividad en Contacto con el Docente (ACD) N.º 2 </strong></summary>

**Descripción**

Actividad desarrollada con el acompañamiento del docente durante el segundo bloque.

🔗 **Acceder a la actividad**

https://drive.google.com/drive/folders/1VkU-psOXGXbvtGBmAJ3Sm0efdM32B3vA?usp=drive_link

---

</details>

---

<details>
<summary><strong> 🧩 Aprendizaje Practico Experimental (APE) – Fases 1 a 5 </strong></summary>

**Descripción**

Compilación de todas las fases correspondientes al Aprendizaje Basado en Problemas (ABP), desarrolladas de manera grupal.

🔗 **Acceder a las actividades**

https://drive.google.com/drive/folders/1sPb47IR0qm7r4bwuqffnLdfyjXs8n0_A?usp=drive_link

</details>

---

> **Nota:** Todos los enlaces dirigen a carpetas de Google Drive donde se encuentran almacenados los documentos, informes y demás evidencias correspondientes a cada actividad académica.


---

</details>
