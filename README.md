# Universidad Técnica de Ambato  
## Facultad de Ingenieria en Sistemas Electronica e Industrial
### Carrera de Ingeniería en Software  

**Asignatura:** Manejo y Configuración de Software  
**Nombre del Estudiante:** Alison Cobos
**Fecha:** 07/10/2025
---

# Evaluación Práctica de Git y GitHub

## Instrucciones Generales

- Cada pregunta debe ser respondida directamente en este archivo **(README.md)** debajo del enunciado correspondiente.
- Cada respuesta debe ir acompañada de uno o más **commits**, según se indique en cada pregunta.
- Cuando se indique, deberán realizarse acciones prácticas dentro del repositorio (como creación de archivos, ramas, resolución de conflictos, etc.).
- Cada pregunta debe estar **etiquetada con un tag**, únicamente en el commit final correspondiente, con el formato: `"Pregunta 1"`, `"Pregunta 2"`, etc.

---

## Pregunta 1 (1 punto)

**Explicar la diferencia entre los siguientes conceptos/comandos en Git y GitHub:**

git clone
fork
git pull

### Parte práctica:

- Realizar un **fork** de este repositorio en la cuenta personal de GitHub del estudiante.
- Luego, realizar un **clone** del fork en el equipo local.
- En este README, describir el proceso seguido:
  ¿Cómo se realizó el fork?
¿Cómo se realizó el clone del fork?
¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?
**📝 Respuesta:**
**Explicar la diferencia entre los siguientes conceptos/comandos en Git y GitHub:**
- **`git clone`**: crea una copia local de un repositorio remoto, descargando todos los archivos y el historial de commits a mi computador.
- **Fork**: crea una copia del repositorio en mi cuenta personal de GitHub. Permite hacer cambios y luego enviar Pull Requests sin modificar el original.
- **`git pull`**: actualiza mi repositorio local con los cambios más recientes del remoto, combinando `fetch` y `merge`.

### Parte práctica:

