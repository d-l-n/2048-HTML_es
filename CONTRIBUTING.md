# Contribuyendo
¡Los cambios y mejoras son más que bienvenidos! Siéntase libre de hacer fork y abrir un Pull Request.

Siga las reglas de la casa para tener una mayor probabilidad de que su contribución se fusione.

## Reglas de la casa

### Cómo hacer cambios
 - Para realizar cambios, cree una nueva rama basada en `master` (no crear una desde `gh-pages` a menos que sea estrictamente necesario) y hazlos allí, luego crear un Pull Request al `master`.  
 `gh-pages` se diferencia de master en que el mismo contiene funciones de compartir, analíticas y otras cosas que no tienen relación directa con el juego. `master` es la versión "pura" del juego.
 - Si quieres modificar el CSS, por favor edita los archivos SCSS presentes en `style/`: `main.scss` y otros. No edites `main.css`, por que  es supuesto a ser generado.  
 Para compilar tus modificaciones de SCSS, necesitas usar la gema `sass` (instalalo ejecutando `gem install sass` una vez que Ruby se encuentre instalado).  
 Para ejecutar SASS, simplemente usa el siguiente comando:  
 `sass --unix-newlines --watch style/main.scss`  
 SASS va a recompilar automáticamente tu css cuando cambie.
 - `Rakefile` contiene algunas tareas que pueden ayudar durante el desarrollo. Siéntete libre de añadir tareas útiles de ser necesario.
 - Por favor use identación de 2-espacios cuando estés editando JavaScript. Se encuentra un archivo `.jshintrc`, el cual ayudará a tu código a seguir las líneas de guía si instalas y ejecutas `jshint`.
 - Pruebe su modificación a fondo antes de enviar su Pull Request.

### Cambios que no serán aceptados
We have to be conservative with the core game. This means that some modifications won't be merged, or will have to be evaluated carefully before being merged:

 - Funciones de Deshacer/Rehacer
 - Funciones de Guardar/Recargar
 - Cambios en el aspecto de los mosaicos/cuadros o su contenido.
 - Cambios en el diseño
 - Cambios en el tamaño de la cuadrícula

### Cambios que serán bienvenidos
 - Solucion de errores
 - Mejoras de compatibilidad
 - Mejoras "bajo el capó"
 - Pequeños cambios que no tienen impacto en el juego principal
