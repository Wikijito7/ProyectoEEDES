# KeepIt

KeepIt es un programa de gestión de notas. Está programado en Python y soporta multiusuario.

## Dependencias:

· Tkinter (integrado en Python)

· PyMySql

· Una base de datos SQL, preferible MySQL o MariaDB.

## Set up del programa

Para hacer funcionar la base de datos, hay que crear un archivo llamado _bd.txt_ en la raiz de los archivos .py.
En este archivo hay que poner en la primera linea el usuario y en la segunda la contraseña, como se indica en [este archivo](https://github.com/Wikijito7/keepit/blob/master/bd.txt).

Una vez creado el archivo, procedemos a crear la base de datos en sí, para ello podemos apoyarnos en esta [base de datos](https://github.com/Wikijito7/keepit/blob/master/sql/keepit.sql).

Tras esto, el programa funcionaría sin problemas.

## Cómo funciona el programa
Primero deberemos ejecutar el script _[main.py](https://github.com/Wikijito7/keepit/blob/master/main.py)_, para ello abrimos una nueva terminal y ejecutamos `python3 main.py`.
Al abrirlo, lo primero nos encontraremos con una pantalla de login, usaremos el usuario que hemos creado. En el caso de no tener, 

Tras esto, nos encontraremos un menú con la opción de añadir nuevas notas. Si ya existen notas, podremos modificarlas o borrarlas.

A la hora de crear la nota, podremos indicar el título de la nota, la categoría o categorías, la etiqueta y el contenido del mismo. Es obligatorio que tenga título y el contenido. Podremos modificar todos los campos posteriormente.

Podremos filtrar las distintas notas por título, categorias o etiquetas. Una vez buscadas, podremos modificarlas o borrarlas.

## Fallos conocidos
- Al hacer la búsqueda, se nota como se recarga la pantalla y se ve _flickering_ o parpadeos.
- Si no hay una base de datos en el puerto 3306, el programa no arranca y no indica por qué ha fallado.

## Cosas por hacer
- Rehacer todo el comportamiento de ventanas a uno más cercano a la orientación a objetos para optimizar el código.
- Hacer la ventana responsiva para poder cambiar el tamaño de la ventana en tiempo de ejecución.
- Mejorar todo el tiempo de carga de la aplicación optimizando cómo funciona internamente el código.
- Reestructurar el código para que sea más legible y poder mejorar su mantenimiento a largo plazo.

## Licencia
El código es de libre uso y distribución. Se aprecia una mención en el código, aunque no es necesario hacerlo.