- Realizar un **fork** de este repositorio en la cuenta personal de GitHub del estudiante.
- Luego, realizar un **clone** del fork en el equipo local.
- En este README, describir el proceso seguido:
  - ¿Cómo se realizó el fork?
    - Inicié sesión en mi cuenta de GitHub.
   - Fui al repositorio del docente:  
     👉 [https://github.com/santiagojara/EVALUACION_1P](https://github.com/santiagojara/EVALUACION_1P)
   - Hice clic en **Fork → Create fork** y GitHub creó mi copia:  
     `https://github.com/Itsuna18/EVALUACION_1P`.
  - ¿Cómo se realizó el clone del fork?
   git clone https://github.com/Itsuna18/EVALUACION_1P.git
   cd EVALUACION_1P
  - ¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?
  Se verifico con git remote -v 

## Pregunta 2 (1 punto)

**Configurar un archivo `.gitignore` para que ignore:**

- Todos los archivos con extensión `.log`.
- Una carpeta llamada `temp/`.
- Todos los archivos `.md` y `.txt`de la carpeta `doc/`. (Probar agregando un archivo `prueba.md` y un archivo `prueba.txt` dentro de la carpeta y fuera de la carpeta.)

### Requisitos:

1. Realizar un **primer commit** que incluya únicamente el archivo `.gitignore` con las reglas de exclusión definidas.
2. Realizar un **segundo commit** donde se explique en este README la función del archivo `.gitignore` y se muestre evidencia de que los archivos y carpetas indicadas no están siendo rastreadas por Git.

**Importante:**  
- Solo el **segundo commit** debe llevar el **tag `"Pregunta 2"`**.

**📝 Respuesta:**
REGLAS QUE APLICAMOS:
*.log        → Ignora todos los archivos con extensión .log  
temp/        → Ignora toda la carpeta temp/  
doc/*.md     → Ignora los archivos .md dentro de doc/  
doc/*.txt    → Ignora los archivos .txt dentro de doc/
COMO FUNCIONA?
Después de crear los archivos:

prueba.log

temp/archivo.log

doc/prueba.md

doc/prueba.txt

prueba.md

prueba.txt

y ejecutar git status, solo aparece el archivo .gitignore como rastreado, confirmando que las reglas funcionan correctamente.
![alt text](IMG/image.png)

## Pregunta 3 (2 puntos)

**Utilizar Git Flow para desarrollar una nueva funcionalidad llamada `ingresar-encabezado`.**

*.log        → Ignora todos los archivos con extensión .log  
temp/        → Ignora toda la carpeta temp/  
doc/*.md     → Ignora los archivos .md dentro de doc/  
doc/*.txt    → Ignora los archivos .txt dentro de doc/
### Requisitos:

- Inicializar el repositorio con Git Flow, utilizando las ramas por defecto: `main` y `develop`.
- Crear una rama de tipo `hotfix` con el nombre `ingresar-encabezado`.
- En dicha rama, **completar con los datos personales del estudiante** el encabezado que ya se encuentra al inicio de este archivo `README.md`.
- Realizar al menos un commit durante el desarrollo.
- Finalizar el hotfix siguiendo el flujo de trabajo establecido por Git Flow.

### En este README, se debe incluir:

- Los **comandos exactos** utilizados desde la inicialización de Git Flow hasta el cierre del hotfix.
- Una descripción del **proceso seguido**, indicando el propósito de cada paso.
- Una reflexión sobre las **ventajas de aplicar Git Flow**, especialmente en contextos colaborativos o proyectos de larga duración.

**Importante:**

- Deben realizarse varios commits durante esta pregunta.
- **Solo el commit final** debe llevar el **tag `"Pregunta 3"`**.
- El flujo debe respetar la estructura de Git Flow con las ramas `develop` y `main`.

**📝 Respuesta:**
Se inicio el repo Git Flow:
![alt text](IMG/image2.png)
Inicio de la rama hotfix:
![alt text](IMG/image3.png)
Finalización del hotfix depues de realizar todo lo anterior sin errores:
![alt text](IMG/image4.png)
Ventajas de Git Flow:
Nos permite realizar todo con mas facilidad, sin utilizar tantos comandos para insertar y mas, ayudandonas a redactar mejor el documento. Podemos decir que convierte el desorden del desarrollo en una estrategia metódica, minimizando riesgos y maximizando la trazabilidad del proyecto.
## Pregunta 4 (2 puntos)

**Trabajo con Issues y Pull Requests**

### Parte teórica:

- Explicar qué es un **issue** en GitHub.
- Explicar qué es un **pull request** y cuál es su finalidad.
- Indicar la diferencia entre ambos y cómo se relacionan en un entorno de trabajo colaborativo.

### Parte práctica:

- Trabajar en la rama `develop`, ya existente desde la configuración de Git Flow.
- Crear un **issue** titulado `"Respuesta a la Pregunta 4"`, en el que se indique que su objetivo es documentar esta pregunta.
- Realizar los cambios necesarios en este archivo `README.md` para responder esta pregunta.
- Realizar un **commit** con los cambios y subirlo a la rama `develop` del repositorio remoto.
- Crear un **pull request** desde `develop` hacia `main` en GitHub.
- **Vincular el pull request con el issue creado**, de manera que al ser aprobado y fusionado, el issue se cierre automáticamente.
- **Aprobar** el pull request para que se haga el merge respectivo hacia `main`.

### En este README, se debe incluir:

- Un resumen del procedimiento realizado.
- El número y enlace del issue creado.
- El número y enlace al pull request.

**📝 Respuesta:**
**Parte teórica**

**¿Qué es un issue?**
Es un ticket en GitHub para reportar bugs, proponer mejoras o documentar tareas. Permite discusión, asignación, etiquetas y seguimiento del estado.
**¿Qué es un pull request (PR) y su finalidad?**
Es una solicitud de integración de cambios desde una rama (o fork) hacia otra (p. ej., develop → main). Sirve para revisión de código, validación y merge controlado.

**Diferencia y relación en trabajo colaborativo**
El issue define el qué y por qué (problema/tarea). El PR entrega el cómo (código/cambios). Un PR puede cerrar automáticamente un issue si en su descripción se incluye Closes #<número> y se fusiona.
**Parte práctica**

1. Trabajé en la rama develop.

2. Creé un issue en GitHub titulado “Respuesta a la Pregunta 4” indicando que documenta esta pregunta.

3. Edité este README para responder teoría y práctica.

4. Hice commit de los cambios y subí a develop en mi fork.

5. Abrí un PR develop → main en GitHub.

6. En la descripción del PR puse Closes #<N> para cerrar automáticamente el issue al hacer merge.

7. Aprobé y fusioné el PR hacia main.
## Pregunta 5 (2 puntos)

**Resolver conflictos entre ramas y realizar un Pull Request**

### Requisitos:

- Crear dos ramas llamadas `ramaA` y `ramaB`, ambas a partir de la rama `develop`.
- En `ramaA`, crear un archivo llamado `archivoA.txt` con el contenido:  
  `Contenido A`
- En `ramaB`, crear un archivo con el mismo nombre (`archivoA.txt`), pero con el contenido:  
  `Contenido B`
- Intentar fusionar `ramaB` sobre `ramaA`, lo cual debe generar un conflicto.
- Resolver el conflicto combinando ambos contenidos.
- Realizar el merge de `ramaA` hacia `develop`.
- Crear un **pull request** desde `develop` hacia `main`.
- Una vez completado lo anterior, eliminar las ramas `ramaA` y `ramaB` tanto local como remotamente.

### En este README, se debe incluir:

- El procedimiento completo:
  - Cómo se crearon las ramas.
  - Cómo se generó y resolvió el conflicto.
  - Cómo se realizó el merge hacia `develop`.
  - Cómo se eliminaron las ramas al finalizar.
- El enlace al pull request.
- Una breve explicación de qué es un conflicto en Git y por qué ocurrió en este caso.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 5 -->

---

## Pregunta 6 (2 puntos)

**Realizar limpieza, explicar versionamiento semántico y enviar cambios al repositorio original**

### Requisitos:

- Trabajar en la rama `develop` del fork del repositorio.
- Eliminar los archivos `archivoA.txt` y `archivoB.txt` creados en preguntas anteriores.
- Realizar un merge desde `develop` hacia `main` en el repositorio local.
- Enviar los cambios de la rama `main` local a la rama `develop` del repositorio remoto (fork). Recuerde incluir todos los tags creados (6 tags).
- Finalmente, crear un **pull request** desde la rama `develop` del fork hacia la rama `main` del repositorio original (del cual se realizó el fork en la Pregunta 1). El titulo del pull request debe ser "NOMBRE APELLIDOS", en la descripción colocar el link de su repositorio de GitHub.

### En este README, se debe incluir:

- Una explicación del proceso realizado paso a paso.
- Una explicación del **versionamiento semántico**, indicando:
  - En qué consiste.
  - Sus tres componentes (MAJOR, MINOR, PATCH).
- El enlace al pull request creado hacia el repositorio original.
- Si hace falta agregar alguna evidencia adicional, agregue un tag adicional que sea `Version Final`.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 6 -->
