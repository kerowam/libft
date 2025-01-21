<div align="center">
  <img src="https://raw.githubusercontent.com/15Galan/42_project-readmes/refs/heads/master/banners/cursus/projects/libft-light.png#gh-light-mode-only" />
  <img src="https://img.shields.io/badge/status-finished-green" />
  <img src="https://img.shields.io/badge/score-125-blue" />
</div> 

---

# 📖 Introducción
Libft es un proyecto del programa de 42 School que consiste en crear una biblioteca de funciones en C. El objetivo principal es replicar y extender funciones comunes de la librería estándar de C (`libc`), además de desarrollar nuevas funciones útiles para futuros proyectos.

Este es el [subject](Libft_es.subject.pdf) del proyecto.

---

## Tabla de contenidos
- ⚙️[Requisitos](#requisitos)
- 🛠️[Instalación](#instalación)
- 🚀[Uso](#uso)
- 📚[Funciones Implementadas](#funciones-implementadas)

---

## ⚙️Requisitos

- **Sistema operativo**: Linux o macOS
- **Compilador**: `gcc` con soporte para el estándar C99 o superior
- **Herramientas**: `Makefile` para la compilación, doxygen(opcional)

---

## 🛠️Instalación

1. Clona este repositorio en tu máquina local:
   ```bash
   git clone https://github.com/tu_usuario/libft.git
   cd libft
   ```
2. Compila la biblioteca ejecutando el comando:
   ```bash
   make
   ```
3. Esto generará un archivo llamado `libft.a`, que puedes incluir en tus proyectos.

---

## 🚀Uso

Para usar libft en tu proyecto, incluye el archivo de cabecera y enlaza la biblioteca al compilar:
  ```c
  #include "libft.h"
  ```
Compila tu programa enlazando la biblioteca:
  ```c
  gcc -o programa principal.c -L. -lft
  ```

---

## 📚Funciones implementadas

En **libft**, las funciones están divididas en varias categorías según su funcionalidad y propósito.

---

### Parte 1 - Funciones de la libc

Estas funciones son implementaciones propias de algunas de las funciones más comunes de la biblioteca estándar de C. Sirven para manipulación de cadenas, memoria y más.

- **Manipulación de memoria:**
  - `ft_memset` - Llena una región de memoria con un byte específico.
  - `ft_bzero` - Llena una región de memoria con ceros.
  - `ft_memcpy` - Copia un bloque de memoria de una ubicación a otra.
  - `ft_memccpy` - Copia bytes de memoria hasta encontrar un carácter específico.
  - `ft_memmove` - Copia bloques de memoria, manejando solapamientos.
  - `ft_memchr` - Busca un byte en una región de memoria.
  - `ft_memcmp` - Compara dos regiones de memoria.

- **Manipulación de cadenas:**
  - `ft_strlen` - Calcula la longitud de una cadena.
  - `ft_strlcpy` - Copia una cadena con un tamaño limitado.
  - `ft_strlcat` - Concatenación segura de cadenas con límite de tamaño.
  - `ft_strchr` - Busca la primera ocurrencia de un carácter en una cadena.
  - `ft_strrchr` - Busca la última ocurrencia de un carácter en una cadena.
  - `ft_strncmp` - Compara dos cadenas hasta un número específico de caracteres.
  - `ft_strnstr` - Encuentra la primera aparición de una subcadena dentro de otra, limitada por tamaño.
  - `ft_strdup` - Crea una copia dinámica de una cadena.

- **Conversión y utilidades:**
  - `ft_atoi` - Convierte una cadena a un entero.
  - `ft_isalpha` - Verifica si un carácter es alfabético.
  - `ft_isdigit` - Verifica si un carácter es un dígito.
  - `ft_isalnum` - Verifica si un carácter es alfanumérico.
  - `ft_isascii` - Verifica si un carácter pertenece al conjunto ASCII.
  - `ft_isprint` - Verifica si un carácter es imprimible.
  - `ft_toupper` - Convierte un carácter a mayúscula.
  - `ft_tolower` - Convierte un carácter a minúscula.

---

### Parte 2 - Funciones adicionales

Estas funciones extienden la funcionalidad estándar y ofrecen herramientas útiles para manipular cadenas y estructuras dinámicas.

- **Manipulación de cadenas:**
  - `ft_substr` - Extrae una subcadena de una cadena dada.
  - `ft_strjoin` - Une dos cadenas en una nueva.
  - `ft_strtrim` - Elimina caracteres específicos de los extremos de una cadena.
  - `ft_split` - Divide una cadena en un array de cadenas basado en un delimitador.
  - `ft_itoa` - Convierte un número entero a una cadena.
  - `ft_strmapi` - Aplica una función a cada carácter de una cadena y genera una nueva.

- **Manipulación de memoria dinámica:**
  - `ft_calloc` - Asigna memoria inicializada a ceros.
  - `ft_free` (opcional según tu implementación) - Libera memoria de manera segura.

---

### Parte 3 - Funciones Bonus

Esta sección está enfocada en trabajar con listas enlazadas, una estructura de datos básica.

- **Creación y manipulación de listas:**
  - `ft_lstnew` - Crea un nuevo nodo para una lista enlazada.
  - `ft_lstadd_front` - Agrega un nodo al frente de una lista.
  - `ft_lstadd_back` - Agrega un nodo al final de una lista.
  - `ft_lstdelone` - Elimina y libera un nodo de la lista.
  - `ft_lstclear` - Elimina y libera todos los nodos de la lista.
  - `ft_lstiter` - Itera sobre una lista y aplica una función a cada nodo.
  - `ft_lstmap` - Crea una nueva lista aplicando una función a cada nodo de la original.

---

Esta clasificación hace que sea más fácil entender y reutilizar las funciones implementadas. Puedes explorar el archivo `libft.h` para ver las definiciones y prototipos de todas las funciones.  
Puedes utilizar Doxygen Documentation Generator para ver más información sobre las funciones mientras las utilizas.
