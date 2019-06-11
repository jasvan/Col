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

###clase tres:  haciendo uso del comando git commit --amend nos sirve para agregar nuevos archivos al commit que ya estaba creado, en el caso de que se presentara la ocacion de hacerlo o de cumplir con una tarea dieria de un proyecto.

### restaurar un archivo a la vercion anterior
el procedimiento lo hace el comando git checkout. Este es un comando peligroso cualquier cambio que se le haya echo al archivo desaparecera, nunca utilice este comando a menos que se este seguro de eliminar los cambios del archivo.

### git log --decorate --all, sirve para mostrar todos los commits realizados y las ramas que tiene los commits

### git checkout y el hash del commit nos sirve para regresar ene el tiempo hacia a tras y deshacer los cambios actuales.

#### git checkout master sirve para devolvernos al futuro al punto de partida y restaurar los cambios antes eliminados.

### Clase 4: git tagv1.1 etiquetas ligeras, una etiqueta ligera no es mas que un checksum de un commit guardado en un archivo, no incluye mas informacion para crear una etiqueta lijera no pasamos las opciones -a, -s, ni -m. ejemplo " git tag mi-etiqueta" este tag se agrega automaticamente al commit mas reciente que ya esta elavorado.

### git tag con anotaciones: git tag -a v1.0-m 'mi vecion 1.0', Se guardan en la base de datos de git como obgetos enteros. tienen un checksum; contiene el nombre del etiquetador, correo electronico y fecha; y tiene un mensaje anotado. no se admiten espacions en blanco.
ejemplo  git tag -a v1.0 -m "Primera vercion estable"

### git sow mi-etiqueta, muestra la informacion que esta relacionada con el commit que reprecenta este tag. tambien se puede componer asi git tag f876sd y el hash del commit.

### git log decorate muestra la informacion entre parentesis de la cabeceras o ramas
ademas git tag lista las etiquetas en orden alfabetico.

### git tag -l "v1.*": lista las etiquetas que coinsidan con ese patron de busqueda.

#### podemos hacer git checkout a una etiqueta y tambien sirve como si se hiciera a un comit sirve de la misma forma.

###git log --decorate --all, mustra todos los archivos del directorio git sin inportar que que punto de la historia este pocicionado.

#### clase 6: creando nuevas ramas, para crear una nueva rama se usa el comando git branch testing: donde testing es el nombre de la nueva rama.

### git checkout testing, en el anterior comando solo se creo la nueva rama pero head sigue puntando a master con git checkout testing movemos o remplazamos head por testing o a la nueva rama.
