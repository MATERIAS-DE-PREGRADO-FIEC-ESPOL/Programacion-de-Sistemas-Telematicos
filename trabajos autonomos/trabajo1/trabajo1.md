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


