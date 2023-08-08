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

# 2.2 Tecnologías web para dispositivos telemáticos
- [Frontend y Backend](#frontback)
- [Mensajes de estado HTTP](#mensajes)
- [HTML (Hypertext Markup Language)](#http)
- [CSS (Cascading Stylesheets)](#css)
- [JavaScript (JS)](#javascript)
- [Creación de API REST con Node.js](#api)
    - [¿Cómo utilizar Node.Js?](#node)
    - [¿Quién usa Node.js?](#uso_node)
    - [Express](#express)
    - [Arquitectura de Node.Js](#arquitectura)


<a name="frontback"> </a>

## 🌐 Frontend – Backend

<p align="center">
  <img src="../imagenes/unid2_1_frontend_backend.png" alt="modelos_red" width="100%">
</p>


<a name="mensajes"> </a>

## 🌐 Mensajes de estado HTTP

<p align="center">
  <img src="../imagenes/unid2_1_http.png" alt="modelos_red" width="100%">
</p>


<a name="http"> </a>

## 🌐 HTML (Hypertext Markup Language)

<p align="center">
  <img src="../imagenes/unid2_1_prerequisitos_html.png" alt="modelos_red" width="80%">
</p>

+ HTML no es un lenguaje de programación. Es un lenguaje de marcado que le d ice a los navegadores web cómo estructurar las páginas web que visita.
+ HTML consta de una serie de elementos que se utilizan para encerrar, envolver o marcar diferentes partes del contenido para que aparezca o actúe de una determinada manera.
+ Las etiquetas adjuntas pueden convertir el contenido en un hipervínculo para conectarse a otra página, poner palabras en cursiva, etc.


<a name="css"> </a>

## 🌐 CSS (Cascading Stylesheets)

<p align="center">
  <img src="../imagenes/unid2_1_prerequisitos_css.png" alt="modelos_red" width="100%">
</p>
+ Se usa para darle estilos y diseño a la página web. Por ejemplo, puede usar CSS para modificar la fuente, el color, el tamaño y el espaciado de su contenido, dividirlo en varias columnas o agregar animaciones y otras características decorativas.


<a name="javascript"> </a>

## 🌐 JavaScript (JS)

<p align="center">
  <img src="../imagenes/unid2_1_prerequisitos_JS2.png" alt="modelos_red" width="100%">
</p>


<p align="center">
  <img src="../imagenes/unid2_1_prerequisitos_JS.png" alt="modelos_red" width="80%">
</p>

+ JavaScript es un lenguaje dinámico de múltiples paradigmas con tipos y operadores, objetos estándar integrados y métodos. 

+ Su sintaxis se basa en los lenguajes Java y C; muchas estructuras de esos lenguajes también se aplican a JavaScript. 

+ JavaScript admite la programación orientada a objetos con prototipos de objetos, en lugar de clases

Referencias: https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript


<a name="api"> </a>

## 🌐 Creación de API REST con Node.js

<p align="center">
  <img src="../imagenes/unid2_1_node.png" alt="modelos_red" width="80%">
</p>

Referencia: https://nodejs.org/

¿Qué es Node.js?
+ Entorno de ejecución de código en JavaScript para el servidor.
+ Asíncrono.
+ Con E/S de datos en una arquitectura orientada a eventos.
+ Basado en el motor  V8 de Google Chrome.


<a name="node"> </a>

### 🕸️ ¿Cómo utilizar Node.Js?

+ Uso de sockets.
+ Servidores locales o remotos.
+ Conexiones a bases de datos.
+ Creación de servicios REST Create-Read-Update-Delete


<a name="uso_node"> </a>

### 🕸️ ¿Quién usa Node.js?
+ Netflix
+ PayPal
+ LinkedIn
+ Uber
+ Ebay


<a name="express"> </a>

### 🕸️ Express

<p align="center">
  <img src="../imagenes/unid2_1_express.jpg" alt="modelos_red" width="80%">
</p>

- Es una infraestructura de aplicaciones web Node.js mínima y flexible que proporciona un conjunto sólido de características para las aplicaciones web y móviles.
- Con miles de métodos de programa de utilidad HTTP y middleware a su disposición, la creación de una API sólida es rápida y sencilla.


<a name="arquitectura"> </a>

### 🕸️ Arquitectura de Node.Js

<p align="center">
  <img src="../imagenes/unid2_1_arquitectura_node.png" alt="modelos_red" width="100%">
</p>

- package.json: Generalmente en la raíz del proyecto, contiene metadatos sobre su aplicación o modulo, así como la lista de dependencias.
- El comando npm install es usado para instalar dependencias y módulos.

<p align="center">
  <img src="../imagenes/unid2_1_npm_node.png" alt="modelos_red" width="80%">
</p>

- NPM (Node Package Manager): Gestor de paquetes por defecto de Node.js.


<p align="center">
  <img src="../imagenes/unid2_1_require_node.png" alt="modelos_red" width="80%">
</p>

- Require: Es un función que incluye módulos que existen en archivos separados. Lee un archivo JavaScript, ejecuta el archivo y luego procede a devolver el objetivo exportado. Permite importar librerías propias de la arquitectura de Node, librerías externas y nuestros propios módulos. 


### Rutas del API en Node.js

<p align="center">
  <img src="../imagenes/unid2_1_rutasAPI_node.png" alt="modelos_red" width="100%">
</p>

En el código mostrado que se encuentra en la ruta PST>src>app.js se define el puerto, la ruta raíz del servidor web, que definen las rutas del API.
imagen

### Métodos GET, POST en Node.js

<p align="center">
  <img src="../imagenes/unid2_1_get_post_node.png" alt="modelos_red" width="100%">
</p>

Definir en la ruta PST>src>controller>estudiante.controller.js los métodos GET, POST para el API.

## Promesas

+ Las promesas nos brindan una forma de darle sentido al comportamiento asincrónico. 
+ Al realizar una solicitud asincrónica, puede suceder una de dos cosas: todo sale como esperamos o hay un error.
+ Las promesas facilitan el manejo de solicitudes asincrónicas, lo cual es bueno, porque tenemos que lidiar con muchos datos asincrónicos en JavaScript.
+ Por ejemplo: Creemos una promesa asincrónica para cargar datos desde la API randomuser.me. Esta API tiene información como dirección de correo electrónico, nombre, número de teléfono, ubicación, etc.
### Rutas del API en Node.js
<p align="center">
  <img src="../imagenes/unid2_1_rutasAPI_node.png" alt="modelos_red" width="100%">
</p>

Programar las rutas del API, en PST>src>routes>estudiante.js
imagen
### Conexión a la base de datos de MySQL
<p align="center">
  <img src="../imagenes/unid2_1_conexion_MySQL.png" alt="modelos_red" width="80%">
</p>

Hacer la conexión a la base de MySQL con código JavaScript en la ruta PST>src>conf>databaseCon.js
imagen
### Pruebas desde cliente Web

<p align="center">
  <img src="../imagenes/unid2_1_pruebas_clienteweb.png" alt="modelos_red" width="100%">
</p>

Probar en el navegador web la URL http://localhost:3000/api/estudiante
imagen
### Backend - PHP

<p align="center">
  <img src="../imagenes/unid2_1_backend_PHP.png" alt="modelos_red" width="100%">
</p>


Para las páginas web dinámicas, el procedimiento es un poco más complicado, ya que puede incluir PHP y MySQL en la mezcla.
imagen
### USING PHP Y MYSQL
+ Con PHP, es simple incrustar una actividad dinámica en páginas web. Cuando le das a las páginas la extensión .php, tienen acceso instantáneo al lenguaje de script.
    <?php
  	echo " Today is " . date("l") . ". ";
?>
Here's the latest news.

+ El resultado final de las dos partes se ve así:
	Today is Wednesday. Here's the latest news.
+ MySQL, de uso gratuito e instalado en un gran número de servidores web de Internet, es un sistema de gestión de bases de datos robusto y excepcionalmente rápido.
+ La verdadera belleza de PHP, MySQL, JavaScript (a veces ayudado por jQuery u otros frameworks), CSS y HTML5 es la maravillosa forma en que todos trabajan juntos para producir contenido web dinámico: PHP maneja todo el trabajo principal en el servidor web, MySQL gestiona todos los datos, y la combinación de CSS y JavaScript se ocupa de la presentación de la página web.
### ¿Qué es WAMP, MAMP, O LAMP?
+ WAMP: “Windows, Apache, MySQL, y PHP”
+ MAMP: “Mac, Apache, MySQL, y PHP”
+ LAMP: “Linux, Apache, MySQL, y PHP”
Estas abreviaturas describen una configuración totalmente funcional utilizada para desarrollar páginas web dinámicas de Internet.
## Frontend -  Framework (marco de trabajo)


### **Ember:**
<p align="center">
  <img src="../imagenes/unid2_1_ember.png" style="width: 20%; height: 80px; float: right; padding: 15px;" alt="configip">
</p>

Es un framework más antiguo, tiene buena popularidad debido a su estabilidad, soporte de la comunidad y algunos principios de codificación inteligentes.
imagen
### **Angular:**

<p align="center">
  <img src="../imagenes/unid_2_1_angular.png" style="width: 20%; height: 80px; float: right; padding: 15px;" alt="configip">
</p>

Es un framework de aplicaciones web y móviles de código abierto.

### **VUE:**
<p align="center">
  <img src="../imagenes/unid2_1_VUE.png" style="width: 20%; height: 80px; float: right; padding: 15px;" alt="configip">
</p>

Extiende HTML con algo de su propio código. Aparte de eso, se basa principalmente en JavaScript estándar y moderno.

### **REACT:**

<p align="center">
  <img src="../imagenes/unid2_1_REACT.png" style="width: 20%; height: 80px; float: right; padding: 15px;" alt="configip">
</p>
Es una biblioteca para renderizar componentes de UI. React se usa en combinación con otras bibliotecas para hacer aplicaciones web.


### Frontend -  REACT
+ La creación de una aplicación React se trata de componentes.
+ Un componente individual de React se puede considerar como un componente de IU en una aplicación.
+ Los componentes de React son objetos reutilizables.
+ En React, la interfaz de usuario se expresa con funciones puras.
+ Escribe código que parece HTML directamente en su JavaScript.


### Frontend -  REACT


Hay tres formas de declarar componentes de React:

(1) Como clases de ES6. Estas clases formalizan el patrón común de JavaScript.¨

```
class HelloWorld extends React.Component { render() { return(<p>Hello, world!</p>) }
```

(2) Importación y uso del método createReactClass ().


<p align="center">
  <img src="../imagenes/unid2_1_frontend_react.png" alt="modelos_red" width="100%">
</p>

(3) Los componentes funcionales sin estado son funciones, no objetos que toman propiedades y devuelven un elemento DOM. El Modelo de objetos de documento (DOM) se refiere al árbol HTML del navegador que forma una página web.

```
const IngredientsList = props => React.createElement("ul", {className: "ingredients"}, 
props.items.map((ingredient, i) => React.createElement("li", { key: i }, ingredient) ) ) 
```

## Herramientas de Desarrollo Web

<p align="center">
  <img src="../imagenes/unid2_1_herramientas_desWeb.png" alt="modelos_red" width="100%">
</p>



### **Código fuente de la página web:**

<p align="center">
  <img src="../imagenes/unid2_1_herramientas_desWeb2.png.jpg"
  style="width: 40%; height: 300px; float: right; padding: 15px;" alt="configip">
</p>

En una página web dar clic derecho, luego seleccionar la opción “Inspeccionar código fuente”.

### **Bootstrap:**


 Es un marco CSS gratuito y de código abierto para el desarrollo web y móvil. Contiene plantillas de diseño basadas en CSS y JavaScript para tipografía, formularios, botones, navegación y otros componentes de la interfaz.
 https://getbootstrap.com

### **Documentación de código fuente para informes.**

https://carbon.now.sh
