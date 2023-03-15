# OBJETIVO DE APRENDIZAJE
Utilizar tecnologías web basadas en red para el monitoreo del estado y la información de los dispositivos telemáticos.
# Aplicaciones basadas en red
imagen
# Visual Studio Code Aplicaciones basadas en red
+ Editor de código fuente ligero.
+ Disponible para Windows, macOS y Linux.
+ Soporte integrado para JavaScript, TypeScript y Node.js
imagen
# Virtualización Aplicaciones basadas en red
+ Virtualización es uno de los avances más significativos que ha contribuido a la habilitación de la computación en la nube.
+ Virtualización es el proceso en el que una computadora física, llamada host, ejecuta múltiples copias de un sistema operativo, donde cada copia es llamada guest  (invitado).
+ Cada invitado obtiene sus propios recursos virtuales y se comunica con la red por su cuenta.
+ El sistema host ejecuta un software llamado hypervisor que cambia los recursos entre los distintos invitados.
+ Con el software de compañías como VMWare y Openbox, puede tomar una CPU potente y usarla para ejecutar múltiples máquinas virtuales.
+ Esto optimiza el uso de los recursos físicos y reduce drásticamente los costos con respecto a la máquina anterior, un modelo de sistema operativo.
# Infraestructura basada en contenedores Aplicaciones basadas en red
+ Un contenedor generalmente representa solo una aplicación o un grupo de aplicaciones.
+ El valor de usar contenedores es que se incluyen todas las bibliotecas y binarios que necesita para ejecutar la aplicación, por lo que el usuario no tiene que realizar ese paso de instalación adicional.
+ El software para crear y administrar u orquestar contenedores está disponible en Docker, AWS (Elasticized Container Service), Microsoft (Azure Container Service) y otros.
+ Los programadores están creando software que realiza una única función de un sistema (como el procesamiento o almacenamiento de la base de datos) que se ejecuta en un contenedor.
+ Estos contenedores están organizados en "pods" que se ejecutan dentro de un "nodo" y pueden comunicarse entre sí y con el mundo exterior si es necesario.
+  Linux es la tecnología subyacente que hace que la tecnología de contenedores funcione.
+ Bare-Metal Deployment, es un sistema informático o una red en la que una máquina virtual se instala directamente en el hardware en lugar de dentro del sistema operativo (SO) del host.
# Frontend – Backend
imagen
# Mensajes de estado HTTP
imagen
## Pre-requisitos
# HTML (Hypertext Markup Language)
+ HTML no es un lenguaje de programación. Es un lenguaje de marcado que le dice a los navegadores web cómo estructurar las páginas web que visita.
+ HTML consta de una serie de elementos que se utilizan para encerrar, envolver o marcar diferentes partes del contenido para que aparezca o actúe de una determinada manera.
+ Las etiquetas adjuntas pueden convertir el contenido en un hipervínculo para conectarse a otra página, poner palabras en cursiva, etc.
imagen
## Pre-requisitos
# CSS (Cascading Stylesheets)
+ Se usa para darle estilos y diseño a la página web. Por ejemplo, puede usar CSS para modificar la fuente, el color, el tamaño y el espaciado de su contenido, dividirlo en varias columnas o agregar animaciones y otras características decorativas.
imagen
## Pre-requisitos
# JavaScript (JS)
+ JavaScript es un lenguaje dinámico de múltiples paradigmas con tipos y operadores, objetos estándar integrados y métodos. 

+ Su sintaxis se basa en los lenguajes Java y C; muchas estructuras de esos lenguajes también se aplican a JavaScript. 

+ JavaScript admite la programación orientada a objetos con prototipos de objetos, en lugar de clases

Referencias: https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript
## Pre-requisitos
# JavaScript (JS)
imagen

# Backend - Creación de API REST con Node.js
imagen

Referencia: https://nodejs.org/

