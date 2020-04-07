### Miembros del equipo:

+ **Jose Baeza Pérez**  <br>
+ **Ariel May** <br>
+ **Nicolas Gala** <br>
+ **Leo Hernandez** <br>


# Objetivo   
Desarrollar una pieza tecnológica para facilitarle al maestro actividades de matemáticas que se realizan
en clase, y poder monitorear los datos obtenidos de la actividad por el alumno.
### Datos relevantes
Actualmente estamos trabajando con el centro de usos multiples CAM número 12 con alumnado entre 12 y 18 años de edad, ya que en esta institución se dan asesorías para poder reforzar temas vistos en sus escuelas regulares, pero apesar
de que hay niños de gran edad, ellos siguen teniendo difcultades para poder.
Al estar recopilando datos, platicando con maestros y alumnos, hemos podido indentificar los siguientes aspectos.   
##### Maestros
+ Los maestros tratan motivar a sus alumnos para aprender temas nuevos, por medio de juegos, actividades, imagenes, etc.
+ La mayoria de los maestros, usan sus computadoras para dar clase y asi poder hacerla más dinamica.
##### Alumnos
+ Presentan problemas para poder poder abstraer la información del mundo real al mundo empirico.
+ Tratan de mejorar como persona para poder superarse y tratar de entender temas que les cueste mucho trabajo comprender.
+ Muchos de ellos son hijos de padres y/o con descendencia de familiares sordos, esto lleva a que solo sepan LSM y tengan difcultades al leer y al escribir.   
   
Existen ciertas aplicaciones con relación a la ejercicios practicos para poder practicar temas con respecto a metematicas 
y español, como podría ser Tangram, Agnitus. mindomo, DotToDot numbers & letters, etc. pero ninguno de estos tiene esa pequeña parte de inclusion. A partir de esta pequeña investigación para poder ver aplicaciones 
similares que toquen el tema de inclusión para gente sorda, pudimos ver un aplicacion llamada "Dilo con Señas" la cual fue desarrollada con el fin de comprender ciertas como decir ciertas cosas en lenguaje de señas, 
pero hay nada con el fin de poder ayudar a esta población para mejorar academicamente. 
### Principal propuesta 
**Desarrollar un sistema tomando como ejemplo el plan educativo manejado en el centro de usos multiples CAM 12, con el fin de mejorar la metodologia de aprendizaje utilizadó para los niños con limitante auditiva.**
___
## Planeación

