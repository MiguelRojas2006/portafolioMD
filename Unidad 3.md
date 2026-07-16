# Estructuras de Datos No Lineales: Grafos y Árboles

## 📖 Introducción

El presente portafolio académico tiene como propósito consolidar y exponer los conocimientos adquiridos en el área de las **estructuras de datos**, elementos fundamentales para el diseño de algoritmos eficientes y la resolución de problemas complejos en el desarrollo de software.

Dentro de este ámbito, el estudio de las **estructuras no lineales** cobra una relevancia crítica, ya que permiten modelar relaciones complejas que superan las limitaciones de las estructuras lineales convencionales, como arreglos, listas o pilas.

En este repositorio se presenta una fundamentación teórica de las dos estructuras no lineales más representativas de las Ciencias de la Computación:

- **Grafos**
- **Árboles**

Además, se describen sus definiciones, propiedades y principales clasificaciones, sirviendo como base para el desarrollo de ejercicios y aplicaciones prácticas.

---

# 🕸️ 1. Definición y Tipología de Grafos

## ¿Qué es un grafo?

Un **grafo** es una estructura matemática abstracta que permite representar relaciones bidimensionales o de red entre un conjunto de elementos.

Formalmente se define como:

```text
G = (V, E)
```
<img width="600" height="432" alt="image" src="https://github.com/user-attachments/assets/ac3927a8-958b-4b15-b31b-6b229791f6ec" />

Donde:

| Símbolo | Descripción |
|---------|-------------|
| **V** | Conjunto no vacío de vértices o nodos que representan objetos o entidades. |
| **E** | Conjunto de aristas o conexiones que relacionan los vértices. |

---

## Clasificación de los Grafos

### 📌 Grafos Dirigidos (Dígrafos)

En este tipo de grafo las aristas poseen una dirección específica.

```text
(u → v)
```

La relación únicamente es válida desde el nodo origen hacia el nodo destino.

**Características**

- Existe un sentido de recorrido.
- La relación es unidireccional.
- Muy utilizados para representar flujos de información o dependencias.
<img width="391" height="345" alt="image" src="https://github.com/user-attachments/assets/c1f92558-f627-4fdd-88b1-51d8cccbe4dd" />


---

### 📌 Grafos No Dirigidos

Las conexiones son bidireccionales.

```text
{u, v}
```

No existe una dirección definida entre los nodos.

**Características**

- La relación es recíproca.
- Si un nodo está conectado con otro, el recorrido puede realizarse en ambos sentidos.

Su simplicidad los convierte en una de las estructuras más utilizadas en programación.

---

### 📌 Árboles Binarios de Búsqueda (BST)

Son árboles binarios que mantienen una propiedad de ordenamiento.

Para cualquier nodo:

```text
Izquierda < Nodo < Derecha
```

Gracias a esta característica permiten realizar búsquedas de forma eficiente.

---

### 📌 Árboles AVL

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

# 🎯 Objetivo del Portafolio

El análisis, diseño e implementación de las estructuras de datos no lineales constituye un pilar fundamental en la formación de futuros profesionales de la ingeniería.

Los ejercicios y casos prácticos desarrollados en este portafolio tienen como finalidad demostrar la aplicación de los conceptos teóricos mediante la resolución de problemas reales, fortaleciendo la comprensión de algoritmos y promoviendo el diseño de sistemas de información eficientes y escalables.

---

# 📂 Actividades del Curso

En esta sección se encuentran organizadas las actividades desarrolladas durante el curso. Cada apartado contiene un enlace al repositorio correspondiente en Google Drive, donde se almacenan los archivos elaborados en grupo.

---

## 📘 Actividad Autónoma (AA) N.º 1

**Descripción**

Actividad desarrollada de forma colaborativa como parte del aprendizaje autónomo.

🔗 **Link de la carpeta**

https://drive.google.com/drive/u/1/folders/1HR13MeR_peho4W_L75XOIpiLsLLmDVXu

---

## 👨‍🏫 Actividad en Contacto con el Docente (ACD) N.º 1

**Descripción**

Actividad desarrollada en conjunto bajo la orientación del docente.

🔗 **Link de la carpeta**

https://drive.google.com/drive/u/1/folders/1Try-_f5gqfEo6DHEY4VUZU3YDRXZQrM6

---

## 📘 Actividad Autónoma (AA) N.º 2

**Descripción**

Actividad colaborativa correspondiente al segundo bloque de aprendizaje autónomo.

🔗 **Acceder a la actividad**



---

## 👨‍🏫 Actividad en Contacto con el Docente (ACD) N.º 2

**Descripción**

Actividad desarrollada con el acompañamiento del docente durante el segundo bloque.

🔗 **Acceder a la actividad**



---

## 🧩 Aprendizaje Practico Experimental (APE) – Fases 1 a 5

**Descripción**

Compilación de todas las fases correspondientes al Aprendizaje Basado en Problemas (ABP), desarrolladas de manera grupal.

🔗 **Acceder a las actividades**



---

> **Nota:** Todos los enlaces dirigen a carpetas de Google Drive donde se encuentran almacenados los documentos, informes y demás evidencias correspondientes a cada actividad académica.


---
