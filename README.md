paso 1: ejecutar el comando adduser para agregar los nombres de nuestros padres y el nuestro para que el sistema los reconosca

adduser juan ,
adduser claudia 
adduser francisco

paso 2: luego ejecutaremos el comando groupadd para crear el grupo donde se alojaran los nombres 

groupadd casa

paso 3: con el comando getent group verficamos que se halla creado correctamente el grupo junto con los nombres que insertamos

getent group casa

paso 4: despues para modificar el monbre del grupo casa a familia ejecutamos el comando groupmod -n (nombre nuevo del grupo) (nombre antiguo del grupo)

groupmod -n familia casa

paso 5: en este paso volvemos a ejecutar el comando getent group para confirmar el cambio de nombre de la siguiente manera

getent group familia

nota: una vez ejecutado nos tiene que mostrar el orden de nombres que insertamos ejemplo: (juan,claudia,francisco) dentro del grupo familia
