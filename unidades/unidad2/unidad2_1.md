---
remote_theme: pages-themes/architect@v0.2.0
plugins:
- jekyll-remote-theme
---

[Regresar](/Programacion-de-Sistemas-Telematicos/)

# Unidad 2 Administración de tecnologías web

## 🎯 Objetivo de Aprendizaje
Al finalizar la clase el estudiante será capaz de:
- Utilizar tecnologías web basadas en red para el monitoreo del estado y la información de los dispositivos telemáticos.

# 2.1 Aplicaciones basadas en red
- [Introducción](#introduccion)
	- [Visual Studio Code](#vsc)
	- [Virtualización](#virtualizacion)
	- [Infraestructura basada en contenedores](contenedores)


<a name="introduccion"> </a>

## 🌐 Introducción

<p align="center">
  <img src="../imagenes/unid2_1_aplicaciones_red.png" alt="modelos_red" width="100%">
</p>


<a name="vsc"> </a>

### 🕸️ Visual Studio Code 

- Editor de código fuente ligero.
- Disponible para Windows, macOS y Linux.
- Soporte integrado para JavaScript, TypeScript y Node.js

<p align="center">
  <img src="../imagenes/unid2_1_vsc.png" alt="modelos_red" width="100%">
</p>


<a name="virtualizacion"> </a>

### 🕸️ Virtualización

<p align="center">
  <img src="../imagenes/unid2_1_virtualizacion.png" alt="modelos_red" width="100%">
</p>

+ Virtualización es uno de los avances más significativos que ha contribuido a la habilitación de la computación en la nube.
+ Virtualización es el proceso en el que una computadora física, llamada host, ejecuta múltiples copias de un sistema operativo, donde cada copia es llamada guest  (invitado).
+ Cada invitado obtiene sus propios recursos virtuales y se comunica con la red por su cuenta.
+ El sistema host ejecuta un software llamado hypervisor que cambia los recursos entre los distintos invitados.
+ Con el software de compañías como VMWare y Openbox, puede tomar una CPU potente y usarla para ejecutar múltiples máquinas virtuales.
+ Esto optimiza el uso de los recursos físicos y reduce drásticamente los costos con respecto a la máquina anterior, un modelo de sistema operativo.


<a name="contenedores"> </a>

## 🕸️ Infraestructura basada en contenedores

<p align="center">
  <img src="../imagenes/unid2_1_infraestructura.png" alt="modelos_red" width="100%">
</p>

- Un contenedor generalmente representa solo una aplicación o un grupo de aplicaciones.
- El valor de usar contenedores es que se incluyen todas las bibliotecas y binarios que necesita para ejecutar la aplicación, por lo que el usuario no tiene que realizar ese paso de instalación adicional.
- El software para crear y administrar u orquestar contenedores está disponible en Docker, AWS (Elasticized Container Service), Microsoft (Azure Container Service) y otros.
- Los programadores están creando software que realiza una única función de un sistema (como el procesamiento o almacenamiento de la base de datos) que se ejecuta en un contenedor.
- Estos contenedores están organizados en "pods" que se ejecutan dentro de un "nodo" y pueden comunicarse entre sí y con el mundo exterior si es necesario.
-  Linux es la tecnología subyacente que hace que la tecnología de contenedores funcione.
- Bare-Metal Deployment, es un sistema informático o una red en la que una máquina virtual se instala directamente en el hardware en lugar de dentro del sistema operativo (SO) del host.