---
remote_theme: pages-themes/architect@v0.2.0
plugins:
- jekyll-remote-theme
---

[Regresar](/Programacion-de-Sistemas-Telematicos/)

# Trabajo Autónomo 1 División de subredes con direccionamiento IPv4

## 🎯 Objetivo de Aprendizaje
Efectuar cálculos de direccionamiento IP usando diagramas de arquitectura para la comunicación entre diferentes redes.

**Recursos:** Procesador de texto, lápiz, papel, calculadora.

**Duración:** 6 horas.

**Instrucciones**

- Mantener el formato del trabajo proporcionado.
Los trabajos se reciben hasta la fecha planificada en el Aula Virtual.
- El ejercicio 0 será resuelto en la sesión de clase con la explicación de la docente.
- Coloque el nombre del archivo así “PST_P#_TAA_Apellido_Nombre”, siendo # el paralelo, A el número del trabajo.
- Una vez que haya desarrollado el trabajo, cada integrante del grupo contestará la encuesta de evaluación de los trabajos autónomos ingresando a https://bit.ly/3jIH3yJ


**Introducción**

Una dirección IP se utiliza para identificar a un dispositivo en una red, por lo que es única dentro de los límites de dicha red. La dirección se compone de 32 bits binarios, mismos que pueden dividirse en una porción correspondiente a la red y otra a hosts, con la ayuda de una máscara de subred.
Los 32 bits binarios se encuentran divididos en 4 octetos, cada uno con 8 bits. Cada octeto binario se convierte a decimal (en el rango de 0-255) y se separa por un punto, es así como una IP puede representarse de la siguiente manera: 192.168.19.0/26, donde:
192.168.10.10/26


Los octetos binarios se convierten a decimales, considerando que los bits desde la derecha a la izquierda siguen la secuencia de una potencia de base 2, como se muestra en la Figura 1.



Figura 1. Traducción de sistema binario a decimal

Según la máscara de subred, las direcciones IP pueden clasificarse en clases, desde la A hasta la E (Figura 2). La clase de una dirección IP se puede determinar a partir de los tres bits del extremo 

izquierdo en el primer octeto. 

El siguiente trabajo autónomo tiene como propósito que el estudiante pueda desarrollar actividades relacionadas al cálculo de división de subredes usando direccionamiento IPv4 para un sistema en red.

## ACTIVIDADES

1.	Efectuar el cálculo de división de subredes usando el direccionamiento IPv4 propuesto en los 5 escenarios. A continuación, se presenta un escenario con la resolución, el cual fue explicado durante la sesión de clase **(30 puntos)**: 

<<<<<<< Updated upstream
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
<<<<<<< HEAD
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 0 (Resuelto)</span></th>
=======


**Escenario 1**

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7btt" colspan="2"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Escenario 1</span></th>
>>>>>>> Stashed changes
=======
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 0 [Resuelto]</span></th>
>>>>>>> 36626492f1ca1e3503cd75ef6d3bbf475b291de4
  </tr>
</thead>
<tbody>
  <tr>
<<<<<<< Updated upstream
    <td class="tg-mcqj">Número de segmentos físicos:</td>
    <td class="tg-73oq">5</td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-73oq">5000</td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.0</span></td>
  </tr>
  <tr>
<<<<<<< HEAD
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-73oq">2=8 subredes</td>
  </tr>
  <tr>
    <td class="tg-mcqj">Máscara de subred propuesta:</td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none">11111111.11111111.</span><span style="font-weight:700">11100000</span>.00000000<br><br><span style="font-weight:400;font-style:normal;text-decoration:none">=255.255.</span>224.0<br><span style="font-weight:400;font-style:normal;text-decoration:none">= Prefijo CIDR= /19</span><br><br><span style="font-weight:400;font-style:normal;text-decoration:none">Explicación: Una vez que tengo cuantas subredes y hosts me pide el ejercicio, tomo los 3 bits encendidos para subredes y 13 bits apagados para hosts, pero solo tomaré el tercer octeto que tiene la parte variable con los 5 bits apagados para formar 2</span><br>5 = 32 saltos como se muestra a continuación.</td>
=======
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-73oq">2<sup>3</sup> = 8 subredes</td>
  </tr>
  <tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-73oq">2<sup>13</sup>= 8192 - 2 = 8190 hosts subredes</td>
  </tr>
  <tr>
    <td class="tg-mcqj">Máscara de subred propuesta:</td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none">11111111.11111111.</span><span style="font-weight:700">11100000</span>.00000000<br><br><span style="font-weight:400;font-style:normal;text-decoration:none">= 255.255.</span>224.0<br><span style="font-weight:400;font-style:normal;text-decoration:none">= Prefijo CIDR= /19</span><br><br><span style="font-weight:400;font-style:normal;text-decoration:none">Explicación: Una vez que tengo cuantas subredes y hosts me pide el ejercicio, tomo los 3 bits encendidos para subredes y 13 bits apagados para hosts, pero solo tomaré el tercer octeto que tiene la parte variable con los 5 bits apagados para formar 2<sup>5</sup> = 32 saltos como se muestra a continuación.</td>
