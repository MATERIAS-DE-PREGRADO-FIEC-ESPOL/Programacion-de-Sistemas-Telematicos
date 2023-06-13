---
remote_theme: pages-themes/architect@v0.2.0
plugins:
- jekyll-remote-theme
---

[Regresar](/Programacion-de-Sistemas-Telematicos/)

# Trabajo Autónomo 2 Aprovisionamiento de direcciones IPv4 en una red empresarial

## 🎯 Objetivo de Aprendizaje
Efectuar cálculos de direccionamiento IP usando diagramas de arquitectura para la comunicación entre diferentes redes.

**Recursos:** Procesador de texto, papel, lápiz

**Duración:**	8 horas.

**Instrucciones**
- El formato del trabajo tiene habilitado recuadros de color amarillo para que llenen las respuestas de los ejercicios.
- Los trabajos se reciben hasta la fecha planificada en el Aula Virtual.
o	El ejercicio 0 será resuelto en la sesión de clase con la explicación de la docente.
- Coloque el nombre del archivo así “PST_TAA_Apellido”, siendo A el número del trabajo.
- Una vez que haya desarrollado el trabajo, contestará la encuesta de evaluación de los trabajos autónomos ingresando al enlace https://forms.gle/oZnGiwGyDB1LJf5w5


**Introducción**
Dentro de una red es esencial que cada dispositivo posea un identificador único, es por ello que el direccionamiento es una función clave de los protocolos de capa de red. Dado que facilita la distribución y asignación de IP para cada dispositivo dentro de una subred, permitiendo la transmisión de datos entre hosts de la misma red o en redes diferentes. El Protocolo de Internet versión 4 (IPv4) ofrece direccionamiento jerárquico para paquetes que transportan datos. La correcta implementación, diseño y administración de un plan de direccionamiento IPv4 garantiza que las redes puedan operar de manera eficiente y eficaz. 

En cada red IPv4 existen tres tipos de direcciones: 
1.	Dirección de red: Es la dirección que referencia a la red o subred.
2. Dirección de broadcast: Es la dirección reservada para la transmisión de datos a todos los hosts de una red o subred. 
3.	Direcciones de host: Son las direcciones IP válidas que se pueden asignar a los dispositivos que formen parte de la red.

Es importante destacar que una red según su topología y requerimientos puede dividirse en varias subredes, mismas que integran un único sistema. 
En el presente trabajo autónomo se proponen actividades relacionadas al aprovisionamiento de direcciones IPv4 para dispositivos de red, sistemas embebidos en una red empresarial. De manera que el estudiante pueda efectuar el cálculo de subredes a partir de topologías de red para la comunicación entre sistemas telemáticos.


## ACTIVIDADES

### **Topología de la red A [Resuelto]:**
Contiene el proceso explicado con la resolución correspondiente. (Ejemplo)
En la parte 1, se otorgó la dirección de red 192.168.10.0/24 a la subred, con la siguiente topología. Determine la cantidad de redes necesarias y luego diseñe un esquema de direccionamiento adecuado.

<p align="center">
  <img src="../imagenes/t.autonomo2_1.png" alt="trabajo1" width="70%">

<br>
<br>
<br>
Paso 1:	Determine la cantidad de subredes en la topología de la red A.
<br>
a.	¿Cuántas subredes hay? 2 subredes 

<br>
b.	¿Cuántos bits debe tomar prestados para crear la cantidad de subredes requeridas? 
1 bit para la primera subred y 6 bits para la segunda subred.

11111111.11111111.11111111.10000000 = 2<sup>1</sup>=2 subredes, 2<sup>7</sup>=128-2=126 hosts

11111111.11111111.11111111.11111100 = 2<sup>6</sup>=64 subredes, 2<sup>2</sup>=4-2=2 hosts

<br>
c.	¿Cuántas direcciones de host utilizables por subred se encuentran en este esquema de direccionamiento?

2<sup>7</sup>=128-2=126 hosts, 22=4-2=2 hosts

<br>
d.	¿Cuál es la máscara de subred nueva en formato decimal punteado?

 255.255.255.128 - 255.255.255.252

<br>
- e.	¿Cuántas subredes quedan disponibles para usar en el futuro?

192.168.10.132 - 192.168.10.255


