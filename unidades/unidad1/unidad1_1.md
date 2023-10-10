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

# 1.1. Arquitectura de comunicación de datos
- [¿Qué es la Red?](#definicion)
    - [Redes locales](#redes_locales)
    - [Conexiones](#conexiones)
    - [Datos](#datos)
- [Comunicación en Red](#comunicacion)
- [Protocolos de Red](#protocolos)
- [Componentes de Red](#componentes)
- [¿Qué es un sistema telemático?](#sistema_telematico)
  - [¿Cómo funciona la telemática?](#telematica)
- [Referencias](#referencias)

<a name="definicion"> </a>
## 🌐 ¿Qué es la Red?

<a name="redes_locales"> </a>

### **Redes locales**
Las redes locales vienen en todos los tamaños: entre pares (dos dispositivos interconectados) o redes domésticas, hasta redes SOHO y redes de organizaciones grandes.


<a name="conexiones"> </a>

### **Conexiones**
Todos los tipos de dispositivos se conectan a redes locales.


<a name="datos"> </a>

### **Datos**
La mayoría de la gente utiliza redes para transmitir sus propios datos para compartirlos con otras personas o para almacenarlos a largo plazo.

<p align="center">
  <img src="../gifs/networks.gif" alt="networks" width="60%">
</p>


<a name="comunicacion"> </a>

## 🌐 Comunicación en red
- Un emisor y un receptor identificados
- Método de comunicación acordado
- Idioma y gramática común
- Velocidad y momento de entrega
- Requisitos de confirmación o acuse de recibo

<p align="center">
  <img src="../imagenes/communication.png" alt="communications" width="60%">
</p>


<a name="protocolos"> </a>

## 🌐 Protocolos de red
- Formato o estructuración del mensaje.
- Proceso por el cual los dispositivos de red comparten información sobre las rutas con otras redes.
- Cómo y cuándo se transmiten mensajes de error y del sistema entre los dispositivos.
- La configuración y la terminación de sesiones de transferencia de datos.

<p align="center">
  <img src="../imagenes/protocols.png" alt="protocols" width="70%">
</p>

<a name="componentes"> </a>
## 🌐 Componentes de Red
<p align="center">
  <img src="../imagenes/configip.jpg" style="width: 40%; height: 200px; float: right; padding: 15px;" alt="configip">
</p>

La configuración IP consta de tres partes, que deben ser correctas para que el dispositivo envíe y reciba información por 
la red:
- Dirección IP: Identifica al host en la red.
- Máscara de subred: Identifica la red a la 
que está conectado el host.
- Gateway predeterminado: Identifica el dispositivo de red que utiliza el host para 
acceder a Internet o a otra red remota.

Una dirección IP puede configurarse manualmente o ser asignada automáticamente por otro dispositivo (DHCP).

<p align="center">
  <img src="../imagenes/componentes_red.png" alt="componentes" width="60%">
</p>


<a name="sistema_telematico"> </a>

## 🌐 ¿Qué es un sistema telemático?
Es un sistema compuesto por dispositivos interconectados a la red de datos, diseñados para realizar una función específica siendo una combinación de ambos hardware y software.

- Puede o no puede contener un sistema operativo para el funcionamiento.
- El firmware es pre-programado y no alterado por el usuario final.
- Los requerimientos de aplicaciones específicas como uso de rendimiento, energía, memoria son factores decisivos.

<p align="center">
  <img src="../imagenes/sistema_telematico.png" alt="telematico" width="50%">
</p>


<a name="telematica"> </a>

## 🌐 ¿Cómo funciona la telemática?
En esencia, un sistema telemático incluye un dispositivo de seguimiento instalado en un vehículo que permite enviar, recibir y almacenar datos telemétricos. Se conecta a través del puerto de diagnóstico a bordo (ODBII) o CAN-BUS del propio vehículo con una tarjeta SIM, y un módem a bordo permite la comunicación a través de una red inalámbrica.

El dispositivo recoge datos GPS y otros datos específicos del vehículo y los transmite a un servidor centralizado a través de una red de telefonía móvil o comunicación por satélite. El servidor interpreta los datos y los muestra a los usuarios finales a través de sitios web seguros y aplicaciones optimizadas para teléfonos inteligentes y tabletas.

Los datos telemáticos capturados pueden incluir ubicación, velocidad, tiempo de ralentí, aceleración o frenado bruscos, consumo de combustible, averías del vehículo y otros datos. Cuando se analiza en busca de eventos y patrones concretos, esta información puede proporcionar información detallada sobre toda una flota.

<p align="center">
  <img src="../imagenes/unidad1_2_vehicle_tracking.png" alt="telematica" width="100%">
</p>