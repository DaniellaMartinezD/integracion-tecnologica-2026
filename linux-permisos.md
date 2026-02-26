¿que es un usuario? 
R/ es una persona o servicio que se define por un nombre, una contraseña y la
cual obtiene permisos especificos segun la necesidad como acceder a archivos o 
ejecutar procesos.

¿que es un grupo?
R/ un grupo es un conjunto de usuarios que pueden gestionar o asignar permisos,
tener acceso a diferentes archivos y recursos de manera grupal. Esto permite
que en lugar de dar acceso a un usuario de forma individiar se otorgen estos 
permisos al grupo.

¿como funciona chmod?
R/ este comando permite modificar los permisos de lectura, escritura y ejecución
de archivos y directorios,a tres tipos de usuarios los cuales son el propietario,
grupo y otros. Tiene desde uso numerico (octal) donde se usan 3 digitos donde
cada digito representa una suma de valores, 4(lectura), 2(escritura) y 1(ejecucion)
y en el uso simbolico se utilizan las letras (u,g,o,a) con operadores (+(añadir)),
(-(quitar)) o (=(establecer).

¿que significa 755?
R/ el 7 significa que el propietario tiene permisos de lectura, escritura y 
ejecución.
el 5 significa que el grupo tiene permisos de lectura y ejecución.
el 5 significa que otros tienen permisos de lectura y ejecución.

¿que hace chown?
R/ el comando chown es decir change owner permite cambiar al propietario y/o al
grupo de un archivo o directorio.

creacion de usuario
R/ para crear un usuario: ejemplo el dev1 
sudo adduser dev1

creacion de grupo
R/ para crear un grupo: ejemplo el grupo supporting
sudo groupadd supporting

cambio de permisos 
R/ para realizar un cambio de permisos, el ejemplo seria con dev1 quien seria 
el propietario y developers el grupo, primero se asigan estos y en caso de que solo
se desee que el propietario tenga acceso completo, el grupo pueda entrar y leer y
los otros no tengan acceso se usaria: sudo chmod 750 /empresa/development. 
