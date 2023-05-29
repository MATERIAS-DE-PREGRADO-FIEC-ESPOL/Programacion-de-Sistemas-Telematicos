# Trabajo Autónomo:
  ## Unidad 1 Introducción a Sistemas Telemáticos
### Objetivo de Aprendizaje:
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

1.	Efectuar el cálculo de división de subredes usando el direccionamiento IPv4 propuesto en los 5 escenarios. A continuación, se presenta un escenario con la resolución, el cual fue explicado durante la sesión de clase: **(30 puntos)**

**Escenario 0 (Resuelto)**


|Escenario 0 (Resuelto)|
|---|---|
|Número de segmentos físicos:|5|
|---|---|
|Máximo número de hosts / Segmento físico: |5000|
|---|---|
|Dirección de red:|152.77.0.0|
|Número de subredes soportadas:
    23=8 subredes
Máximo número de hosts por subred:
213=8192 - 2=8190 hosts
Máscara de subred propuesta:

11111111.11111111.11100000.00000000

Máscara de subred
=255.255.224.0
Prefijo CIDR= /19

Explicación: Una vez que tengo cuantas subredes y hosts me pide el ejercicio, tomo los 3 bits encendidos para subredes y 13 bits apagados para hosts, pero solo tomaré el tercer octeto que tiene la parte variable con los 5 bits apagados para formar 25=32 saltos como se muestra a continuación.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-1wig{font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 873px">
<colgroup>
<col style="width: 304px">
<col style="width: 342px">
<col style="width: 227px">
</colgroup>
<thead>
  <tr>
    <th class="tg-c3ow" colspan="3"><span style="font-weight:700">Escenario 0 (Resuelto)</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-fymr">Número de segmentos físicos:</td>
    <td class="tg-0pky" colspan="2">5</td>
  </tr>
  <tr>
    <td class="tg-fymr"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Máximo número de hosts / Segmento físico:</span></td>
    <td class="tg-0pky" colspan="2">5000</td>
  </tr>
  <tr>
    <td class="tg-fymr"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Dirección de red:</span></td>
    <td class="tg-0pky" colspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.0</span></td>
  </tr>
  <tr>
    <td class="tg-1wig"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de subredes soportadas:</span></td>
    <td class="tg-0lax" colspan="2">23=8 subredes</td>
  </tr>
  <tr>
    <td class="tg-1wig">Máscara de subred propuesta:</td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none">11111111.11111111.</span><br><span style="font-weight:700;font-style:normal;text-decoration:none">111</span><br><span style="font-weight:700;font-style:normal;text-decoration:underline">00000</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">.00000000</span><br><br><span style="font-weight:400;font-style:normal;text-decoration:none">Máscara de subred</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">=255.255.</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">224</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">.0</span><br><span style="font-weight:400;font-style:normal;text-decoration:none">Prefijo CIDR= /19</span><br><br><span style="font-weight:400;font-style:normal;text-decoration:none">Explicación: Una vez que tengo cuantas subredes y hosts me pide el ejercicio, tomo los 3 bits encendidos para subredes y 13 bits apagados para hosts, pero solo tomaré el tercer octeto que tiene la parte variable con los 5 bits apagados para formar 2</span><br>5 = 32 saltos como se muestra a continuación.</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-amwm" rowspan="9">Rangos de host válidos por subred:</td>
    <td class="tg-1wig">Subred</td>
    <td class="tg-amwm"><span style="font-weight:700;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Primera dirección host - Última dirección host válida</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.0</span></td>
    <td class="tg-0lax"><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.0.1 – 152.77.31.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.32.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.32.1 – 152.77.63.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.64.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.64.1 – 152.77.95.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.96.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.96.1 – 152.77.127.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.128.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.128.1 – 152.77.159.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.160.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.160.1 – 152.77.191.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.192.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.192.1 – 152.77.223.254</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.</span><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:#0FF">224</span><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">.0</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">152.77.224.1 – 152.77.255.254</span></td>
  </tr>
</tbody>
</table>

