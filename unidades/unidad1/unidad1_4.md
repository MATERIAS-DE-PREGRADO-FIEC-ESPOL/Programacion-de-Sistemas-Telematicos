---
remote_theme: pages-themes/architect@v0.2.0
plugins:
- jekyll-remote-theme
---

[Regresar](/Programacion-de-Sistemas-Telematicos/)

# Unidad 1: Introducción a sistemas telemáticos

## 🎯 Objetivo de Aprendizaje
Al finalizar la clase el estudiante será capaz de:
- Efectuar cálculos de direccionamiento IP usando diagramas de arquitectura para la comunicación entre diferentes redes.

# 1.4. Administración de sistemas operativos en red
- [Administración de sistemas operativos en red](#sistemas_operativos)
  - [Recursos computacionales para Linux](#recursos)
  - [Tipos de Instalación](#instalacion)
  - [Particiones en un disco duro](#particiones)
  - [Herramientas de virtualización](#herramientas_virtualizacion)
- [Referencias](#referencias)

<a name="sistemas_operativos"> </a>

## 🌐 Administración de sistemas operativos en red
- Como todo sistema operativo, Linux tiene exigencias en el hardware donde se ejecutará, es por eso que antes de que se precipite e instale el software, tiene que asegurarse de estos requerimientos y limitaciones de hardware de Linux.

- Considerando que Linux fue desarrollado por sus usuarios, en la mayoría de las ocasiones el hardware soportado por Linux es únicamente aquél al que usuarios y desarrolladores tiene realmente acceso. Según pasa el tiempo aumenta el hardware soportado por Linux.

- Un inconveniente en el soporte de hardware bajo Linux, es que muchas compañías han decidido conservar las especificaciones del interfaz de su hardware como propietario. Como consecuencia de esto, los desarrolladores voluntarios de Linux simplemente no pueden escribir controladores (drivers) para estos periféricos (y si pudieran, tales controladores serían propiedad de la compañía dueña de la interfaz, lo cual violaría el GPL).


<a name="recursos"> </a>

### 💻 Recursos computacionales para Linux
Previo a la instalación de una distribución de Linux para un servidor es necesario considerar los recursos básicos de hardware como sigue:

- CPU: Intel Celeron de 2.4 Ghz
 -Procesador: Pentium IV
- Disco duro: 40 GB
- Memoria: 4 GB
- Tarjetas de Red: 2 NICs PCI Realtek/basadas en chip Realtek o Via


<a name="instalacion"> </a>

### 💻 Tipos de Instalación
- Estación de trabajo: Más adecuada si es nuevo en el mundo de Linux y quiere probarlo. 
- Servidor: Si desea que su sistema funcione como un servidor basado en Linux utilizando servicios específicos.
- Portátil: Instalación sencilla en ordenadores portátiles. 
- Personalizada: Mayor flexibilidad en el proceso de instalación. Podrá elegir su esquema de particionamiento, los paquetes que desea instalar y mucho más. 
- Actualización: Para actualizar rápidamente a los últimos paquetes y versiones del kernel. 


<a name="particiones"> </a>

### 💻 Particiones en un disco duro
- Hay tres clases de particiones: primarias, extendidas y lógicas.
- Muchas distribuciones necesitan que se creen a mano las particiones de Linux utilizando el programa fdisk. Otras pueden crearlas automáticamente.
- En el primer sector del disco está el registro de arranque maestro “MBR” junto a la tabla de particiones.

<p align="center">
  <img src="../imagenes/unidad1_3_particion.png" alt="industria" width="100%">
</p>

En Linux los manejadores, que se encuentran en el directorio /dev, se usan para comunicarse con los dispositivos de su sistema como discos duros. Los discos duros SSD se nombran con /dev/disksn.

<p align="center">
  <img src="../imagenes/unidad1_3_df.png" alt="industria" width="100%">
</p>

Por lo general se crean dos particiones para Linux, una para ser usada como sistema de ficheros raíz y la otra como espacio de intercambio “swap”.
La partición swap, es un espacio de intercambio de ayuda a la memoria RAM a pasar datos temporalmente al disco duro.

<p align="center">
  <img src="../imagenes/unidad1_3_particiones_servidor.png" alt="industria" width="100%">
</p>


<a name="herramientas_virtualizacion"> </a>

### 💻 Herramientas de virtualización
- [VirtualBox](https://www.virtualbox.org)
- [Vmware](https://www.vmware.com)
- [Microsoft Azure](https://azure.microsoft.com/)

<p align="center">
  <img src="../imagenes/unidad1_3_virtualization_tools.png" alt="industria" width="70%">
</p>


<a name="referencias"> </a>

## 📚 Referencias
- [VirtualBox](https://www.virtualbox.org)
- [Vmware](https://www.vmware.com)
- [Microsoft Azure](https://azure.microsoft.com/)
- [Submarine Cable Map from](https://www.submarinecablemap.com/)