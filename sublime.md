# Instalación de SublimeText
<img src="https://imgur.com/PaitXUM.png">

### Introducción

En esta tarea seguimos paso a paso el procedimiento para instalar SublimeText en Linux Ubuntu.

Sublime Text es un potente editor de código multiplataforma, ligero y con pocas concesiones a las florituras. Está construido a partir de componentes personalizados, que proporciona una capacidad de respuesta inigualable. Su interfaz de color oscuro y la riqueza de coloreado de la sintaxis centra nuestra atención completamente. Desde un potente kit de herramientas de interfaz de usuario multiplataforma personalizado hasta un motor de resaltado de sintaxis sin igual, Sublime Text establece el estándar de rendimiento.

### Pasos
Se debe de ejecutar cada uno de los siguientes pasos para la instalación:

#### Paso 1:

``
sudo apt-get upgrade
``

![1](https://user-images.githubusercontent.com/91209203/135347601-e8d2f380-3801-4511-8494-ca48f027c54c.png)
![1 2](https://user-images.githubusercontent.com/91209203/135347685-90997c3e-42b0-487d-9c19-2c1597571286.png)

#### Paso 2:

``
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
``

![2](https://user-images.githubusercontent.com/91209203/135347738-e553d3f4-0df6-4f65-9d2e-26868d446969.png)

#### Paso 3:

``
sudo apt-get install apt-transport-https
``

![3](https://user-images.githubusercontent.com/91209203/135347772-0f3beeab-efba-4ef9-be5b-496c9b539eaa.png)

#### Paso 4:

``
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
``

![4](https://user-images.githubusercontent.com/91209203/135347805-407837e6-4d23-46ed-9e22-ae1284d10e7e.png)

#### Paso 5:

``
sudo apt update
``

![5](https://user-images.githubusercontent.com/91209203/135347823-d1acd305-5583-4ce2-b583-976503961003.png)

#### Paso 6:

``
sudo apt install sublime-text
``

![6](https://user-images.githubusercontent.com/91209203/135347850-43455ffc-192b-455c-b2f8-a5f9e8450ca9.png)

#### Paso 7:
Pulsa el símbolo de ubuntu en la esquina superior izquierda en azul y busca sublime.

![7](https://user-images.githubusercontent.com/91209203/135347878-605f91c4-dedf-4cbc-9c9a-199a7a7368be.png)






