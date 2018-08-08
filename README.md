# topicosEnTelematica
# Proyecto 1 tópicos en telemática

# Descripción del proyecto:
La aplicación consiste en obtener una ruta en un navegador web a través de una serie de puntos obtenidos por geolocalización (latitud y longitud).
Para el desarrollo de la aplicación se utilizaron 3 ambientes distintos: local, de pruebas (DCA) y en la nube (AWS).

# Configuración de los ambientes

Como la aplicación fue desarrollada en un sistema operativo Linux (Centos7) con las herramientas NodeJS y una persistencia en mongoDB en forma dockerizada los necesitaremos instalar y se hace de la siguiente manera:
mongoDB:
* sudo vi /etc/yum.repos.d/mongodb-org.repo
*	sudo yum install mongodb-org
*	sudo systemctl start mongod
Fuente: https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-centos-7
NodeJS:
*	sudo yum install epel-release
*	sudo yum install nodejs
*	node --version
y listo con eso nos daremos cuenta le versión del node.

Fuente: https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-a-centos-7-server
Además de estas herramientas, también necesitaremos instalar Docker para todo el manejo de la dockerización en los ambientes del DCA y 
AWS y se hace así:


Docker-ce:

*	sudo yum install -y yum-utils \
  	device-mapper-persistent-data \
 	lvm2
*	sudo yum-config-manager \
  	  --add-repo \
   	 https://download.docker.com/linux/centos/docker-ce.repo
*	sudo yum install docker-ce
*	sudo systemctl start Docker

para confirmar la correcta instalación se corre el siguiente comando
*	sudo docker run hello-world
y si nos aparece un mensaje informacional, está correctamente instalado.



