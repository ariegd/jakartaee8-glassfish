## Jakarta  EE 8 Aplicaciones de ejemplo
----------------------------------------

Ejemplos sencillos utilizando Servlet, Rest, JSF, Websocket, EL, EJB, CDI, Connectors y Security. Apectos fundamentales de las aplicaciones distribuidas o aplicaciones empresariales. Estos ejemplos obtenidos del repositorio de Eclipse GlassFish.

## Nota importante
------------------

Sólo se pude utilizar inyección de dependencias en servlets o en componentes EJB. La razón es que el servidor de aplicaciones debe inyectar el objeto referenciado en tiempo de ejecución y para ello debe poder controlar el ciclo de vida del componente en el que inyecta la dependencia. Esto sucede con los servlets o los componentes EJB que viven en los respectivos contenedores gestionados por el servidor de aplicaciones.

Un error muy común es colocar una anotación @Resource en una clase normal. El compilador no da ningún error, la clase se compila y la aplicación se despliega en el servidor de aplicaciones correctamente. Pero nadie inyecta la fuente de datos en la variable de instancia.


## JavaBeans
------------

Un JavaBean (o, para abreviar, un bean) es un componente software reutilizable escrito en Java. En realidad un bean no es más que una clase Java escrita siguiendo unas ciertas convenciones. Estas convenciones hacen posible que herramientas automáticas puedan acceder a sus propiedades y manipularlas sin necesidad de modificar el código. Esto puede servir en el caso de un IDE, por ejemplo, para realizar "programación visual". En JSP el uso principal de los beans es manipular componentes Java sin necesidad de incluir código en la página, accediendo a sus propiedades mediante etiquetas.

El uso de beans en páginas JSP ofrece diversas ventajas con respecto al uso directo de código Java:

    Se evita el uso de sintaxis Java, en su lugar se emplean etiquetas con sintaxis XML. Esto permite separar más fácilmente el trabajo de programadores y diseñadores web.
    Se simplifica la creación y uso de objetos compartidos entre varias páginas.
    Se simplifica la creación de objetos a partir de los parámetros de la petición