Paso 2:	Registre la información de subred.
Complete la siguiente tabla con la información de la subred:

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:0px 0px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:0px 0px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-72fj{border-color:inherit;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-72fj">  Número de <br>subred   </th>
    <th class="tg-72fj">   <br>Dirección de <br>subred   <br></th>
    <th class="tg-72fj"><br>Primera dirección <br>de host utilizable   <br></th>
    <th class="tg-72fj">   Última dirección de <br>host utilizable   </th>
    <th class="tg-72fj">   Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.0</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.126</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.127</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.128</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.129</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.130</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:red">192.168.10.131</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

##1) Topología de la red B (20 puntos)##
La topología de la red de la parte 1 se expandió para admitir el agregado del router R3 y la red complementaria, como se ilustra en la topología siguiente. Utilice la dirección de red 172.32.0.0/16 para proporcionar direcciones a los dispositivos de red y luego diseñe un nuevo esquema de direccionamiento para admitir el requisito de red adicional.


<p align="center">
  <img src="../imagenes/t.autonomo2_2.png" alt="trabajo1" width="90%">

Paso 1: Determine la cantidad de subredes en la topología de la red B.

- a.	¿ Cuántas subredes existen y a qué tipo de clase pertenecen cada una?
     

- b.	¿Cuántos bits debe tomar prestados para crear la cantidad de subredes requeridas? 
     

- c.	¿Cuántas direcciones de host utilizables por subred se encuentran en este esquema de direccionamiento? 
     

- d.	¿Cuál es la máscara de subred nueva en formato decimal punteado? 
     

- e.	¿Cuántas subredes quedan disponibles para usar en el futuro? 
     

Paso 2: Registre la información de subred.
Complete la siguiente tabla con la información de la subred:

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:0px 0px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:0px 0px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-qiwj{border-color:inherit;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-qiwj">   <br>Número de<br> subred   </th>
    <th class="tg-qiwj">   <br>Dirección de<br> subred   </th>
    <th class="tg-qiwj">   <br>Primera dirección<br>de host utilizable   </th>
    <th class="tg-qiwj">   <br>Última dirección <br>de host utilizable   </th>
    <th class="tg-qiwj">   <br>Dirección de<br> broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black">1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black">2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black">3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black">4</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black">5</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-c3ow">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>


### **Topología 2 (20 puntos)**

La topología volvió a cambiar con una LAN nueva agregada al R2 y un enlace redundante entre R1 y R3. Utilice la dirección de red 190.95.0.0/16 para proporcionar direcciones a los dispositivos de red. También proporcione un esquema de direcciones IP que admita estos dispositivos adicionales. Para esta topología, asigne una subred a cada red.

<p align="center">
  <img src="../imagenes/t.autonomo2_3.png" alt="trabajo1" width="80%">

**Paso 1:** Determine la cantidad de subredes en la topología de la red C.


- a.	¿Cuántas subredes existen y a qué tipo de clase pertenecen cada una?.
     

- b.	¿Cuántos bits debe tomar prestados para crear la cantidad de subredes requeridas?.

      
- c.	¿Cuántas direcciones de host utilizables por subred se encuentran en este esquema de direccionamiento?.

     
- d.	¿Cuál es la máscara de subred nueva en formato decimal punteado?. 
     

- e.	¿Cuántas subredes quedan disponibles para usar en el futuro?. 

 
**Paso 2:** Registre la información de subred.

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-pb0m{border-color:inherit;text-align:center;vertical-align:bottom}
.tg .tg-23jf{border-color:inherit;color:#ffffff;font-size:16px;font-weight:bold;text-align:left;vertical-align:bottom}
.tg .tg-8d8j{text-align:center;vertical-align:bottom}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-23jf">Número de <br>subred   </th>
    <th class="tg-23jf">Dirección de <br>subred   </th>
    <th class="tg-23jf">   <br>Primera dirección <br>de host utilizable   </th>
    <th class="tg-23jf">   <br>Última dirección <br>de host utilizable   </th>
    <th class="tg-23jf">   <br>Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black">1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black">2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black">3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black">4</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black">5</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-pb0m">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-8d8j">&nbsp;&nbsp;&nbsp;<br><span style="color:black">6</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-8d8j">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-8d8j">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-8d8j">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-8d8j">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

**Paso 3:**	 Asignar direcciones a los dispositivos de red en las subredes.

a.	Complete la siguiente tabla con las direcciones IP y las máscaras de subred para las interfaces del router:

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-bhg3{border-color:#3166ff;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-rbd8{border-color:#3166ff;text-align:center;vertical-align:bottom}
.tg .tg-s4wa{border-color:#3166ff;text-align:center;vertical-align:middle}
.tg .tg-bidy{border-color:#3166ff;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-bhg3">   <br>Dispositivo   </th>
    <th class="tg-bhg3">   <br>Interfaz   </th>
    <th class="tg-bhg3">   <br>Dirección IP   </th>
    <th class="tg-bhg3">   <br>Máscara de <br>subred   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-s4wa" rowspan="3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">GigabitEthernet 0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/0</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa" rowspan="3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">GigabitEthernet 0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/0</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-s4wa" rowspan="3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">GigabitEthernet 0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-bidy"></td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/0</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-bidy"></td>
  </tr>
  <tr>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-bidy"></td>
  </tr>
</tbody>
</table>


b.	Complete la tabla siguiente con las direcciones IP y las máscaras de subred para los dispositivos en la LAN, como se muestra en la topología.


<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-70h3{border-color:#3166ff;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-bhg3{border-color:#3166ff;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-s4wa{border-color:#3166ff;text-align:center;vertical-align:middle}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-bhg3">   <br>Dispositivo   </th>
    <th class="tg-bhg3">   <br>Interfaz   </th>
    <th class="tg-bhg3">   <br>Dirección IP   </th>
    <th class="tg-bhg3">   <br>Máscara de<br>subred   </th>
    <th class="tg-bhg3">   <br>Gateway<br> predeterminado   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-A</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-B</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">S1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">VLAN 1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-C</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-D</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">S2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">VLAN 1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-E</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">PC-F</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">NIC</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">S3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-70h3">&nbsp;&nbsp;&nbsp;<br><span style="color:black">VLAN 1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-s4wa">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>
First row is a table header 


Paso 4: Análisis

- a.	En caso que la conexión falle entre R3 y R2, ¿es posible seguir enviando información?. Argumente su respuesta.
     
- b.	En caso la conexión falle entre R2 y S2, ¿PC-C y PC-D pueden seguir comunicándose?. Argumente su respuesta.

### **Topología 3 (30 puntos)** 
Utilice la dirección de red 192.170.0.0/16 para proporcionar las direcciones en el diagrama mostrado.
   

<p align="center">
  <img src="../imagenes/t.autonomo2_2.png" alt="trabajo1" width="80%">

**Paso 1:** Determine la cantidad de subredes en la topología de la red D.

a.	¿Cuántas subredes hay? 

     
b.	¿Cuántos bits debe tomar prestados para crear la cantidad de subredes requeridas? 

     
c.	¿Cuántas direcciones de host utilizables por subred se encuentran en este esquema de direccionamiento? 

     
d.	¿Cuál es la máscara de subred nueva en formato decimal punteado?

     
e.	¿Cuántas subredes quedan disponibles para usar en el futuro? 
     

Paso 2: Registre la información de subred.
Complete la siguiente tabla con la información de la subred.

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-merh{border-color:#3166ff;font-weight:bold;text-align:center;vertical-align:bottom}
.tg .tg-bhg3{border-color:#3166ff;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-rbd8{border-color:#3166ff;text-align:center;vertical-align:bottom}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-bhg3">   <br>Número de<br> subred   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>subred   </th>
    <th class="tg-bhg3">   <br>Primera dirección <br>de host utilizable   </th>
    <th class="tg-bhg3">   <br>Última dirección <br>de host utilizable   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">4</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">5</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">6</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">7</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">8</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">9</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

**Paso 3: Análisis**

a.	¿Qué beneficios conlleva que R4 esté en la topología de red?

b.	La organización ha detectado que existen problemas en la red interna. El Departamento Técnico ha descubierto que los problemas se deben a que los paquetes se duplican. Además, de que el tráfico de datos se encuentra congestionado. Usted como Ingeniero en mecatrónica de la organización, habiendo aprendido la matería de Programación de Sistemas Telemáticos, le piden que emita un informe técnico en base a estos inconvenientes. ¿Cuál es el inconveniente presentado en este caso?. 


**4.	Topología de la red E (30 puntos)**
La organización tiene una dirección de red 192.37.0.0/16 que se dividirá como se ilustra en la topología siguiente. Debe elegir un esquema de direccionamiento que pueda admitir la cantidad de redes y hosts en la topología.


<p align="center">
  <img src="../imagenes/t.autonomo2_5.png" alt="trabajo1" width="80%">


**Paso 1:** Determine la cantidad de subredes en la topología de la red E.

a.	¿Cuántas subredes hay existen y a qué tipo de clase pertenecen cada una? 

     
b.	¿Cuántos bits debe tomar prestados para crear la cantidad de subredes requeridas?

     
c.	¿Cuántas direcciones de host utilizables por subred se encuentran en este esquema de direccionamiento? 

     
d.	¿Cuál es la máscara de subred nueva en formato decimal punteado? 

     
e.	¿Cuántas subredes quedan disponibles para usar en el futuro? 
     

Paso 2: Registre la información de subred.
Complete la siguiente tabla con la información de la subred:

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-merh{border-color:#3166ff;font-weight:bold;text-align:center;vertical-align:bottom}
.tg .tg-bhg3{border-color:#3166ff;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-rbd8{border-color:#3166ff;text-align:center;vertical-align:bottom}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-bhg3">   <br>Número de<br> subred   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>subred   </th>
    <th class="tg-bhg3">   <br>Primera dirección <br>de host utilizable   </th>
    <th class="tg-bhg3">   <br>Última dirección <br>de host utilizable   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">4</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">5</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">6</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">7</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">8</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black">9</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-merh">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

Paso 3: Asignar direcciones a los dispositivos de red en las subredes
a.	Complete la siguiente tabla con las direcciones IP y las máscaras de subred para las interfaces del router:

<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-gijy{border-color:#3531ff;text-align:center;vertical-align:bottom}
.tg .tg-70h3{border-color:#3166ff;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-bhg3{border-color:#3166ff;color:#ffffff;font-size:16px;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-rbd8{border-color:#3166ff;text-align:center;vertical-align:bottom}
.tg .tg-3sc7{border-color:#3531ff;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-i5h4{border-color:#3531ff;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-bhg3">   <br>Dispositivo   </th>
    <th class="tg-bhg3">   <br>Interfaz   </th>
    <th class="tg-bhg3">   <br>Dirección IP   </th>
    <th class="tg-bhg3">   <br>Máscara de subred   </th>
    <th class="tg-bhg3">   <br>Dirección de <br>broadcast   </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-70h3" rowspan="4">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">   <br><span style="color:black">GigabitEthernet 0/0</span>   </td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-rbd8">   <br><span style="color:black">GigabitEthernet 0/1</span>   </td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-rbd8">   <br><span style="color:black">Serial 0/0/0</span>   </td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-rbd8">   <br><span style="color:black">Serial 0/0/1</span>   </td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-70h3" rowspan="4">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R2</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">   <br><span style="color:black">GigabitEthernet 0/0</span>   </td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-rbd8">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-gijy">   <br><span style="color:black">GigabitEthernet 0/1</span>   </td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-gijy">   <br><span style="color:black">Serial 0/0/0</span>   </td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-gijy">   <br><span style="color:black">Serial 0/0/1</span>   </td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-3sc7" rowspan="4">&nbsp;&nbsp;&nbsp;<br><span style="color:black">R3</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">   <br><span style="color:black">GigabitEthernet 0/0</span>   </td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black;background-color:#BFBFBF">     </span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black">GigabitEthernet 0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
  </tr>
  <tr>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/0</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
  </tr>
  <tr>
    <td class="tg-gijy">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Serial 0/0/1</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
    <td class="tg-i5h4">   <br><span style="color:black;background-color:#BFBFBF">     </span>   </td>
  </tr>
</tbody>
</table>


Paso 4: Análisis.
a.	La organización quiere hacer un inventario para reconocer las computadoras de la Sucursal 1 que estén activas y conectados a la subred. ¿Qué acción recomendaría en este caso?.
     

**Reflexiones**
1.	¿Qué información es necesaria para determinar un esquema de direccionamiento adecuado en una red?
     

2.	Una vez asignadas las subredes, ¿se utilizarán todas las direcciones de host en cada subred?.
     

3.	Explique las funciones de las capas del modelo OSI.
     

4.	En caso de que requiera una red sin conexión a internet con la menor cantidad de hosts posibles, ¿Cúal es la máscara de subred que usaría?. Argumente su respuesta.


