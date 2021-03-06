# 馃攺 3. Consideraciones para seguridad en el desarrollo

## 3.1. Uso de librer铆as y frameworks de seguridad

Para un desarrollo seguro es necesario seleccionar librer铆as y frameworks confiables, teniendo en cuenta que tiene un desarrollo y mantenimiento activo, para que sean ampliamente utilizadas por los programadores, es importante tener un control sobre las librer铆as y frameworks con la intenci贸n de tener las versiones m谩s actualizadas o en su defecto las m谩s estables.

La mayor铆a de frameworks nos indican ciertos puntos sobre c贸mo solucionar alg煤n problema en espec铆fico que ya hab铆a ocurrido anteriormente en el desarrollo de software. Por lo regular se recurre a optar por el uso de frameworks que se enfocan en atender distintas 谩reas como la seguridad como el control de acceso, el cifrado y la validaci贸n de entradas, etc.

## 3.2. Consultas seguras a las bases de datos

Las vulnerabilidades pueden llegar hacer por una inyecci贸n SQL qu茅 ocurre cuando datos no confiables son insertados en una consulta SQL. Este tipo de ataques permite al enemigo extraer, modificar o eliminar informaci贸n desde la base de datos, e incluso llegar a tomar el control del sistema.

Para prevenir este tipo de ataques se deben tomar ciertas medidas de protecci贸n a la informaci贸n que ayuden a:

### 3.2.**1.** **Limitar el acceso a la base de datos:**

Cuando muchas personas tienen intervenci贸n, el resultado no puede ser positivo, esto ocurre con los accesos a las bases de datos, por eso cuanto m谩s acotados los permisos y privilegios, se tiene un mejor control.

### 3.2.**2.** **Identifica los datos sensibles:**

Antes de pensar en utilizar alguna t茅cnica o herramienta de protecci贸n, es necesario saber cu谩l es la informaci贸n importante que se debe proteger. As铆 que es importante entender la l贸gica para poder definir una buena base de datos, y llegar a poder determinar d贸nde y c贸mo podemos almacenar los datos sensibles. La 煤nica forma de tener una buena administraci贸n es tener conocimiento de la base de datos que se desarrolla.

### 3.2.**3.** **Monitorear la actividad de la base de datos:**

Estar atento es importante para poder registrar las acciones y movimientos que se realizan sobre los datos para saber qui茅n ha manipulado la informaci贸n. Tener un historial de las operaciones va a ayudar a comprender todo lo que se realiza, modifica en la base de datos y as铆 se podr谩 evitar robo de informaci贸n, cambios malintencionados y detectar acciones sospechosas.

### 3.2.**4.** **Cifrar la informaci贸n:**

Una vez que se identifican los datos sensibles y/o la informaci贸n confidencial, una buena pr谩ctica es utilizar m茅todos que puedan cifrar estos datos.

Cuando un atacante encuentra alguna vulnerabilidad y logra tener acceso al sistema, se sabe que a lo primero a lo que 茅l accede es a la base de datos, ya que se tiene mucha informaci贸n importante, la mejor manera de cuidar estos datos es volverla ilegible para cualquier persona.

### 3.2.**5.** **Soluciones de seguridad:**

Un buen an谩lisis puede ayudar a detectar las vulnerabilidades que se tienen en el sistema, encontrando as铆 los riesgos y poder establecer un plan de prevenci贸n y un plan de recuperaci贸n de la informaci贸n ante desastres que el atacante pueda llegar hacer, por lo que el administrador de la base de datos debe mantener y asegurar la informaci贸n.

## 3.3. Codificar y escapar los datos

Estas llegan hacer t茅cnicas que evitan ataques de terceros, pues esta consiste en transformar algunos caracteres especiales en otros caracteres equivalentes que puedan ser entendidos f谩cilmente para el int茅rprete.

