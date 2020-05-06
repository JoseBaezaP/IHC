# Segunda Entrega

### Requerimientos Especificos

El propósito del proyecto es desarrollar una pieza tecnológica para los maestros para monitorear las actividades que realizan los alumnos con dificultades auditivas, en las areas de matematicas y español con el fin de localizar las áreas en las que un alumno pueda tener más dificultad y poder brindar un reforzamiento, que les permita mejorar su educación.

#### Requisitos Funcionales

Identificación de usuarios.

|NR|Descripcion|
|---|---|
|1 |El sistema deberá contar con un login para los usuarios.|
|2|Debe ingresar usuario y contraseña. El sistema deberá recuperar el usuario y contraseña de los alumnos en la base de datos de los usuarios registrados.|
|3|El sistema deberá permitir el uso de acceso a través de la cuenta google y facebook.|

Registro de usuarios.
|#R|Descripcion|
|---|---|
|1|El sistema deberá tener las opciones para la creación de cuentas para maestros o alumnos.| 
|2|El sistema deberá contar con un formulacion para la creación de nuevos usuarios de maestros y alumnos.|
|3|Los datos que debe tener el formulario son Nombres, Apellido Materno, Apellido Paterno, Correo, Contraseña.|

Creación  de grupos

|#R|Descripcion|
|---|---|
|1|Los maestros podrán crear grupos dentro del sistema y se le asignará un nombre del grupo.|
|2|los maestros podrán agregar alumnos al grupo por medio de un codigo de invitacion.|
|3|los alumnos podrán ingresar a un grupo por un código de invitación proporcionado por el maestro.|

Visualización de grupos.
|#R|Descripcion|
|---|---|
|1|Los maestros podrán visualizar a todos los alumnos que pertenecen al grupo.|
|2|Los maestros podrán visualizar la puntuación de sus alumnos en cada actividad realizada.|
|3|Los maestros podrán visualizar gráficas de todas las actividades realizada por sus alumnos.|

Selección de actividades.
|#R|Descripcion|
|---|---|
|1|Las actividades estarán clasificadas por temas, Español, Matemáticas.|
|2|Las actividades de los temas deberá empezar con una pequeña introducción.|
|3|Las instrucciones deberán estar en español y en lengua de señas. |
|4|Las actividades estarán compuestas, por una instrucción, el problema y sus opciones múltiples.|
|5|Las instrucciones y el problema deberá tener la opción de mostrar en lengua de señas.|
|6|Los alumnos podrán seleccionar los problemas de cada tema a realizar.|
|7|Los alumnos podrán seleccionar un explicación del problema en lengua de señas.|
|8|El sistema validará que los alumnos ingresen la respuesta correcta y notificarle.|

#### Requisitos No Funcionales de Usabilidad
|#NR|Descripcion|
|---|---|
|1|Los usuarios deberán poder crear una cuenta del sistema en menos de 5 minutos.|
|2|Los usuarios debera poder ingresar al sistema en menos de 3 minutos.|
|3|Los alumnos deben poder acceder a una actividad de en menos de 5 toques.|
|4|Los ejercicios deber ser fácil de seleccionar una respuesta.|
|5|Los maestros deben aprender a acceder a sus funcionalidades de creación de grupos en menos de 5 toques.|
|6|Los ejercicios deben permitir al usuario cambiar con facilidad las instrucciones de LSM a español.|
|7|El sistema debe de tener una interfaz sencilla y principalmente entendible para los usuarios.|
|8|Los ejercicios contarán con un video en LSM para que los alumnos puedan comprender mejor lo que se debe hacer.|
|9|El tiempo de aprendizaje del sistema por un usuario debe ser menor a 30 min.|
|10|El sistema debe poseer interfaces gráficas bien informadas.|
|11|El color de las interfaces debe hacer uso de una buena combinación de colores.|

## Casos de Uso
Caso de uso 1: Crear cuenta   

Actor primario: Alumno o Maestro

Meta en el contexto: El usuario cree un tipo de cuenta en el sistema.

Condiciones previas: El usuario debió haber abierto la aplicación en su dispositivo móvil.

Activador: El cliente debio haber seleccionado crear nueva cuenta. 
Escenario: 

* Usuario: Selecciona el tipo de cuenta que va a crear Alumno o Maestro.
* Usuario: Ingresa sus datos en el formulario.
* Usuario: Selecciona el botón crear cuenta.