¿Qué es Node.js?
+ Entorno de ejecución de código en JavaScript para el servidor.
+ Asíncrono.
+ Con E/S de datos en una arquitectura orientada a eventos.
+ Basado en el motor  V8 de Google Chrome.
# ¿Cómo utilizar Node.Js?
+ Uso de sockets.
+ Servidores locales o remotos.
+ Conexiones a bases de datos.
+ Creación de servicios REST Create-Read-Update-Delete

# ¿Quién usa Node.js?
+ Netflix
+ PayPal
+ LinkedIn
+ Uber
+ Ebay

# Express
+ Es una infraestructura de aplicaciones web Node.js mínima y flexible que proporciona un conjunto sólido de características para las aplicaciones web y móviles.
+ Con miles de métodos de programa de utilidad HTTP y middleware a su disposición, la creación de una API sólida es rápida y sencilla.
imagen
# Arquitectura de Node.Js
+ package.json: Generalmente en la raíz del proyecto, contiene metadatos sobre su aplicación o modulo, así como la lista de dependencias.
+ El comando npm install es usado para instalar dependencias y módulos.
# Arquitectura de Node.js
NPM (Node Package Manager): Gestor de paquetes por defecto de Node.js.
# Arquitectura de Node.js
Require: Es un función que incluye módulos que existen en archivos separados. Lee un archivo JavaScript, ejecuta el archivo y luego procede a devolver el objetivo exportado. Permite importar librerías propias de la arquitectura de Node, librerías externas y nuestros propios módulos. 
# Rutas del API en Node.js
En el código mostrado que se encuentra en la ruta PST>src>app.js se define el puerto, la ruta raíz del servidor web, que definen las rutas del API.
imagen
# Métodos GET, POST en Node.js
Definir en la ruta PST>src>controller>estudiante.controller.js los métodos GET, POST para el API.
imagen
# Promesas
+ Las promesas nos brindan una forma de darle sentido al comportamiento asincrónico. 
+ Al realizar una solicitud asincrónica, puede suceder una de dos cosas: todo sale como esperamos o hay un error.
+ Las promesas facilitan el manejo de solicitudes asincrónicas, lo cual es bueno, porque tenemos que lidiar con muchos datos asincrónicos en JavaScript.
+ Por ejemplo: Creemos una promesa asincrónica para cargar datos desde la API randomuser.me. Esta API tiene información como dirección de correo electrónico, nombre, número de teléfono, ubicación, etc.
# Rutas del API en Node.js
Programar las rutas del API, en PST>src>routes>estudiante.js
imagen
# Conexión a la base de datos de MySQL
Hacer la conexión a la base de MySQL con código JavaScript en la ruta PST>src>conf>databaseCon.js
imagen
# Pruebas desde cliente Web
Probar en el navegador web la URL http://localhost:3000/api/estudiante
imagen
# Backend - PHP
Para las páginas web dinámicas, el procedimiento es un poco más complicado, ya que puede incluir PHP y MySQL en la mezcla.
imagen
# USING PHP Y MYSQL
+ Con PHP, es simple incrustar una actividad dinámica en páginas web. Cuando le das a las páginas la extensión .php, tienen acceso instantáneo al lenguaje de script.
    <?php
  	echo " Today is " . date("l") . ". ";
?>
Here's the latest news.

+ El resultado final de las dos partes se ve así:
	Today is Wednesday. Here's the latest news.
