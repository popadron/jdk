# Instalación de JDK en el SO
                                                                              Patricia Isabel Ojeda Padrón 1ºDAM ETS

ÍNDICE
1. Introducción
2. Ejercicio
  2.1 ¿Cómo instalar una versión específica de Java?
  2.2 Configuración de las variables de entorno
  2.3 Listar las versiones de OpenJDK instaladas
  

1. Introducción

Java , sin dudas, es un lenguaje de programación muy usado para diversas utilidades como pueden ser la elaboración de aplicaciones de productividad ,como hojas de cálculo, entretenimiento ,un ejemplo sería el uso de Java para que varios juegos se puedan ejecutar en diferentes plataformas,(también conocido como multiplataforma), entre otros muchos usos.

La instalación de Java es una tarea esencial, por este motivo se expondrá de forma detallada como instalar Java en nuestro SO (Sistema Operativo) con el JDK (Java Development Kit), es decir el kit de desarrollo de Java, y el entorno de ejecución JRE (Java Runtime Environment).

2. Ejercicio

Lo primero debemos de actualizar el sistema con:

``
sudo apt-get update
``

![1](https://user-images.githubusercontent.com/91209203/134744146-5c3d7d7a-3612-4f73-8594-2209e1bc1c78.png)

E instalamos Java con este comando:

``
sudo apt-get install default-jdk
``

![2 1](https://user-images.githubusercontent.com/91209203/134744684-c9d20736-9c08-44d3-a9f4-ae8d44fab736.png)
![2 3](https://user-images.githubusercontent.com/91209203/134744690-7be8ae1b-760c-4fb9-93a1-1b83b480e520.png)


Para comprobar que tenemos instalado Java en nuestro sistema ejecutamos:

``
java --version
``

![3](https://user-images.githubusercontent.com/91209203/134744709-c5743c25-628f-4690-8f94-3b25407805fe.png)

2.1 ¿Cómo instalar una versión específica de Java?

Para instalar Ubuntu Java Open JDK ("la que utilizaremos en 1º").
 - OpenJDK:
   - 11 
   ``
   sudo apt install openjdk-11-jdk
   ``
   
   ![4](https://user-images.githubusercontent.com/91209203/134744890-4ac521eb-71a8-4acd-b43f-5fe15a67c2db.png)

   
    - 9 
   ``
   sudo apt install openjdk-9-jdk
   ``
   
   ![5](https://user-images.githubusercontent.com/91209203/134744954-e6360bc2-1fa5-437a-b541-d9b70c22b5ca.png)
   
   Linux Mint no tiene el paquete de la versión 9.
   
    - 8
   ``
   sudo apt install openjdk-8-jdk
   ``
   
   ![6 1](https://user-images.githubusercontent.com/91209203/134744973-e58d3a8f-eb00-4769-97f4-058119ff550b.png)
   ![6 2](https://user-images.githubusercontent.com/91209203/134745111-89bb6db4-66a4-4842-a71e-507ef6086a95.png)

   
La versión que se debe de trabajar es la versión 8. Para ello verificaremos la versión de java que se esta ejecutando con la sentencia:
``
  java --version
``

![7](https://user-images.githubusercontent.com/91209203/134745201-5c7a29b9-b3cb-4afa-bcb1-68bd6d09966c.png)

En caso que no se ejecuta la versión 8 se debe configurar las variables de entorno.

2.2 Configuración de las variables de entorno

 El siguiente paso consiste en establecer  las variables de entorno. Es necesario porque cuando se usa Java, Linux necesita saber dónde está ubicado el programa para ejecutarlo y qué versión de Java usar de forma predeterminada. Para modificar esto, usaremos el editor de texto nano. Primero, abra el archivo en Nano.

2.3 Listar la versiones de OpenJDK instaladas

 Ejecuta el siguiente comando para verificar que se han descargado las diferentes versiones de OpenJDK.

``
 ls /usr/lib/jvm
``

![8](https://user-images.githubusercontent.com/91209203/134745256-d135f440-3b9b-4bd2-ac24-a0e81d941511.png)

Actualización de las variables de entorno

 Edita y modifica el fichero profile, con los comandos:

``
nano /etc/profile
``

![9 1](https://user-images.githubusercontent.com/91209203/134745267-f0382f83-8754-4272-b797-69a609aba837.png)


y realiza los siguientes cambios y seleccionando la versión 8:

``
# Java version
JAVA_HOME=/usr/lib/jvm/_____openJdk_____
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
``

![9 2](https://user-images.githubusercontent.com/91209203/134745274-5cb0f6a5-ae41-49ff-95af-d2e93baec4d5.png)