Escapar caracteres tambi茅n llega hacer muy parecido a codificar los datos, con la diferencia de que en lugar de reemplazar un car谩cter por otro, se a帽ade un car谩cter antes del dato a escapar, para evitar una mal interpretaci贸n.

Se debe tomar en cuenta que se debe considerar como inseguros los datos que se ingresen fuera de la aplicaci贸n, as铆 como tambi茅n los datos que provienen desde la base de datos todo esto por si alg煤n atacante hizo alguna modificaci贸n de los datos, por eso deben ser correctamente codificados y escapados los datos.

## 3.4. Validaci贸n de datos

La validaci贸n de datos ayuda a garantizar que todos los datos que se ingresen en la aplicaci贸n sean correctos, es decir que sean, precisos, seguros y consistentes. Esto se logra a trav茅s de funciones que realizan las debidas validaciones para las entradas de datos.

Es una buena pr谩ctica asegurar que solo los datos que se ingresaron correctamente podr谩n se registren en la aplicaci贸n. Por ejemplo, si se espera que en un campo se puedan ingresar solo d铆gitos num茅ricos, no se deben aceptar cualquier otro tipo de caracteres.

Algunos de los tipos de validaci贸n de datos incluyen:

* Validaci贸n de c贸digo
* Validaci贸n de tipo de datos
* Validaci贸n del rango de datos
* Validaci贸n de restricciones

## 3.5. Implementar mecanismos de autenticaci贸n seguros

Para poder proteger la identidad de los usuarios cuando se realice alguna acci贸n, se debe identificarse, autenticarse y estar autorizado, haciendo uso de alg煤n m茅todo donde pueda registrarse. Se debe saber que:

* **La autenticaci贸n:**

Se define como aquel proceso mediante el cual un usuario obtiene acceso a los recursos de un sistema a trav茅s de una identificaci贸n.

* **La autorizaci贸n**

Consiste en designar los recursos que estar谩n permitidos al usuario acceder de un sistema, si bien, ya se encuentra autenticado, no significa que tendr谩 el acceso completo del sistema.

La autenticaci贸n hace referencia a la acci贸n de verificar que una persona es quien dice ser. Se pueden utilizar varios mecanismos como lo son:

* **Contrase帽as:**

Las aplicaciones deben exigir al usuario el uso de una buena contrase帽a, tambi茅n se deben implementar mecanismos para la recuperaci贸n de contrase帽as, ya sea utilizando alg煤n medio como un correo electr贸nico o mensajes.

Tambi茅n se debe implementar alg煤n m茅todo donde solo el usuario tenga un l铆mite de intentos de inicio de sesi贸n, ya sea bloqueando las cuentas despu茅s de un cierto n煤mero de intentos fallidos, y no se debe llegar a bloquear permanentemente las cuentas, ya que podr铆a traer problemas con los usuarios reales de las cuentas donde se quiso ingresar sin su consentimiento.

* **Multifactor**

Esta es otra manera donde se requiere varios m茅todos de autenticaci贸n para comprobar la identidad de un usuario. Com煤nmente se usa una combinaci贸n de dos o m谩s factores como lo son: las contrase帽as, tokens de seguridad, o mediante el uso de verificaci贸n biom茅trica que permite crear una mejor seguridad que dificulta que un atacante acceda f谩cilmente al sistema, o una base de datos etc. Si en un factor se logra ingresar, al menos el atacante tendr铆a una o m谩s barreras que romper antes de entrar con 茅xito en el objetivo.

* **Autenticaci贸n criptogr谩fica**

La autenticaci贸n con cifrado es la manera donde se puede tener una comunicaci贸n segura. Ya que ayuda a garantizar que el origen de donde salen los datos y el destino a donde llegan sean seguras. Esto consiste en codificar la comunicaci贸n en el origen y decodificarla cuanto esta llega a su destino. El cifrado impide que los atacantes puedan interceptar cualquier informaci贸n que sea transmitida.

## 3.6. Implementar mecanismos de manejo de sesi贸n