+ MySQL, de uso gratuito e instalado en un gran número de servidores web de Internet, es un sistema de gestión de bases de datos robusto y excepcionalmente rápido.
+ La verdadera belleza de PHP, MySQL, JavaScript (a veces ayudado por jQuery u otros frameworks), CSS y HTML5 es la maravillosa forma en que todos trabajan juntos para producir contenido web dinámico: PHP maneja todo el trabajo principal en el servidor web, MySQL gestiona todos los datos, y la combinación de CSS y JavaScript se ocupa de la presentación de la página web.
# ¿Qué es WAMP, MAMP, O LAMP?
+ WAMP: “Windows, Apache, MySQL, y PHP”
+ MAMP: “Mac, Apache, MySQL, y PHP”
+ LAMP: “Linux, Apache, MySQL, y PHP”
Estas abreviaturas describen una configuración totalmente funcional utilizada para desarrollar páginas web dinámicas de Internet.
# Frontend -  Framework (marco de trabajo)
### **Ember:**
Es un framework más antiguo, tiene buena popularidad debido a su estabilidad, soporte de la comunidad y algunos principios de codificación inteligentes.
imagen
### **Angular:**
Es un framework de aplicaciones web y móviles de código abierto.
### **VUE:**
Extiende HTML con algo de su propio código. Aparte de eso, se basa principalmente en JavaScript estándar y moderno.
### **REACT:**
Es una biblioteca para renderizar componentes de UI. React se usa en combinación con otras bibliotecas para hacer aplicaciones web.
# Frontend -  REACT
+ La creación de una aplicación React se trata de componentes.
+ Un componente individual de React se puede considerar como un componente de IU en una aplicación.
+ Los componentes de React son objetos reutilizables.
+ En React, la interfaz de usuario se expresa con funciones puras.
+ Escribe código que parece HTML directamente en su JavaScript.
# Frontend -  REACT
Hay tres formas de declarar componentes de React:

(1) Como clases de ES6. Estas clases formalizan el patrón común de JavaScript.
class HelloWorld extends React.Component { render() { return(<p>Hello, world!</p>) }

(2) Importación y uso del método createReactClass ().
imagen

(3) Los componentes funcionales sin estado son funciones, no objetos que toman propiedades y devuelven un elemento DOM. El Modelo de objetos de documento (DOM) se refiere al árbol HTML del navegador que forma una página web.
const IngredientsList = props => React.createElement("ul", {className: "ingredients"}, 
props.items.map((ingredient, i) => React.createElement("li", { key: i }, ingredient) ) ) 
# Herramientas de Desarrollo Web
imagen
### **Código fuente de la página web:**

En una página web dar clic derecho, luego seleccionar la opción “Inspeccionar código fuente”.
### **Bootstrap:**