Escenario secundario:
* Usuario: Crea una cuenta a través de su cuenta de facebook.
* Usuario: Crea una cuenta a través de su cuenta de google.

Excepciones:
* El usuario ya existe.
* El correo ya existe.
* Cancelar.

Frecuencia de uso: Cada vez que se necesite crear una nueva cuenta.

Canal hacia el actor: A través de la aplicación.

-----

Caso de uso 2: Ingresar al sistema   

Actor primario: Alumno o Maestro

Meta en el contexto: El usuario ingresa a su perfil del sistema.

Condiciones previas: El usuario debió haber creado su cuenta previamente.

Activador: El cliente debio haber seleccionado ingresar al sistema. 

Escenario: 
* Usuario: Ingresa su usuario y contraseña al formulario.
* Usuario: Selecciona el botón ingresar.
* Escenario secundario:
* Usuario: Ingresa a través de su cuenta de facebook.
* Usuario: Ingresa a través de su cuenta de google.

Excepciones:
* Usuario o contraseña incorrecta.
* Servidor fuera de servicio.

Frecuencia de uso: Cada vez que se necesite ingresar al sistema

Canal hacia el actor: A través de la aplicación.

----

Caso de uso 3: Crear grupo

Actor primario: Maestro

Meta en el contexto: El maestro creará un grupo.

Condiciones previas: El maestro debió haber ingresado su cuenta previamente.

Activador: El maestro debió haber ingresado sus datos correctos en el login. 

Escenario: 
* Maestro: Selecciona la opción de nuevo grupo.
* Maestro: Ingresa los datos del grupo.
* Maestro: Genera un código del grupo.

Excepciones:
* Maestro: El maestro ya tiene un grupo con el mismo nombre.

Frecuencia de uso: Cada vez que se necesite crear un grupo.

Canal hacia el actor: A través de la aplicación.

----

Caso de uso 4: Ingresar a un grupo.    

Actor primario: Alumno

Meta en el contexto: El alumno ingresará a un grupo.

Condiciones previas: El alumno debió haber ingresado su cuenta previamente.

Activador: El alumno debió haber ingresado sus datos correctos en el login. 

Escenario: 
* Alumno: Selecciona el código que le envió el maestro.
* Sistema: Abre la aplicación y verifica el código del grupo. 
* Alumno: Acepta el ingreso al grupo.

Excepciones:
* Sistema: El codigo de invitacion ya no es válido .

Frecuencia de uso: Cada vez que un alumno ingrese a un grupo.

Canal hacia el actor: A través de la aplicación.

------

Caso de uso 5: Visualizar alumnos    

Actor primario: Maestro

Meta en el contexto: El maestro visualizará los datos del alumno.

Condiciones previas: El maestro debió haber ingresado su cuenta previamente.

Activador: El maestro debió haber ingresado sus datos correctos en el login. 

Escenario: 
* Maestro: Selecciona un grupo existente..
* Maestro: Selecciona todos los alumnos.
* Maestro: Selecciona a un alumno y accede a todos los aciertos de ese alumno en cada area.
* Escenario secundario:
* Maestro: Selecciona las gráficas de aciertos  de su grupo. 

Frecuencia de uso: Cada vez que se accedan a los aciertos de cada grupo o alumno.

Canal hacia el actor: A través de la aplicación.

---

Caso de uso 6: Realizar una actividad.    

Actor primario: Alumno

Meta en el contexto: El alumno realizará una actividad.

Condiciones previas: El alumno debió haber ingresado su cuenta previamente.

Activador: El alumno debió haber ingresado sus datos correctos en el login. 
Escenario: 
* Alumno: Selecciona una de las áreas Español o Matemáticas
* Sistema: Selecciona un ejercicio.
* Alumno: Selecciona una de las respuestas.
* Sistema: Si la respuesta es correcta, envía un notificación al alumno.
* Sistema: Actualiza los aciertos del alumno.
* Escenario Secundario:
* Sistema: Si la respuesta es incorrecta le muestra la respuesta correcta.
* Alumno: Selecciona para la explicación en LSM.

Excepciones:
* Sistema: Falla de la conexión .

Frecuencia de uso: Cada vez que un alumno ingrese a un grupo.

Canal hacia el actor: A través de la aplicación.

Se puede encontrar toda esta informacion son más detalle en la especificación de Requerimientos de software [ERS](https://github.com/JoseBaezaP/IHC/blob/master/Deliveries/Especificacion%20de%20Requisitos%20de%20Software%20v1.1.pdf)


### Trazabilidad de los requisitos

* Identificacion de Usuario
  
![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz5.png)

* Registro de Usuarios

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz6.png)

