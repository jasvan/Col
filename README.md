## proyecto colegio 09/06/2019
### flujo de trabjo basico de git
1. Mofifica una serie de archivos en tu directorio de trabajo.
2. Prepara los archivos, añadiendolos a tu area de preparacion.
3. Confirmas los cambios, lo que toma son los archivos tal y como estan en el area de preparacion y almacena esa copia instatantanea de manera permanente en tu directprio de git.

### git commit toma la los archivos que estavan en la zona de preparacion y los guarda en un punto en la historia, o hace una copia inmediata de nuestros archivos.

### git log muestra todos los commits echos hasta el momento.
### git diff muestra los cambios echos en los archivos de los que estavan en commit en compartiva a los que todavia no estan confirmados.

### Zonaas de git, o notas de la clase.
Zona 1 Directorio de trabajo
Zona 2 Area de preparacion
Zona 3 Directorio git

## Sistema de de control de versiones para el manteniminto eficiente y confiable de archivos.

## git rm elimina archivos rastreados del directorio de trabajo de manera permanente y se confirma la eliminacion creando un commit de esa eliminacion.

###git checkout --nombre del archivo, se utiliza para restablecer archivos borrados  manuelmente, o renombrados con el editor o eliminados con el edito.

### git mv "nombre del archivo acutal" "Nuevo nombre del archivo", si se renombra con el editor gir los tomara cono eliminados momentaneamente.

### git log: nos muestra las opciones de comando que podemos encontrar,
'--oneline:' nos muestra el historial abreviado.

'--graph:' añade un pequeño grafico asccii, mostrando el historial de ramificaciones y unoines.

ejemplo git log --oneline otro git log --graph otro git log --oneline -- ggraph. 

### git log -2 por ejemplo muestra los dos ultimos commits que se hicieron
## git log --help muestra todas las opciones relacionadas a it log que se puese usar.
### git log --after="fecha y hora": muestra los commits echos depues de esa fecha, como tambien se puede mostrar los commits echos del dia de hoy.
ejemplo git log --after="11:42:35 2019"