 Es un marco CSS gratuito y de código abierto para el desarrollo web y móvil. Contiene plantillas de diseño basadas en CSS y JavaScript para tipografía, formularios, botones, navegación y otros componentes de la interfaz.
 https://getbootstrap.com
### **Documentación de código fuente para informes.**

https://carbon.now.sh

# Recomendaciones de estudio
+ Lee el material proporcionado por la profesora.
+ Participa en clase en la resolución de los ejercicios.
+ Asiste a las ayudantías de docencia.  
+ Investiga, aprende, se parte de la clase.
# Introducción a los sistemas de gestión de bases de datos
+ Hay una variedad de sistemas de administración de bases de datos disponibles para Linux. Estos incluyen sistemas de gestión de bases de datos de alto nivel comercial, como Oracle, DB2 de IBM y Sybase.
+ Las bases de datos de código abierto de Linux también están disponibles, como MySQL y PostgreSQL. Estos están entre los más utilizados en los sistemas Linux. La mayor parte de los sistemas de administración de base de datos disponibles para Linux, están diseñados para soportar grandes bases de datos relacionales.
El propósito de una base de datos es ayudar a las personas a dar seguimiento a las cosas. Las aplicaciones clásicas de bases de datos se refieren al seguimiento de artículos tales como órdenes, clientes, empleos, empleados.
El “DataBase Management System” (DBMS) procesa la base de datos, y lo utilizan tanto los programadores como los usuarios, quienes pueden ingresar al DBMS directa o indirectamente.
imagen
Figura 3. Componentes de un sistema de bases de datos
# Introducción a los sistemas de gestión de bases de datos
El ciclo de desarrollo de sistemas de bases de datos contiene los siguientes pasos:

+ Requerimientos: Pueden ser de 3 tipos de requerimientos escritos, verbales, formularios.
+ Modelo lógico: Pueden existir varios métodos como jerárquico/árbol, red, relacional (modelo entidad relación), objeto, internet.
+ Modelo físico
+ Desarrollo
+ Implantación
+ Retroalimentación
# Modelo lógico
## Modelo entidad/relación
Los elementos claves del modelo entidad-relación son entidades, atributos y relaciones.     

Entidad: Es un objeto sobre el cual se requiere mantener o almacenar información. Ejemplos: facultad, alumno, materia, ciudad, item. Los tipos de entidades son: sujeto (empleado), objeto (articulo), evento (pedido), lugar (pais).

imagen

Figura 4. Entidades
Atributo: Las entidades tienen atributos o propiedades, como a veces se les llama, que describen las características de la entidad. Por ejemplo: 

imagen

Tipos de Atributos
	Clave primaria: #
	Obligatorio: *
	Opcional: O
	Foráneo: F
	Clave primaria foránea: F#

imagen

Relaciones
	1 : 1 
	1 : N
	N : M
imagen

imagen

Figura 8. UML (Lenguaje de Modelado Unificado) del Diagrama de Entidad/Relación del Sistema Académico

imagen

Figura 9. UML del Diagrama de Entidad/Relación de un Sistema Musical
https://www.lucidchart.com/

# Estructura y diseño de base de datos relacional
tablas

# SQL (Structured Query Language)
SQL es el lenguaje utilizado por la mayoría de los sistemas de gestión de base de datos relacional (RDBMSs), incluidos MySQL y PostgreSQL. Aunque muchos RDBMS usan herramientas administrativas para administrar bases de datos, en Linux MySQL y PostgreSQL.
imagen
Referencia: https://www.w3schools.com/sql/default.asp

## MySQL
+ MySQL es un sistema de gestión de bases de datos relacional desarrollado bajo licencia GPL/Licencia comercial por Oracle Corporation. 
+ MySQL está estructurado en un modelo cliente/servidor con un daemon de servidor (mysqld) que llena solicitudes de programas cliente. MySQL está diseñado para velocidad, confiabilidad y facilidad de uso. Se pretende que sea un sistema de gestión de bases de datos rápido para bases de datos grandes y, al mismo tiempo, fiable, adecuado para un uso intensivo.
+ Está considerada como la base datos open source más popular del mundo.
# Servicio de MySQL
## Instalación
+ Para la instalación de MySQL se realizan los siguientes pasos:
1. Instale MySQL y active el servicio.

root@ubuntu:/home/ubuntu# apt-get install mysql-server
root@ubuntu:/home/ubuntu# service mysqld start
## Servicio de MySQL
### Creación de usuarios en MySQL
+ Para crear un usuario en MySQL:
	mysql> CREATE USER 'acollaguazo'@'localhost' IDENTIFIED BY 'adi’;
	Query OK, 0 rows affected (0.07 sec)
+ Se otorga permisos al nuevo usuario:
mysql> GRANT ALL ON *.* TO 'acollaguazo'@'locahost' IDENTIFIED BY 'adi’;
	Query OK, 0 rows affected (0.00 sec)
Se refrescan todos los privilegios:
mysql> FLUSH PRIVILEGES;
Se accede con el usuario acollaguazo a MySQL:
[root@localhost admin]# mysql -u acollaguazo -p
Enter password: 
	Welcome to the MySQL monitor.  Commands end with ; or \g.
	Your MySQL connection id is 8
	Server version: 5.6.36 MySQL Community Server (GPL)
	Copyright (c) 2000, 2017, Oracle and/or its affiliates. All rights reserved.
	Oracle is a registered trademark of Oracle Corporation and/or its
	affiliates. Other names may be trademarks of their respective owners.
	Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.
+ Para eliminar un usuario existente de MySQL:
	mysql> DROP USER 'admin'@'localhost’;
	Query OK, 0 rows affected (0.00 sec)