* Creaccion de grupos

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz1.png)

* Visualización de grupos

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz2.png)

* Selección de actividades

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz3.png)
![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Matriz/Matriz4.png)

Se puede encontrar toda esta informacion en el documento de [matriz de trazabilidad de requisitos](https://github.com/JoseBaezaP/IHC/blob/master/Deliveries/Matriz%20de%20trazabilidad%20de%20requisitos%20V2.pdf)


# Prototipado de Intefaces

### Desarollo de Prototipos

Para el desarrollo de prototipos se realizó usando la herramienta InVision, que te permite realizar prototipos de alta fidelidad.

Con la información que habiamos obtenido de las encuestas a los maestros de CAM12 y a la maestra Nallelly Sanchez Razo de la organización de Audio Amigo de México que nos estuvo apoyando con informacion, acerca de como trabajan en el estado de México. Se logro hacer la primera versión del prototipo en InVision, el cual se puede encontrar en el siguiente enlace. [Prototipo](https://practicalsession.invisionapp.com/prototype/ck9rnxpny00c70q01efivt67a/play)

### Guias de Diseño

Para empezar a darle un buen diseño a las interfaces para el prototipo empezamos a investigar y buscar guías de diseño que nos permitan acomodar la información que debíamos plasmar en el prototipo, no nos basamos de uno solo, sino que recopilamos varias guías de diseño para crear en nuestro.
Además investigamos acerca de la ergonomía del celular, para saber los beneficios que tiene, por ejemplo si la aplicación es vertical, entonces el uso de una o dos manos, puede ser más fácil, sin embargo las interacciones en la parte superior de la pantalla necesitan mayor esfuerzo. Por lo tanto era necesario que las plantillas cumplieran con la organización para el uso del celular en modo vertical.  

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Prototype/Prototype1.png)


Al final, notamos que la mayoría de las plantillas siguen este principio y la forma de acomodar era similar a las anteriores, al investigar más el porqué, es para el usuario además de acceder a las funcionalidades, una organización sigue el principio de proximidad lo que le da a usuario comprender las funcionalidades principales de la pantalla.
Mientras más difícil se encuentre la funcionalidad es secundaria.

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Prototype/Prototype3.png)

### Diseño de Interacción

La IxDA (Interaction Design Association), lo define como: 

“El diseño de interacción (IxD) define la estructura y el comportamiento de sistemas interactivos. Los diseñadores de interacción buscan crear relaciones significativas entre las personas y los productos o servicios que estos usan, desde computadoras hasta dispositivos móviles, aparatos y más…”

#### Cuatro dimensiones para el diseño de interacción

*1ra Dimensión - Palabras:*

En toda la interfaz de usuario se trató de  dar la información con la menor palabras de manera que sea concisa y no abrume a los niños por demasiada informacion, ademas de incluir videos durante cada ejercicio donde se muestra la instrucción en LSM, para que no tengan dudas al momento de empezar con las actividades. Usando imágenes para identificar materias opciones, y usando la organización antes mencionado.

*2da Dimensión - Representaciones visuales:*

Optamos por incluir más imágenes que representen la acciones que realiza ya sea un botón, además eso permite que los usuarios puedan cometer menos errores al momento de usar la aplicación, ya que se asocia a cosas que ellos ya conocen.

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Prototype/Prototype5.png)

*3ra Dimensión - Espacio:*

Al ser una aplicación para dispositivos móvil, las principales acciones por parte del usuario es la pantalla táctil, por lo que fue necesario utilizar la ergonomía del celular, para que el usuario pueda usar la aplicación si problemas.
Se decidió realizar el desarrollo del prototipo de manera horizontal, ya que de esta manera se puede usar las dos manos y abarcar toda la pantalla, o usar solo una mano y no tendrias complicaciones. 

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Prototype/Prototype4.png)

*4ta Dimensión - Tiempo*

Motivando a los alumnos cuando acaban un ejercicio para mejorar su puntuación o realizando otro actividad. 

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Prototype/Prototype.png)

# Metodos de Inspección

Metodo de Inspección 

# Planeacion de la Prueba

![](https://github.com/JoseBaezaP/IHC/blob/master/Image/PlaneacionPrueba.png)

# Trabajo en equipo

Bitácora/Evidencia del proceso

Metrica de contribución 

Presentacion del Avance 
