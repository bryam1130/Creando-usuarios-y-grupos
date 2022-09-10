# Creando-usuarios-y-grupos
### Comenzando 🚀
### Ingresamos a root.

>root
>clave

#Creamos usuarios.
adduser blanca
adduser mario
adduser bryam

#Comprobamos que los usuarios existen.
* **cat /etc/passwd**

#Creamos el grupo llamado casa.
* **groupadd casa**

#Comprobamos que el grupo existe.
* **cat /etc/group**

#Agregamos los usuarios creados anteriormente al grupo llamado casa.
adduser blanca casa
adduser mario casa
adduser bryam casa

#Ver que los usuarios se han añadido a casa
cat /etc/group

#Modificamos el nombre al grupo casa, lo llamamos ahora familia.
groupmod -n familia casa

#Ver que ahora el grupo casa paso a llamarce familia.
cat /etc/group

Otros comandos utiles:

Borrar Usuario.
userdel [Nombre de usuario]

Borrar usuario de un grupo.
deluser [Nombre de usuario] [Nombre del grupo]

Borrar grupo.
groupdel [Nombre del grupo]
