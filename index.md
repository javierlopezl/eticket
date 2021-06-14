# eTicket

**¿Qué es?**

Es un sistema de tickets de soporte electrónico basado en PHP, que puede recibir tickets por correo electrónico (pop3 / pipe) o un formulario web. También ofrece un administrador de tickets con muchas funciones. Una solución de asistencia técnica ideal para cualquier sitio web.


**Principales características:**

- Admite alias / tuberías con perl gateway.

-  Admite el inicio de sesión POP3 con crontab opcional.

- Utiliza puerta de enlace Perl, backend PHP y base de datos MySQL.

- Maneja correos electrónicos ilimitados.

- Paneles de administrador / partidario / usuario.

- Intervalos de correo electrónico para evitar bucles de respuesta automática.

- Máximo permitido para limitar el número máximo de tickets que el usuario puede haber abierto.

- Filtros para eliminar mensajes en respuestas.

- Acepta archivos adjuntos y limita el tamaño.


**Funciones de administración:**

- Eliminar completamente los tickets de la base de datos.

- Crear categorías (departamentos).

- Crear representantes (partidarios).

- Definir grupos.

- Editar o deshabilitar mensajes de respuesta.

- Alertas por correo electrónico compatibles con buscapersonas.

- y mucho más...


**Funciones de usuario:**

- Inicie sesión con correo electrónico y cualquier boleto que se le asigne.

- Ver todos los tickets enviados desde ese correo electrónico. 


**Guía de instalación/uso:**

He descargado el eTicket en formato zip, lo he metido en el xampp y no me ha funcionado, y lo que he hecho junto con el profe, ha sido, descargar el vagrant y hacer lo siguiente:


Hemos puesto estos comandos en el cmd, crear el directorio xampp e instalar una máquina de vagrant ya que no hemos podido instalarlo en mi propio equipo ya que eTicket funciona con php 5, y yo tengo php 7 instalado.

```bash
mkdir xampp
cd xampp
vagrant init danielbueno99/xampp
vagrant up
```



Hemos creado un fichero llamado phpinfo.php para poder ver a travez de xampp la versión y la información del php en el que vamos a instalar eTciket

```bash
/var$ cd www
vagrant@jessie:/var/www$ ls
vagrant@jessie:/var/www$ nano phpinfo.php
vagrant@jessie:/var/www$ sudo nano phpinfo.php
```



Luego hemos descargado eticket en formato zip y con el comando unzip instalándolo a través de este comando apt install -y unzip.

Se ha actualizado los paquetes de la máquina e instalar los paquetes de php5 y mysql

```bash
apt update
apt install -y php5-mysql
```



Además de instalar los paquetes que han sido necesarios para que funcione también tenemos que poner los comandos para crear la base de datos en mysql y ver las tablas de esta.

```sql
create database eticket;
show tables;
```



Y este es el **resultado después de instalar** eTicket en xampp, ahora nos quedarían estos pasos de instalación (los seguimos igual que las imágenes):


![](1.PNG)

![](1 (1).PNG)

![](2.PNG)

![](3.PNG)





Luego en este paso tenemos que hacer lo que nos indica el anterior, en el apartado “Things to do next”. (Cosas para hacer a continuación)

![](4.PNG)



Una vez hemos terminado, iniciamos sesión con el usuario "admin" y la contraseña que hemos puesto, y ya tenemos acceso a este programa.

 



**Pantalla principal eTicket\**

![](5.PNG)

