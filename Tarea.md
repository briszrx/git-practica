Nombre: Allison Briseyda Avila Moctezuma
Url del repositorio: [briszrx/git-practica](https://github.com/briszrx/git-practica)
## Parte 1 | Investigación git
#### ¿Qué es un sistema de control de versiones?
Es una herramienta que permite gestionar y rastrear los cambios en el código fuente de un proyecto a lo largo del tiempo, facilitando la colaboración y la recuperación de versiones anteriores. 

Evita la pérdida de código, da trazabilidad sobre quién modificó qué y previene sobreescrituras al trabajar en equipo.

Es util porque puedes crear copias aisladas para probar funciones o corregir bugs, Une el trabajo de varios desarrolladores, permite regresar a cualquier versión estable.

Las ventajas a comparación de copias manuales es que hay menos espacio, hace que el trabajo en equipo sea fluido al no estarse mandando archivos por correo ni copiar y pegar código a mano.
#### ¿Qué es Git?
**Git** es un sistema de control de versiones distribuido, gratuito y de código abierto, creado por Linus Torvalds en 2005. El desarrollo del kernel de **Linux**, tras perder la licencia gratuita del sistema propietario que usaban antes (BitKeeper). Su principal propósito es gestionar cambios en proyectos de desarrollo, permitiendo a múltiples desarrolladores trabajar en paralelo sin conflictos. A diferencia de los sistemas centralizados (donde el historial completo vive solo en un servidor central), en Git **cada desarrollador tiene una copia local completa del repositorio**, incluyendo todo el historial y todas las ramas. Esto permite trabajar, hacer commits y consultar versiones sin conexión a internet, además de evitar un punto único de falla.
## Parte 2 | Git vs GitHub 
#### Git
es el programa de control de versiones que instalas y ejecutas localmente en la computadora, funciona de forma offline y se encarga de registrar el historialk de cambiso de los archivos, crear ramas y guardar versiones mediante commits

#### GitHub
Es un servicio en la nube el cual aloja proyectos que se gestionan con Git, este si requiere internet y sirve para respaldar el código en línea, colaborar y compartir con otras personas con otras personas a través de funciones web como Pull Requests, seguimiento de problemas y revisión de código.

##### GitLab
El enfoque de esta pataforma integral de DevOps / DevSecOps (_todo en uno_). Trae herramientas nativas muy potentes para todo el ciclo de vida del software: gestión de tareas, escaneo de seguridad y pipelines de CI/CD avanzados, Ofrece código abierto que permite autohospedar la plataforma en servidores propios de una empresa de forma gratuita y con control total.
##### Bitbucket
Esta busca una integración con el ecosistema empresarial de Atlassian. Se conecta de manera nativa y bidireccional con herramientas populares de gestión de proyectos como **Jira**, Confluence y Trello.
Incluye su propio sistema de integración continua ligero llamado_Bitbucket Pipelines.

## Parte 3 | Instalar Git

Sistema Operativo: Windows

Versión de Git
![[Pasted image 20260904185043.png|230]]



Configuración: 
![[Pasted image 20260904185128.png|418]]

## Parte 4 | Crear primer repo

![[Pasted image 20260904185524.png]]

## Parte 5 | Crear primer archivo

![[Pasted image 20260904190010.png]]


Con comando: git status

![[Pasted image 20260904190050.png]]

## Parte 6 | Estados principales de git

solo había Información dentro de la parte

## Parte 7 | Primer Commit

Siguiendo los pasos dentro de la terminal...
![[Pasted image 20260904190554.png]]

## Parte 8 | Trabajar con cambios

Siguiendo las instrucciones:
![[Pasted image 20260904191033.png]]

## Parte 9 | Cliclo normal del trabajo
Nos da a entender el cliclo de como es que debemos de trabajar con git y el repositorio

## Parte 10 | Crear una rama

![[Pasted image 20260904191321.png]]
##### Git checkout 
sirve para cambiar entre ramas, restaurar archivos o inspeccionar commits específicos en un repositorio Git. Es una herramienta esencial para gestionar versiones y ramas en proyectos.

## Parte 11 | Trabajar en la nueva rama

Evidencia:
![[Pasted image 20260904191926.png]]

## Parte 12 |  Merge

![[Pasted image 20260904192046.png]]

##### ¿Que es una rama?
Una rama es como una partición de la versión de nuestro proyecto la cual es independiente, funciona como una copia donde puedes escribir y probar código sin alterar la rama principal.

##### ¿Por qué un equipo de desarrollo utilizaría ramas?
Porque este permite que varios desarrolladores trabajen al mismo tiempo en funciones distintas, correcciones de errores o experimentos sin estorbarse ni sobreescribir el trabajo ajeno. También, mantiene la rama principal siempre limpia, estable y lista para producción, asegurando que solo se integre código revisado y probado.

##### ¿Que hace git merge?
Es el comando que integra los cambios de una rama secundaria que es dentro de la actual con la principal (suele ser).

## Parte 13 | .gitignore

##### ¿Para qué sirve?
El archivo `.gitignore` sirve para indicarle a Git qué archivos, carpetas o extensiones debe ignorar por completo, evitando que se registren en el historial de cambios o se suban a un repositorio remoto.
##### ¿Por qué no se suele incluir node_modules?
Debido a su gran tamaño y la enorme cantidad de archivos que contiene, lo que haría que clonar o sincronizar el repositorio fuera un proceso lento e ineficiente.

##### ¿Por qué un `.env` puede contener información que no debería publicarse?
No debe publicarse porque almacena variables de entorno con información confidencial y sensible para el funcionamiento de la aplicación, como credenciales de bases de datos, claves secretas de encriptación, tokens de autenticación o API keys privadas.

## Parte 14 | Repositorio local y remoto

Explicacion del commit y el push

## Parte 15 | Publicar el repositorio en GitHub

conexion de ambos repos
![[Pasted image 20260904194040.png]]

## Parte 16 | Clonar repositorio

Siguiendo los comandos
![[Pasted image 20260904194321.png]]

## Parte 17 | `push`, `pull` y trabajo colaborativo

dice la explicacion de  los comandos git push, git pull y git clone

## Parte 18 | Preguntas de reflexión

1. ¿Qué diferencia existe entre `git add` y `git commit`?
		git add selecciona y prepara los archivos modificados y git commit toma todos los cambios de los arvhivos que estaban en el area de preparacion por asíd ecir t los guarda de forma permanente en el historial del repositorio local con un mensaje si es que lo pones con -m
2. ¿Qué ventaja tiene realizar varios commits pequeños en lugar de un solo commit grande? 
		hay dos cosas que yo considero principales, como el que puedes entender de una mejor forma todos los cambios que se han hecho ya que se especifica que es lo que se cambio de forma muy precisa y que también puedes recuperar desde un punto en adelante y poder reparar algún error en cambio si se hace de forma grande puede que no sepas desde fue que dejó de funcionar.
3. ¿Qué diferencia existe entre Git y GitHub?
		Git es el software de control de versiones que corre de forma local sin necesidad de tener internet, en cambio githubes una plataforma web en la nube que sirve para alojar los repositorios de git de forma remota, respalda codigo y permite colaborar con otras personas.
4. ¿Qué problema resuelven las ramas?
		Resuelven el conflicto de trabajar sobre una única línea de código compartida. Cada persona puede trabajar en su propia rama sin "estorbarse" y ayuda para agregar funciones, experimentar o arreglar errores, para integrar ya que se este listo.
5. ¿Qué información no debería normalmente almacenarse en Git?
		Archivos de entorno, contraseñas  privadas, API keys, Dependencias de paquetes, Archivos del sistema o archivos compilados o binarios pesados
6. ¿Qué ocurriría si borras tu proyecto local pero está publicado en GitHub?
		Si lo tienes actualizado en github no causaría ningún problema porque lo puedes recuperar con solo clonarlo
7. ¿Por qué Git es especialmente importante cuando varias personas trabajan sobre el mismo proyecto?
		Porque así no interrumpen su trabajo entre sí, cada quien avanza en su propia rama sin sobrescribir o borrar accidentalmente el avanza de los demás
8. ¿Cuál es la diferencia entre `git clone`, `git pull` y `git push`?
		Git clone: Descarga un repositorio remoto a tu computadora, es decir, lo clona.
		Git pull: Descarga e integra automaticamente los commits nuevos del repo en la nube al repo en lel local, es decir baja la informacion nueva
		Git push: envía los commits que hiciste en tu repo local hacia el repo en la nube para que quede publicado y respaldado, es decir sube su avance
9. ¿Por qué un commit no aparece automáticamente en GitHub?
		Porque Git es un sistema de control de versiones distribuido. Las operaciones cotidianas (`git add` y `git commit`) ocurren exclusivamente en la base de datos local de tu computadora (`.git/`) y funcionan sin conexión.