>>>>>>> 36626492f1ca1e3503cd75ef6d3bbf475b291de4
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.1 – 152.77.31.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.32.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.32.1 – 152.77.63.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.64.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.64.1 – 152.77.95.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.96.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.96.1 – 152.77.127.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.128.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.128.1 – 152.77.159.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.160.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.160.1 – 152.77.191.254</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.192.0</span></td>
    <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.192.1 – 152.77.223.254</span></td>
  </tr>
  <tr>
  <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.</span><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:#0FF">224</span><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">.0</span></td>
  <td class="tg-73oq"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.224.1 – 152.77.255.254</span></td>
  </tr>
</tbody>
<<<<<<< HEAD
</table>
=======
   

**Escenario 2**
=======

<br>
<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 1</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-mcqj">Número de segmentos físicos:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">28</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">1981</span></td>
  </tr>
  <tr>
        <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">176.7.0.0</span></td>
  </tr>
  <tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
     <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máscara de subred propuesta: </span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">          </span></td>
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
</tbody>
</table>

<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 2</span></th>
  </tr>
</thead>
<tbody>
  <tr>
   <td class="tg-mcqj">Número de segmentos físicos:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">30</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">5</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">210.20.10.0</span></td>
  </tr>
  <tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
     <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máscara de subred propuesta: </span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">          </span></td>
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
</tbody>
</table>

<br>
>>>>>>> 36626492f1ca1e3503cd75ef6d3bbf475b291de4

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 3</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-mcqj">Número de segmentos físicos:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">58</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">185230</span></td>
  </tr>
  <tr>
  <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">180.0.0.0</span></td>
  </tr>
<tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
     <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máscara de subred propuesta: </span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">          </span></td>
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
</tbody>
</table>

<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 4</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-mcqj">Número de segmentos físicos:</span></td>
    <td class="tg-0lax" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">140</span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-0lax" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">180</span></td>
  </tr>
  <tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0lax" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">195.18.5.0</span></td>
  </tr>
<tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
     <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máscara de subred propuesta: </span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">          </span></td>
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
</tbody>
</table>

<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-l49g{border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-mcqj{border-color:#000000;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-mqa1{border-color:#000000;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 646px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
</colgroup>
<thead>
  <tr>
    <th class="tg-l49g" colspan="2"><span style="font-weight:700">Escenario 5</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-mcqj">Número de segmentos físicos:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">3</span></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">56</span></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">192.115.30.0</span></td>
    <td class="tg-0lax"></td>
  </tr>
<tr>
<td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts por subred:</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
     <td class="tg-mcqj"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máscara de subred propuesta: </span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">          </span></td>
  </tr>
  <tr>
    <td class="tg-mqa1">Subred</td>
    <td class="tg-mqa1"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
</tbody>
</table>

<br>

2. Determine  la  dirección de subred,  dirección  de  difusión (broadcast) y el rango de hosts válidos **10 puntos**: 
<br>
<br>
- 180.42.67.2/19

- 176.128.64.40/23

- 107.194.140.27/14

- 230.53.192.37/10

- 192.18.81.4/17

<br>
<br>
3. Dada una red de Clase B y los bits de red identificados (CIDR), complete la siguiente tabla para identificar la máscara de subred y el número de direcciones de host posibles para cada máscara **(10 puntos)**:

<br>
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-1wig{font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-l49g" colspan="1"><span style="font-weight:700">CIDR</span></th>
    <th class="tg-l49g" colspan="1"><span style="font-weight:700">Máscara de subred (formato decimal)</span></th>
    <th class="tg-l49g" colspan="1"><span style="font-weight:700">Número de host por subred (2<sup> x </sup> - 2)</span></span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">/14</span></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">/26</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">/18</span></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">/20</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
  <tr>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">/31</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">     </span></td>
  </tr>
</tbody>
</table>

<br>
<br>

<<<<<<< HEAD
>>>>>>> Stashed changes
=======
4. La empresa de desarrollo de software AditaTech S.A. tiene 3 puntos que son la matriz en Guayaquil, las sucursales en Quito y Cuenca. La dirección de red usada en los puntos es 192.168.1.0/24. Acorde a la topología de la red proporcionada, identifique los problemas existentes detallando en qué capa del Modelo OSI ocurren estos problemas, y a la vez proponga una solución a cada problema. **(40 puntos)**

<p align="center">
  <img src="../imagenes/trabajo1_actividad4_diagrama.png" alt="trabajo1" width="80%">

<br>
<br>

## Desafío

5. Determinar la IP pública y privada de su dispositivo de usuario final. Se admiten imágenes en las respuestas. **(10 puntos)**
>>>>>>> 36626492f1ca1e3503cd75ef6d3bbf475b291de4
