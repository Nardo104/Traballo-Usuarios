
## CONFIGURACIÓN DE SISTEMAS OPERATIVOS






+ Santiago Ezequiel Torres
+ Leonardo Caamaño Tajes














1-Creacion de usuarios	3







1-Creación de usuarios y grupos locales (windows)


Primero que nada empezaremos por abrir el administrador de sistemas,“Herramientas del sistema” y “Usuarios y grupos locales”.
Una vez aquí iremos a grupos click derecho crear grupo nuevo.
![image](https://github.com/Nardo104/Traballo-Usuarios/assets/164507058/fca211b6-00c0-403c-b1f0-32368d2247a2)














Tras lo cual nos aparecera la siguiente ventana donde le pondremos el nombre que deseamos y pulsaremos crear.


Para crear RRHH repetiremos estos mismo pasos.

Para crear a los usuarios iremos a usuarios y pulsaremos en Usuario nuevo.



Tras lo cual nos aparecera la siguiente ventana donde rellenaremos los datos del usuario y unavez echo esto le daremos a crear.


Repetiremos esto con todos los usuarios.

Para añadirlos a sus respectivos grupos iremos a grupos y los pondremos como miembros en sus respectivos grupos.

Repetiremos este proceso para todos los usuarios.


Ficheros:

Creamos los directorios Desarrollo y Recursos humanos



Permisos:

Para otorgar permisos en Windows primero tenemos que ir a la carpeta que queremos otorgar los permisos.


Una vez en ella haremos click derecho e iremos a propiedades.


Luego a seguridad.


Para luego aquí editar.


Pondremos los permisos que queremos que tenga nuestros grupos y usuarios, para añadir a otros usuarios o grupos iremos a agregar.

Una vez en agregar iremos a opciones avanzadas


En opciones avanzadas pulsaremos en buscar ahora y elegiremos a las personas o grupos que queramos añadir, pulsaremos aceptar.



Una vez añadidos aqui les daremos los permisos necesarios.


Compartido:




RRHH:




Desarrollo:




Fichero Personal:


Linux:




Crea los siguientes usuarios locales:

● Juan (Grupo: Desarrollo) 


● María (Grupo: Desarrollo) 



● Lorena (Grupo: Desarrollo)


● Verónica (Grupo: RRHH) 















● Diego (Grupo: RRHH)



Crea los siguientes directorios: 

● /srv/Empresa/Desarrollo
● /srv/Empresa/RRHH 


Crea los siguientes subdirectorios:

● /srv/Empresa\Desarrollo\Juan 
● /srv/Empresa\Desarrollo\María 
● /srv/Empresa\Desarrollo\Lorena
● /srv/Empresa\RRHH\Compartido


 Dentro de cada directorio y subdirectorio añade los siguientes ficheros:

● Un fichero de texto plano (.txt)
● Un fichero de imagen (.jpg) 
● Un fichero ejecutable (crea y utiliza un pequeño script en Bash con extensión .sh que devuelva el nombre del PC en el cual se ejecuta)




Bash:


Para Crear un fichero en bash que nos mostre o nombre do ordenador usaremos o comando nano para escribir o código e copiaremos o código da imaxen de arriba, unha vez feito esto empezaremos a copiar e pegar o archivo nos nosos distintos repositorios.


Permisos Linux:







● Actividad 4.5 - Procesos y servicios en Windows 11 Pro: 
Administrador de tareas: 

● Explica brevemente qué información contiene cada una de las pestañas del Administrador de tareas:

 Procesos: Los procesos son los procedimientos que realizan las distintas aplicaciones en el sistema y en la pestaña de procesos nos muestra los que estan funcionando.


 Rendimiento: Donde encontramos el rendimiento del ordenador.

Historial de Aplicaciones: Nos muestra el tiempo de uso de una aplicación principalmente.


Inicio: (Non sei)


Usuario: Muestra los usuarios que están utilizando el ordenador en este momento.



Detalles: Muestra los detalles de los procesos en marcha.


Servicios: (Non sei)









● Documenta cómo puede cerrarse un proceso en primer plano desde la pestaña Procesos. 

Primero que nada iremos a procesos y daremos click derecho sobre el proceso que querramos cerrar y luego pulsaremos en “Finalizar tarea”, listo.




● Documenta cómo se puede consultar el consumo de datos de la interfaz de red (tarjeta de red) de la máquina. Genera tráfico de red e indica cómo los has generado qué parte de la gráfica lo representa. 

En el apartado de rendimiento poderemos observar en Ethernet el flujo de datos si abrimos un navegador web.



● Indica dónde se puede consultar la lista de usuarios conectados a tu equipo. Cierra uno de los procesos en primer plano abiertos por otra persona usuaria del sistema que haya hecho login previamente en la máquina. Después, cierra la sesión de esa persona. Explica ambos procesos.

La lista de usuarios conectados a mi equipo se puede consultar en usuarios.

Para cerrar uno de los procesos abiertos iremos al usuario en concreto buscaremos el proceso que queremos acabar, le daremos click derecho y para finalizar pulsaremos”Finalizar tarea”.


Para desconectar a un usuario buscaremos a dito usuario despois click dereito sobre el e daremoslle a “Cerrar sesión” para finalizar.








 ● Documenta cómo desactivar una aplicación que se muestre en la pestaña “Inicio”. Explica qué efecto va a provocar desactivar esa aplicación. 







● Instala Adobe Acrobat Reader DC y documenta:


 	○ cómo puedes detener el servicio AdobeARMService (Adobe Acrobat Update 
Service). 







○ cómo evitar que el servicio AdobeARMService (Adobe Acrobat Update Service) se 
inicie de manera automática cada vez que arranque el sistema operativo (Pestaña 
“Servicios” -> Abrir servicios). 
















● Actividad 4.6 - Procesos y servicios en Ubuntu Linux 22.04 LTS: 
● Indica los comandos y argumentos utilizados para: 
○ Gestión de Procesos:

■ obtener la lista de procesos que están ejecutándose en el sistema. Explica 
los valores que se muestran respecto de un proceso al invocar el comando.



Explicación de los valores mostrados:

USER: Usuario que inició el proceso.
PID: Identificador único del proceso.
%CPU: Porcentaje de uso de CPU.
%MEM: Porcentaje de uso de memoria.
VSZ: Tamaño virtual del proceso en KB.
RSS: Tamaño residente del proceso en KB.
STAT: Estado del proceso (S: durmiendo, R: corriendo, Z: zombie, etc.).
START: Hora de inicio del proceso.
TIME: Tiempo total de CPU consumido por el proceso.
COMMAND: Nombre del comando o programa asociado al proceso.

■ ejecutar desde consola un programa instalado en el equipo. 

Simplemente poniendo el nombre del programa ya lo ejecutaría.

■ “matar” el proceso correspondiente al programa ejecutado anteriormente. 

Con el comando “pkill” seguido del nombre del programa anterior
 
○ Gestión de Servicios (Daemons):

■ obtener la lista de servicios (daemons) registrados en el sistema. Explica 
los valores que se muestran respecto de un servicio al invocar el comando.

systemctl list-unit-files --type=service

UNIT FILE: Nombre del archivo de unidad asociado al servicio.
STATE: Estado del servicio (enabled, disabled, static, etc.).



■ obtener la lista de servicios (daemons) que están habilitados 

systemctl list-unit-files --type=service | grep enabled

■ obtener la lista de servicios (daemons) deshabilitados. 

systemctl list-unit-files --type=service | grep disabled

○ Monitorización de recursos del sistema:

■ monitoriza en tiempo real el uso de recursos del sistema.
 Explica los valores que se muestran respecto de un proceso al invocar el 
comando. 
		
		comando: top
		
		valores que se repiten anteriormente como:

USER
PID
%CPU
%MEM
COMMAND

Y los demás son:
	
PR: Prioridad del proceso.
NI: Nivel de renic (prioridad ajustada).
VIRT: Tamaño virtual del proceso.
RES: Tamaño residente del proceso.
SHR: Tamaño compartido.
TIME+: Tiempo total de CPU consumido por el proceso.

■ Utiliza intensivamente una aplicación instalada en el sistema mientras 
compruebas cómo se modifican los valores que muestra la herramienta de 
monitorización de recursos.



■ Justifica por qué al utilizar la aplicación estos 
valores aumentan o disminuyen. 






