La forma que nosotros usamos para poder fue en base a encuestas, ya que esto nos ayudo a poder identificar datos especificos de los alumnos y maestros. Los cuales fueron muy importantes debido
a que notamos particularidades en tanto a niños como maestros (las todas las entrevistas se encuentran en el siguiente [enlace](https://github.com/JoseBaezaP/IHC/tree/master/Surveys)), gracias a esto pudimos notar lo siguiente:   
![](https://github.com/JoseBaezaP/IHC/blob/master/Surveys/graphics/imagenes/Alumnos%201.PNG)
![](https://github.com/JoseBaezaP/IHC/blob/master/Surveys/graphics/imagenes/Alumnos%202.PNG)
![](https://github.com/JoseBaezaP/IHC/blob/master/Surveys/graphics/imagenes/Alumnos%203.PNG)
![Aparatos que usan mas](https://github.com/JoseBaezaP/IHC/blob/master/Surveys/graphics/imagenes/Alumnos%204.PNG)
![](https://github.com/JoseBaezaP/IHC/blob/master/Surveys/graphics/imagenes/Alumnos%205.PNG)

Con esto podemos ver que muchos de estos niños tinen detalles practicamente en las mismas materias y prefieren aprender de manera practica las cosas,
ya que prefieren materiales didacticos para poder entender mejor los temas. Es por ello que el sistema que deseamos realizar sea usado en el CAM, para
que las maestras ya que tiene ventaja debido a que la mayoria de ellas usan sus computadoras, tabletas o telefonos para dar clase, es por ellos que se piensa
crear este sistema para poder ayudar a las maestras y que los niños le tomen mucho más interes en aprender.
Es posible que dicho sistema pueda ser usado por los niños para que ellos puedan repasar ciertos temas que deseen reforzar antes de ir a sus clases regulares o para poder tener practicar e ir con mas ideas o dudas especificas antes de ir al CAM.   
*Si desea ver todas las graficas puede entrar al siguiente [enlace](https://github.com/JoseBaezaP/IHC/tree/master/Surveys/graphics)*   
Para poder realizar las nuevas actividades tenemos asignados los siguientes días:
![](https://github.com/JoseBaezaP/IHC/blob/master/Image/calendar/Calendario%201.jpeg)
![](https://github.com/JoseBaezaP/IHC/blob/master/Image/Calendar/Calendario%202.jpeg)


## Personas

Ya despues de todo la investigación realizado pudimos indentificar a dos personas involucradas para el desarrollo de este proyecto
las personas con las que trabajaremos serían **maestros** y **alumnos**. Estas personas quedarían de la siguiente manera:
![Persona alumno](https://github.com/JoseBaezaP/IHC/blob/master/Image/personas/Student%20Persona.png "Especificacion de la persona alumno")
![Persona maestro](https://github.com/JoseBaezaP/IHC/blob/master/Image/personas/Teacher%20Persona.png "Especificacion de la persona maestro")
___

# Requisitos
Para la elaboración de este sistema, la dirección de centro de usos múltiples nos asignó a una maestra con la cual trabajaremos 
a lo largo de este proyecto.   
Al estar platicando con esta maestra, nos dío la oportunidad de ver su plan didáctico con la finalidad de plantear alguna idea
de los futuros temas que verá con su grupo. De esta manera se planteo realizar un sistema que le permita al maestro conocer en que temas tienen más problemas sus alumnos, de esta manera enfocarse en las áreas de mayor importancia. Estos resultados se realizaran por medio de una serie de actividades que los alumnos deberan realizar y el maestro podrá visualizar el resultado de cada alumnos para su retroalimentacion.

Esto se llevará acabo mediante la implementacion de un sistema movil en donde los usuarios puden darse de alta como maestros o alumnos.


| R001   |  Descripción    |  
|----------|:-------------:|
|  1| El sistema deberá permitir el acceso a los usuarios que tienen una cuenta. |

***

|R002    | Descripción     |  
|----------|:-------------:|
| 2| El sistema debera manejar un portal de acceso a los usuarios que tienen una cuenta.|
| 2.1 | El portal debe desplegar en la pantalla los campos de usuario y contraseña para validar el acceso.|
| 2.2| El portal de acceso debe mostrar en pantalla las respuestas obtenidas fallas al acceder. Datos incorrectos, Cuenta no existe.|

***
| R003   |      Descripción      |  
|----------|:-------------:|
| 3 | Los usuarios prodrán registrarse al sistema como maestros o alumnos. |
|3.1 | Debera llenarse un formulario con la siguiente información.|
| |  Nombres, Apellido Materno, Apellido Paterno, Correo, Contraseña. |

***
| R004 | Descripción |
|----|----|
| 4 | Un usuario del tipo Maestro puede crear grupos y agregar a sus alumnos por medio de un código de invitación.|

***
|R005  | Descripción   |
|----|----|
|5 | Un usuario del tipo Maestro puede visualizar a todos sus alumnos que pertenecen al grupo.

***
|R006  | Descripción   |
|----|----|
|6 | Un usuario del tipo Maestro puede visualizar la puntuacion obtenida de todos sus alumnos en cada ejercicio.

***
|R006  | Descripción   |
|----|----|
|6 | Un usuario del tipo Alumno pude seleccionar los diferentes ejercicios del area a realizar.
|6.1 | Las áreas son Español y Matemáticas. |

***
|R007  | Descripción   |
|----|----|
|7 | El sistema debe validar que la respuesta sea la correcta y notificarle a alumno.

***
|R007  | Descripción   |
|----|----|
|7 | Cada área deberá contar con una pequeña intruduccion del tema.

***
|R008  | Descripción   |
|----|----|
|8 | Los ejercicios cuentan con instrucciones, problema y posibles respuestas.
| 8.1 | Cada apartado del ejercicio debe estar traducido en Lengua de Señas Mexicanas.




___

# Metricas

La forma en la cual decimos medir el trabajo realizado entre nosostros fue de la siguiente forma:   
Porcentaje trabajado=(numero de actividades realizadas + reuniones asistidas/numero de total trabajos asignados + reuniones totales)/4   
***
#### Reuniones
- 1 Primera reunion en CAM 12.
- 2 Solicitud de oficios.
- 3 Entrega de oficios a la direcctora de CAM 12.
- 4 Planeacion de actividade con la directora.
- 5 realizacion de encuestas.

#### Actividades

#### Primera Entrega

- 1 Busqueda de información
- 2 Creacion de encuestas.
- 3 Aplicación de las encuestas   

| Nombre   |      Metrica     |   Porcentaje   |  
|:--------:|:----------------:|:-----:|
| Leonardo | (((3+4)/(3+5))/4)+.01  | 24  |
| Jose     | (((3+5)/(3+5))/4)+.01  | 26  |
| Ariel    | (((3+5)/(3+5))/4)+.01  | 26  |
| Nicolas  | (((3+4)/(3+5))/4)+.01  | 24  |

#### Segunda Entrega


