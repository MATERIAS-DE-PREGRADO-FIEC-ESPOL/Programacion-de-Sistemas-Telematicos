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

# 1.2. Modelos de Estructura de Red
- [Modelo de Estructura de Red](#modelo_red)
- [Referencias](#referencias)

<a name="modelo_red"> </a>
## 🌐 Modelos de estructura de red
<p align="center">
  <img src="../imagenes/modelos_red.png" alt="modelos_red" width="100%">
</p>


El Modelo OSI (Open Systems Interconnection) contiene 7 capas que se describen a continuación:

- La capa física, que es la capa inferior del modelo OSI, se ocupa de la transmisión y recepción del flujo de bits sin estructurar a través de un medio físico. Describe las interfaces eléctricas/ópticas, mecánicas y funcionales con el medio físico y transporta las señales para todas las capas superiores.

- La capa de enlace de datos proporciona una transferencia sin errores de tramas de datos de un nodo a otro a través de la capa física, lo que permite a las capas superiores asumir una transmisión prácticamente sin errores a través del enlace.

- La capa de red controla el funcionamiento de la subred, decidiendo qué ruta física deben seguir los datos en función de las condiciones de la red, la prioridad del servicio y otros factores.

- La capa de transporte garantiza que los mensajes se entreguen sin errores, en secuencia y sin pérdidas ni duplicaciones.

- La capa de sesión permite el establecimiento de sesiones entre procesos que se ejecutan en estaciones diferentes.

- La capa de presentación da formato a los datos que se presentan a la capa de aplicación. Puede considerarse como el traductor de la red. Esta capa puede traducir los datos de un formato utilizado por la capa de aplicación a un formato común en la estación emisora y, a continuación, traducir el formato común a un formato conocido por la capa de aplicación en la estación receptora.

- La capa de aplicación sirve de ventana para que los usuarios y los procesos de aplicación accedan a los servicios de red.