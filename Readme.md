Digital ocean, un misterio me di cuenta que ya no se usa el putty ahora desde el mismo navegador con una ventaa puedes mepter tujs script; saben que es gracioso que yo la vez pasada pense en que para queexistes aplicaciones de escritorio si todo prodria ser web..

Correos electornico a la bandeja de gmail con nuestro user and password.

luego de poner 2 deces el password viene poder escojer nuestro password

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04

# INSTALACION DE POSTGREST
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib

Postgress utiliza un concepto llamado "roles" q

Cambiando a una Cuenta Postgres
    sudo -i -u postgres
psql // accedemos a modo consola query
\q


# Crear un Nuevo Rol
dentro de postgres (postgres@server)
createuser --interactive   // admin

sudo -u postgres createuser --interactive //visionsecurity

man createuser < mas informacion>

createdb sammy .....o como usuario normas .... sudo -u postgres createdb sammy  (visionsecuritydb

# crear un usuario para tu bd postgrest con la misma usuario de linux
sudo adduser <sammy>

ingresar
sudo -i -u sammy

cpuma
Peru123.
port:"5432".

# habilite el puerto
ufw allow 5432/tcp

sudo nano /etc/postgresql/9.3/main/pg_hba.conf

and allow connection by all users to all databases from any IP if the user has right MD5-encrypted password by adding the following line:

host all all 0.0.0.0/0 md5


77777777777777777
listen_addresses='*'
to your postgresql.conf file

service postgresql restart


# CREacion de una clave SSH.
ls -la // verificamos si existe la carpeta .ssh o sino se crea con mkdir
entramos al directorio .ssh 
ls 

ssh-keygen -t rsa -C ristian.puma.es6@gmail.com
contraseña
:..::
.:.
..::
Y te genera 2 archivos 1.pub

/////////////////
FATAL: no pg_hba.conf entry for host "200.1.181.183", user "cpuma", database "cpuma", SSL on


Tenemso que entrar en modo sudo
dentro de postgres/version/main/ ls
sudo nano pg_hba.conf
//-------al ultimo 
agregar
host    all     all   miip/32       trust
        /db     //user  //ladireccion

sudo nano postgresql.conf

habiklitamos el listen_addresses = '*'


sudo nano postgresql restart


y ya nos podemos conectar.
https://www.youtube.com/watch?v=zujeb8VWncI