El manejo de la sesi贸n es uno de los aspectos cr铆ticos de la seguridad. Los objetivos principales son:

* Los usuarios autenticados tengan un mejor control con sus sesiones.
* Se cumplan los medios de autorizaci贸n cuando se requiera ingresar el usuario.
* Se prevengan los ataques, como lo es ingresar a sesiones activas que no fueron cerradas correctamente.

**Algunas vulnerabilidades que pueden ocurrir si no se implementan de forma correcta los mecanismos pueden ser:**

* Fijaci贸n de sesi贸n donde el atacante obtiene el identificador de sesi贸n de otra persona y puede ingresar.
* Manejo de la informaci贸n de sesi贸n err贸nea, por no implementar un buen control en las sesiones, el atacante puede obtener datos de la sesi贸n de otro usuario.

Para el manejo de las sesiones, se debe considerar al menos lo siguiente:

* Al iniciar sesi贸n el identificador de sesi贸n debe ser 煤nico.
* Se deben generar otro identificador de sesi贸n cuando este inicie sesi贸n.
* Se tiene que terminar la sesi贸n del usuario por inactividad.

## 3.7. Datos en reposo

Debemos siempre tratar de proteger la informaci贸n del usuario, ya que a veces se requieren medios de protecci贸n dependiendo el estado en el que se encuentre la informaci贸n, con esto se refiere a la informaci贸n que no est谩 siendo accedida, usada y que se encuentra guardada.

Es por eso que se debe evitar, cuando sea posible, el almacenamiento de datos sensibles por parte de la aplicaci贸n. En caso de que no se pueda evitar almacenar datos sensibles, estos deben ser protegidos mediante encriptaci贸n, para prevenir la modificaci贸n o acceso no autorizado.

## 3.8. Desarrollo orientado a pruebas

El equipo de desarrollo deber谩 tener un set de datos no v谩lidos, escogido para trabajar y cargar el sitio para efectos de pruebas de integraci贸n continua o unitarias. Este set no debe contener informaci贸n real y la cantidad de datos debe ser reducida, pero suficiente para generar pruebas.

## 3.9. Calidad de c贸digo

Algo muy importante dentro del desarrollo de software es la calidad del c贸digo; los est谩ndares se encuentran constantemente presentes en la vida cotidiana, son importantes para mantener un orden en las cosas y en el desarrollo no es la excepci贸n.

Los est谩ndares de c贸digo son una serie de reglas definidas para un lenguaje de programaci贸n, o bien, un estilo de programaci贸n espec铆fico. El estilo garantiza que todos los que contribuyen en un proyecto tengan una forma 煤nica de dise帽ar su c贸digo, lo que da como resultado una base de c贸digo coherente, asegurando una f谩cil lectura y mantenimiento.

Algunas consideraciones a tomar en cuenta son:

* Tomar como base est谩ndares oficialmente publicados de las herramientas que se utilizan en cada proyecto.
* Para obtener un c贸digo de f谩cil lectura es necesario poner atenci贸n al estilo del mismo como segmentos de c贸digo, correcto uso de indentaci贸n, longitud de l铆neas y espacios entre ellas.
* Asignaci贸n correcta de nombres en variables, funciones, etc.
* Establecer l铆mites en complejidad o longitud de funciones.

## 3.10. Manejo seguro de errores y excepciones

Se debe desarrollar el sistema, de forma tal, que aplique el principio de 鈥渇allar seguro鈥?, es decir:

* No exponer informaci贸n sensible o privada en los mensajes de error. En particular, nunca olvidar desactivar el modo debug al pasar a producci贸n.
* Asegurarse de que una excepci贸n o fallo no comprometa la seguridad por un error de programaci贸n en el sistema. Por ejemplo, causar una denegaci贸n de servicio o ejecuci贸n de c贸digo con privilegios incorrectos.
* Registrar las excepciones adecuadamente en los sistemas que correspondan.
