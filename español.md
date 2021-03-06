
# EQUIPO ROJO

## DESARROLLO Y OPERACIONES

## Una guía práctica

##### EDICIÓN DE DÍA CERO

```
Joe Vest y James Tubberville
```

```
©2019 Joe Vest y James Tubberville
```
Aviso de derechos de autor: Todos los derechos reservados. Ninguna parte de este libro puede ser reproducida o transmitida de ninguna
forma o por cualquier medio, electrónico o mecánico, incluyendo fotocopias, grabaciones, o por cualquier
sistema de almacenamiento y recuperación de información sin la autorización escrita del autor, excepto cuando
permitido por la ley.

[http://redteam.guide](http://redteam.guide)


## Declaración de los autores

"Se invierte mucho tiempo y dinero en proteger los activos digitales críticos. Muchas organizaciones
centran sus pruebas de seguridad en el cumplimiento o en revisiones de alcance limitado de un sistema. Estas pruebas limitadas
a menudo dejan a la organización con una falsa sensación de seguridad. Las organizaciones que se abren a una
evaluación no sólo de su tecnología, sino también de sus personas y procesos, pueden mejorar significativamente
su postura de seguridad y ajustar su limitado presupuesto y recursos de seguridad para proteger los activos más
activos más críticos. Las pruebas basadas en escenarios y las técnicas de los equipos rojos pueden utilizarse para determinar cómo una
organización se enfrenta realmente a una amenaza realista y determinada". - Joe Vest y James Tubberville

![Alt Image](./Images/1.png)

## Prefacio

Este libro es la culminación de años de experiencia en el campo de la tecnología de la información y la ciberseguridad
campo de la tecnología de la información y la ciberseguridad. Los componentes de este libro han existido como notas aproximadas, ideas, procesos informales y formales
desarrollados y adoptados por los autores mientras dirigían y ejecutaban compromisos de equipos rojos durante muchos
años. Los conceptos descritos en este libro se han utilizado para planificar, realizar y llevar a cabo con éxito
y llevar a cabo con éxito proyectos profesionales de equipos rojos de todos los tamaños y complejidades. Algunos de estos conceptos fueron
Algunos de estos conceptos se documentaron e integraron en los procesos de gestión de los equipos rojos, y muchos se mantuvieron como conocimiento tribal.
conocimiento tribal. Uno de los primeros intentos formales de capturar esta información fue el curso SANS SEC564 Red
El curso Red Team Operation and Threat Emulation fue uno de los primeros intentos formales de capturar esta información. Este primer esfuerzo fue un intento de documentar estas ideas
en un formato utilizable por otros. Los autores han ido más allá de la formación de SANS y utilizan este libro para
detallar las operaciones de los equipos rojos en una guía práctica.

El objetivo de los autores es proporcionar orientación práctica para ayudar en la gestión y ejecución de
equipos rojos profesionales. El término "equipo rojo" se confunde a menudo en el ámbito de la ciberseguridad. El término
raíces se basan en conceptos militares que poco a poco se han abierto paso en el espacio comercial.
Numerosas interpretaciones afectan directamente al alcance y la calidad de los compromisos de seguridad actuales. Esta confusión de
confusión ha creado una dificultad innecesaria cuando las organizaciones intentan medir las amenazas a partir de los
resultados de las evaluaciones de seguridad de calidad. La complejidad del red teaming se entiende rápidamente si
de la definición en Google, o mejor aún, buscando entre las numerosas definiciones e interpretaciones publicadas por los profesionales de la seguridad.
definiciones e interpretaciones publicadas por los profesionales de la seguridad en Twitter. Este libro fue escrito para
proporcionar una solución práctica para hacer frente a esta confusión.

El concepto de equipo rojo requiere un enfoque único y diferente de otras pruebas de seguridad. Se basa en gran medida
se basa en gran medida en TTPs bien definidos, críticos para la simulación exitosa de amenazas realistas y técnicas de los adversarios.
adversarios. Los resultados adecuados de los equipos rojos son mucho más que una simple lista de fallos identificados durante otras
pruebas de seguridad. Proporcionan una comprensión más profunda de cómo actuaría una organización frente a una
Una buena prueba de equipo rojo es mucho más que una simple lista de fallos identificados en otras pruebas de seguridad.

Ya sea que usted apoye un papel defensivo u ofensivo en la seguridad, entender cómo los Equipos Rojos pueden ser
para mejorar las defensas es extremadamente valioso. Las organizaciones gastan una gran cantidad de tiempo y dinero
en la seguridad de sus sistemas. Es fundamental contar con profesionales que comprendan la amenaza y puedan
operar de manera efectiva y eficiente sus herramientas y técnicas de forma segura y profesional. Este libro
le proporcionará la orientación del mundo real necesaria para gestionar y operar un Equipo Rojo profesional,
llevar a cabo compromisos de calidad, comprender el papel que desempeña un equipo rojo en las operaciones de seguridad. Usted
explorará en profundidad los conceptos de los equipos rojos, comprenderá los fundamentos de la emulación de amenazas
y comprenderá las herramientas necesarias para reforzar la postura de seguridad de su organización.

¿A quién va dirigido este libro?
```
● Profesionales de la seguridad interesados en ampliar sus conocimientos sobre Red Teaming.
● Probadores de penetración o hackers éticos que buscan entender cómo el Red Teaming es diferente de otros tipos de pruebas de seguridad.
● Defensores que quieren entender mejor las metodologías, herramientas y técnicas ofensivas.
● Auditores que necesitan construir habilidades técnicas relevantes y entender cómo medir el éxito.
● Miembros de equipos rojos que buscan entender mejor su oficio como profesionales.
● Cazadores de amenazas que buscan entender mejor cómo el red teaming puede aumentar su capacidad de defensa.
● Equipos de defensa o explotación de redes informáticas (CND/CNE).
● Especialistas forenses que quieran entender mejor las tácticas ofensivas.
● Directores de seguridad de la información que necesitan incorporar las actividades de los equipos rojos a sus operaciones.
```

En resumen, este libro le preparará para:
```
● Aprender qué es el Red Teaming y en qué se diferencia de otros compromisos de pruebas de seguridad.
● Comprender la visión única del campo de la seguridad ofensiva del Red Teaming y los conceptos, principios y directrices fundamentales para su éxito.
● Diseñar y crear objetivos específicos de amenazas para medir y entrenar a los defensores de la organización.
● Aprender a utilizar la metodología "Get In, Stay In, and Act" para lograr impactos operativos.
● Diseñar, operar y ejecutar un programa profesional de red teaming.
● Hacer el mejor uso de un equipo rojo y aplicarlo para medir y comprender las defensas de seguridad de una organización.
```

## Agradecimientos

Escribir este libro ha sido un viaje intenso y muchos obstáculos han mostrado su cara. La vida
no se detiene y te da tiempo para cumplir con los plazos. Sin el apoyo de la familia, los amigos, los compañeros de trabajo
y la comunidad de infoseguridad, este libro no se habría escrito. Gracias a todos.

Este libro es una colección de pensamientos, ideas y experiencias. Muchas de estas ideas y conceptos
no se habrían desarrollado sin las personas con las que hemos trabajado en los últimos diez años. Queremos agradecer
Queremos dar las gracias a todos los que nos han escuchado divagar durante horas. Ustedes son tan parte de este libro como nosotros.
parte de este libro como nosotros.

Tenemos que dar las gracias especialmente a la familia y a los amigos cercanos. Leer los primeros borradores, escuchar las divagaciones
de seguridad, dando consejos, manteniéndonos sinceros y animándonos a seguir en el camino, son sólo algunas de las formas en que nos habéis ayudado.
maneras en que nos ayudaron. Este libro no se habría escrito sin vuestro aliento y apoyo.
Os damos las gracias y os queremos a todos.

Queremos nombrar a todos por su nombre, pero no queremos dejar de mencionar a alguien involuntariamente. Estrecharemos
su mano o le daremos un abrazo la próxima vez que le veamos.

Os animamos a todos a alcanzar vuestras metas.


## Cómo utilizar el libro

Este libro se ha escrito para ofrecer un enfoque práctico para crear y dirigir un Red
profesional. El libro está dividido en capítulos que coinciden aproximadamente con las fases de un compromiso del Equipo Rojo.
Los capítulos comienzan profundizando en un tema específico para proporcionar antecedentes y detalles sobre diversos temas del Equipo Rojo.
de los equipos rojos. Cada capítulo finaliza con los puntos clave del capítulo y las tareas para casa. Los puntos clave del capítulo
resumen del capítulo y los deberes enumeran los pasos que el lector debe dar para aplicar los temas específicos.
temas específicos. El trabajo en casa permite crear los elementos necesarios para un equipo profesional de Red
profesional. Estos elementos pueden utilizarse como hoja de ruta para ayudar a un equipo a desarrollarse y crecer.


### Sitio web complementario (http://redteam.guide)

Este libro tiene un sitio web complementario, **[http://redteam.guide.](http://redteam.guide.)** Este sitio web contiene información adicional
información adicional, plantillas, guías, laboratorios y otra información útil que ayuda a mejorar el contenido del libro.
del libro.


## Índice de contenidos

**DECLARACIÓN DE LOS AUTORES**

**PREFACIO**

**AGRADECIMIENTOS**

**CÓMO UTILIZAR EL LIBRO

```
SITIO WEB COMPLEMENTARIO (HTTP://REDTEAM.GUIDE)
```
**ÍNDICE DE CONTENIDOS

**INTRODUCCIÓN

```
LOS EQUIPOS ROJOS EN LAS PRUEBAS DE SEGURIDAD
ORGANIZACIONES DE EQUIPOS ROJOS
PRINCIPALES CONCLUSIONES DEL CAPÍTULO
TRABAJO EN CASA
```
PLANIFICACIÓN DEL COMPROMISO

```
COSTE Y FINANCIACIÓN
ALCANCE
DURACIÓN
COSTE DE LA MANO DE OBRA DEL PERSONAL
COSTE DEL EQUIPO Y DEL SOFTWARE
COSTE DE VIAJE
COSTE PREVIO Y POSTERIOR AL COMPROMISO
FRECUENCIA
NOTIFICACIONES DE COMPROMISO
FUNCIONES Y RESPONSABILIDADES
NORMAS DE ACTUACIÓN (ROE)
GESTIÓN DEL RIESGO
PLANIFICACIÓN DE LA AMENAZA
PERFIL DE LA AMENAZA
CREACIÓN DE UN PERFIL DE AMENAZA MEDIANTE LA DESCOMPOSICIÓN DE UNA AMENAZA
REVISIÓN DE LA TÉCNICA DE UN BLACKHAT
PERSPECTIVA DE LA AMENAZA
ESCENARIO DE LA AMENAZA
EMULACIÓN DE LA AMENAZA
MODELOS DE ESCENARIOS
INDICADORES DE COMPROMISO
CONCEPTOS DE COMPROMISO
DECONFLICCIÓN
MANEJO DE DATOS
PRINCIPALES CONCLUSIONES DEL CAPÍTULO
TRABAJO EN CASA
```
**EJECUCIÓN DEL COMPROMISO**

```
DEPÓSITO DE DATOS
RECOGIDA DE DATOS
TRADECRAFT
ORIENTACIÓN GENERAL
CONCEPTOS DE EJECUCIÓN
HERRAMIENTAS Y EJEMPLOS DE HERRAMIENTAS
MANDO Y CONTROL (C2)
PRINCIPALES CONCLUSIONES DEL CAPÍTULO
TRABAJO EN CASA
```
**CULMINACIÓN DEL COMPROMISO**

```
SANITIZACIÓN Y LIMPIEZA
VERIFICACIÓN DEL REGISTRO DEL OPERADOR
REUNIONES INFORMATIVAS PREVIAS AL INFORME
PRINCIPALES CONCLUSIONES DEL CAPÍTULO
TRABAJO EN CASA
```
**INFORMES DE COMPROMISO**

```
DIAGRAMAS DE FLUJO DE ATAQUE
OBSERVACIONES VS. HALLAZGOS
CLASIFICACIÓN Y MÉTRICAS DE RIESGO
COMPARACIÓN DE MATRICES DE RIESGO
NARRACIÓN DE LOS ATAQUES
PRINCIPALES CONCLUSIONES DEL CAPÍTULO
TRABAJO EN CASA
```
**RESUMEN**

**CONCLUSIÓN**

**APÉNDICE A: PLANTILLAS DE EJEMPLO**

**APÉNDICE B: EJERCICIOS DE REFLEXIÓN**

```
DESAFÍO DE MENTALIDAD ADVERSA
COMENTARIOS Y RESPUESTAS AL DESAFÍO MENTAL
```
**APÉNDICE C: EJERCICIO DE DESCOMPOSICIÓN DE UNA AMENAZA**

```
DESCRIPCIÓN
ESCENARIO DEL EJERCICIO
OBJETIVO
RECURSOS
COMENZAR EL EJERCICIO
CREAR UN PERFIL DE AMENAZA
POSIBLE SOLUCIÓN
```
**GLOSARIO DE TÉRMINOS**


## Introducción

Diseñar, desplegar y gestionar un programa de seguridad integral es complejo y desafiante
y, por lo tanto, no es una tarea fácil para la mayoría. Las organizaciones se ven influenciadas y presionadas por múltiples
a menudo en competencia, de múltiples fuentes. Esta presión puede provenir de los clientes, el cumplimiento, la dirección, los compañeros
las finanzas, la opinión pública y las noticias de dominio público, por nombrar algunas. Incluso cuando se enfrentan a estos
desafíos, las organizaciones suelen ser capaces de superar estas presiones e implementar lo que se
lo que se considera un programa de seguridad sólido. Las organizaciones pueden satisfacer a las distintas partes y, al menos
sobre el papel, describir un programa de seguridad diseñado para detener los ciberataques maliciosos. Como resultado, las auditorías y
auditoría y de cumplimiento, se despliegan sólidos sistemas de gestión de parches y se llevan a cabo
de vulnerabilidad y pruebas de penetración. Estos son pasos iniciales significativos para proporcionar
los medios para defender una red de los ataques. Desgraciadamente, a menudo esto se queda corto para lograr el
objetivo principal de prevenir, detectar y responder a las amenazas reales. ¿Por qué? ¿Qué es lo que falta? La verdadera
pregunta a considerar es:

### ¿Están las organizaciones creando realmente programas de seguridad diseñados para hacer frente a la amenaza?

Un programa de seguridad incluye muchos componentes, como personal, políticas, procedimientos, herramientas, gestión
supervisión, respuesta a incidentes, etc. El programa se diseña y construye con la ayuda de miembros
de varias divisiones o funciones de trabajo diferentes, que aportan sus ideas y requisitos de seguridad.
de seguridad. Los programas de seguridad suelen utilizar esta estrategia para garantizar un programa de seguridad completo y holístico.
Sin embargo, ¿qué o quién falta a menudo? ¿Alguien del equipo de operaciones de seguridad ha
¿ha visto alguna vez a un tipo malo? ¿Alguien del equipo ha atacado o puesto en peligro una red? ¿En qué medida? En 
citar a Peter en la película Office Space[1]. "No puedo creer que seamos una panda de empollones. Estamos
Estamos buscando en el diccionario sobre el lavado de dinero".
no conocen ni entienden?

### ¿Se incluye la amenaza en la planificación de la seguridad?

Las buenas intenciones de un grupo de personas inteligentes no se suman a la comprensión de las amenazas o de cómo
operan. Si el objetivo de las operaciones de seguridad es prevenir, detectar, responder y recuperarse de las acciones maliciosas
Si el objetivo de las operaciones de seguridad es prevenir, detectar, responder y recuperarse de las acciones maliciosas, sólo tiene sentido incluir las opiniones de aquellos a los que se está defendiendo.
Desgraciadamente, el diseño de la seguridad suele excluir la perspectiva de las amenazas o de los peligros. Esta omisión suele
Esta omisión a menudo conduce a la mitigación o aceptación de riesgos que no se comprenden o revelan durante las
pruebas y auditorías de seguridad tradicionales. El resultado es una falsa sensación de seguridad grave. Una amenaza real lo sabe
y lo utiliza en su beneficio.

```
Considere esto:
¿Sabe una amenaza que un objetivo tiene un sólido programa de seguridad?
¿Realizan las amenazas acciones que desencadenan una alerta o hacen que las atrapen?
¿Siguen teniendo éxito las amenazas?
Si es así, ¿por qué las amenazas son capaces de lograr sus objetivos con éxito y de impactar negativamente en una organización cuando ésta tiene un programa de seguridad completo? 
Para entender esto debemos comprender la amenaza para desarrollar las defensas adecuadamente.
```

El sector de la seguridad utiliza el término amenaza, pero ¿qué es una amenaza?

**Dictionary.com** [2] define la amenaza como
una declaración de intención o determinación de infligir un castigo, una lesión, etc., en represalia por, o
una amenaza una indicación o advertencia de un probable problema una persona o cosa que amenaza.
persona o cosa que amenaza.

**ISO 27001** [3] define la amenaza como:
Una causa potencial de un incidente, que puede resultar en el daño de los sistemas y la organización.

**NIST** [4] define la amenaza como:
Cualquier circunstancia o evento con el potencial de impactar adversamente las operaciones de la organización (incluyendo
misión, funciones, imagen o reputación), activos de la organización, individuos, otras organizaciones o
la Nación a través de un sistema de información mediante el acceso no autorizado, la destrucción, la divulgación
modificación de la información o denegación de servicio.

Veamos esto en el contexto de las amenazas a la ciberseguridad. Una amenaza es un evento que tiene el
potencial para impactar negativamente en una organización. ¿Los equipos de operaciones de seguridad se están defendiendo contra esta
amenaza? ¿Un evento negativo? Tal vez, pero considere la posibilidad de incluir el término amenaza-actor cuando utilice el término amenaza. A
amenaza-actor es la persona o grupo de personas que está detrás de un ataque. Una estrategia defensiva sólida debe defenderse
contra un actor-amenaza inteligente decidido a causar daños a una organización y no sólo un
evento potencial. Las personas están detrás de los ciberataques. Cuando la defensa considera las tácticas, técnicas
y procedimientos (TTPs) de los actores-amenaza inteligentes, empiezan a entender la verdadera amenaza. Los defensores
pueden entonces implementar sólidas defensas de seguridad que impactan directamente en la capacidad que tiene un actor de amenaza para
realizar acciones dañinas. Cambiar las operaciones de seguridad desde la mentalidad de "Vulnerable" o "No
Vulnerable" y adoptar un enfoque que se centre en las acciones de las amenazas mejorará significativamente la
capacidad de una organización no sólo para prevenir, sino también para detectar y responder a las amenazas reales. Profundizar en los
TTPs es el comienzo de la comprensión de la seguridad a través de los ojos de la amenaza. Las organizaciones que utilizan
las acciones de las amenazas para impulsar sus TTP defensivos pueden hacer la vida muy difícil a los actores de las amenazas e incluso
protegerse contra ataques desconocidos o de día cero.

#### ¿Por qué tienen éxito las amenazas?

Muchas organizaciones utilizan actualmente la auditoría y el cumplimiento, las evaluaciones de vulnerabilidad y las pruebas de penetración
para evaluar y medir el riesgo de ciberataque. ¿Por qué preocuparse por un nuevo enfoque centrado en las amenazas?

### ¿No es suficiente la identificación y mitigación de las vulnerabilidades?

Para responder, hay que entender cómo piensa y actúa un actor de amenazas. Recuerde, una amenaza es realmente una
persona inteligente decidida a causar daño. NO es un exploit de una vulnerabilidad, NO es un trozo de
malware, ni un ataque de phishing. Estos son simplemente los medios que un actor de la amenaza puede elegir para lograr
su objetivo final. El actor de la amenaza asume que el objetivo tiene un programa de seguridad completo y un conjunto de herramientas de seguridad (cortafuegos, etc.).
de herramientas de seguridad (cortafuegos, sistemas de detección de intrusos, antivirus, EDR, etc.) desplegados con la
intención de detener los ciberataques. Un buen actor de amenazas probablemente asumirá que una organización ha desplegado
parches, ha realizado evaluaciones de vulnerabilidad para reducir la superficie de ataque de los exploits y ha realizado
pruebas de penetración para identificar las rutas de ataque. Esta comprensión puede cambiar significativamente las acciones tomadas
por un actor de la amenaza. Estas acciones pueden ser muy diferentes en comparación con las acciones tomadas por un probador de seguridad tradicional.
de seguridad tradicional. ¿El actor de la amenaza dispara un escáner de puertos y enumera toda una red? ¿Realiza un
¿ejecuta un actor de amenazas una herramienta de escaneo de vulnerabilidades para encontrar un exploit? Los ataques de los actores de amenazas no
no siempre siguen los modelos adoptados por las pruebas de seguridad tradicionales. Un ataque no es escaneo -> explotación ->
beneficio. Un actor de amenazas inteligente evalúa lo que presenta un objetivo y utiliza puntos débiles que no siempre
descubiertos a través de las pruebas de seguridad tradicionales. Un "buen" actor de amenazas dará varios pasos controlados
para obtener acceso a un objetivo, establecer el mando y el control, establecer la persistencia, realizar el conocimiento de la situación
para lograr el objetivo deseado. Las personas encargadas de defender una
organización a menudo ignoran o malinterpretan los pasos que da un actor de la amenaza. Esta incomprensión
a menudo conduce a centrarse en la prevención, no en la detección. Los defensores que se centran en la detección pueden ahogarse
en registros y alertas por defecto o generados por el proveedor. ¿Has oído alguna vez a un analista de
analista de operaciones de seguridad decir: "Tenemos demasiados registros y alertas para responder" o "¡Sólo estamos tratando de mantener el volumen de tickets!
o "¡Intentamos seguir el ritmo del volumen de tickets! ¿Por qué las organizaciones registran lo que registran? ¿Cumplimiento? En
caso de que se necesiten? ¿Por consejo de un proveedor? A las organizaciones les sigue faltando una pieza clave para todas las amenazas;
entender sus acciones y TTPs.

#### Considere este escenario

Después de evaluar una red objetivo, un actor de la amenaza decide que el phishing es su método elegido para obtener
acceso. Envía un correo electrónico de phishing a un pequeño número de personas. El phishing contiene un archivo adjunto
Excel con un ataque basado en DDE[5]. Uno de los destinatarios del correo electrónico abre el archivo adjunto. Este
Esto lanza el código malicioso y establece el comando y control (C2). El actor de la amenaza lleva a cabo una serie de
una serie de pasos que incluyen el conocimiento de la situación del acceso actual, la enumeración de nuevos objetivos potenciales y la identificación de opciones de movimiento lateral.
objetivos, y la identificación de opciones de movimiento lateral hacia esos objetivos. En este caso, la amenaza encuentra
credenciales de base de datos en texto claro en una copia de seguridad de una aplicación web de prueba antigua en un recurso compartido público. La aplicación
La aplicación web no tiene importancia directa ni datos críticos, salvo el acceso a una base de datos de prueba sin
datos críticos. Es sólo una aplicación de prueba. Las credenciales proporcionan los medios para moverse lateralmente a un servidor de base de datos de prueba.
servidor de base de datos de prueba. Recuerde, la base de datos no tiene datos sensibles pero es parte de la "zona de servidores"
en la red. La ejecución del código en el servidor de la base de datos proporciona un acceso elevado. El ciclo de conocimiento de la situación se repite.
El ciclo de conocimiento de la situación se repite. El actor de la amenaza descubre credenciales elevadas almacenadas en la memoria del
servidor de la base de datos. La amenaza extrae este material de credenciales y lo utiliza para comunicarse con un controlador de dominio de Windows
controlador de dominio de Windows para extraer una credencial elevada aún mayor de un controlador de dominio de Windows
utilizando la técnica dcsync[6]. El actor de la amenaza repite el ciclo de conocimiento de la situación y enumeración
utilizando las credenciales recién obtenidas del controlador de dominio. El objetivo previsto se identifica
y localizado en un repositorio de archivos sensibles. El actor-amenaza se preposiciona utilizando el acceso
e información obtenida y logra su objetivo final exfiltrando datos sensibles de la
red.

Responde a las siguientes preguntas como si fueras parte de la organización objetivo.

```
¿Es razonable este escenario?
¿Se presentaron oportunidades para detectar o prevenir la amenaza?
¿Podría su programa de seguridad actual prevenir, detectar o responder a esta amenaza?
¿Está seguro?
¿Lo ha verificado?
Si es así, ¿cómo?
¿Qué técnicas o indicadores dejó esta amenaza?
```
Las organizaciones suelen culpar al usuario final que hizo clic en el enlace. Este escenario indica que todo el modelo de seguridad
modelo de seguridad de una organización puede depender de que los usuarios no hagan clic en un enlace de un correo electrónico. ¿Qué pasa con las acciones que la
amenaza después del clic inicial? Muchas organizaciones no pretenden que toda la seguridad dependa de un único
usuario, pero las medidas tomadas para defender los sistemas suelen decir lo contrario.

```
Considere lo siguiente
Un ataque de phishing que lleva a un compromiso NO es culpa de un usuario final, sino de los insuficientes controles de seguridad de un entorno objetivo. 
A menudo se culpa a los usuarios finales del compromiso debido a un ataque de phishing. 
Las defensas de seguridad no están pensadas para depender de la decisión de un usuario de hacer clic o no.
Si un usuario que es víctima de un ataque de phishing lleva a un compromiso de todo el sistema, ese usuario ya tenía el potencial de elevar los privilegios o comprometer de otra manera el entorno.
```
#### ¿Por qué tiene éxito este escenario?

Las organizaciones suelen tener una mentalidad errónea en cuanto a la defensa de la seguridad.

**Se culpa a los usuarios por hacer clic en los enlaces**.  
La educación del usuario es sólo una pieza de defensa en las operaciones de seguridad. Los usuarios harán clic. Es su trabajo.

**Las políticas, los procedimientos y el cumplimiento miden la seguridad**.  
Son extremadamente importantes para un programa de seguridad, pero a menudo sólo representan el mínimo necesario para
cumplir con una norma. Trate el cumplimiento como el palo en un parque de atracciones. Hay que ser "así de alto" para montar.

**Registrar todo; nunca se sabe lo que se necesita**  
Las operaciones de seguridad a menudo registran una enorme cantidad de datos inviables. El registro puede deberse a
requisitos de cumplimiento, recomendaciones de los proveedores, falta de comprensión de las fuentes de datos, o una mentalidad de "más vale prevenir que curar".
que lamentar". Esta incomprensión conduce a cuellos de botella y a la sobrecarga de los analistas de seguridad.
de seguridad.

**Parche, parche, parche. Las amenazas sólo utilizan exploits**  
Un malentendido o punto de vista común es que las amenazas sólo utilizan exploits. Esto está muy lejos de la realidad. El parche
La gestión de parches es un factor esencial en un programa de seguridad integral que ayuda a reducir la superficie de ataque.
de ataque. Las amenazas entienden esto y pueden cambiar sus tácticas. Este concepto se explora más a fondo y se
discutido en el texto como "explotación sin exploits".

**Nuestras herramientas de seguridad nos salvarán  
La industria de la seguridad depende en gran medida de las herramientas de seguridad. Por desgracia, muchos no saben cómo funcionan estas
herramientas. La falta de conocimiento lleva a una mala puesta a punto y a una mala configuración. Las herramientas deberían
mejorar la eficiencia y la capacidad de nuestros defensores y analistas de seguridad y no dirigir directamente las operaciones de seguridad.
operaciones de seguridad directamente. Son herramientas. Un martillo y unos clavos no construirán una casa sin un carpintero.

Hay numerosas razones por las que el escenario anterior tiene éxito. Estas viñetas son intentos de humor
son intentos de humor; la mayoría de las veces se trata de problemas en las prácticas y procesos de pensamiento de las organizaciones del mundo real.
organizaciones del mundo real.

#### ¿Cómo podemos resolver este dilema?

Podemos resolverlo mediante ejercicios basados en el Red Teaming. El Red Teaming capta la perspectiva de la amenaza.
Inspirado en la filosofía militar, muchas industrias han descubierto la virtud de "Red Teaming" una
capacidad defensiva, y que su eficacia aumenta cuando se pone a prueba en condiciones reales de campo de batalla.
El mero estudio de las tácticas de una amenaza es menos útil que experimentarlas realmente. Las amenazas simuladas
Las amenazas simuladas generan confianza y memoria muscular en los defensores de la red y los dotan de un mejor conocimiento situacional de las herramientas y las tácticas.
de las herramientas y las tácticas, así como las lecciones aprendidas de los fallos simulados.

El Red Teaming puede denominarse emulación de amenazas, simulación de amenazas, emulación de adversarios
simulación de adversarios, o alguna otra frase que exprese un enfoque de las pruebas de seguridad basado en las amenazas.

Antes de adentrarnos en los conceptos del red teaming, debemos nivelar nuestras definiciones. A
Un léxico común es crítico para mantener a todos en la misma página para asegurar que mantenemos una base común
una base común e imparcial de entendimiento. Los autores de este libro han visto cómo los términos malinterpretados causan graves
complicaciones y expectativas perdidas. Los conceptos se definirán y explicarán a lo largo de este libro.
Comenzamos definiendo el red teaming.

### El Red Teaming es el proceso de utilizar Tácticas, Técnicas y Procedimientos (TTPs) para emular una amenaza del mundo real con el objetivo de entrenar y medir la eficacia de las personas, los procesos y la tecnología utilizados para defender un entorno.

Las suposiciones, los prejuicios, los malentendidos y la incredulidad tienen un impacto significativo en las operaciones de seguridad de un entorno.
operaciones de seguridad de un entorno. Los equipos rojos proporcionan evaluaciones formidables y honestas de las prácticas internas y los controles de seguridad.
prácticas internas y controles de seguridad al desafiar las suposiciones, ignorar las normas y exponer la atrofia
y los prejuicios. Un análisis imparcial mediante Red Teaming mide la diferencia entre "lo que es" y "lo que
debería ser". La aplicación del red teaming proporciona una verdad de base imparcial y un conocimiento profundo
de las operaciones de seguridad en su conjunto.

El Red Teaming personifica la práctica de atacar los problemas desde un punto de vista adverso. Esta
mentalidad desafía una idea para ayudar a probar su valor, identificar los puntos débiles o identificar las áreas a mejorar.
Los sistemas complejos son desarrollados, diseñados e implementados por profesionales cualificados y de confianza. Estos
Estos individuos son muy respetados y de confianza en su campo y son muy capaces de diseñar y desarrollar sistemas funcionales.
y desarrollar sistemas funcionales. Aunque estos sistemas son altamente funcionales y capaces, las ideas,
conceptos y pensamientos a veces pueden estar "encajonados", lo que lleva a suposiciones incorrectas sobre cómo funciona honestamente un
sistema funciona honestamente. La gente construye sistemas, y la gente hace suposiciones sobre la capacidad
funcionalidad y seguridad. Estas suposiciones conducen a defectos de los que puede aprovecharse una amenaza.

El Red Teaming proporciona un medio para desafiar y poner a prueba la sabiduría y el pensamiento convencionales. Algunos
métodos estándar para aplicar los escenarios de Red Teaming son:

**Ejercicios de mesa** - Una actividad en la que personas clave recorren una situación simulada para responder a preguntas del tipo "¿qué pasaría si?
preguntas "qué pasaría si". No se realizan pruebas técnicas reales. Los debates sobre los posibles resultados se
Se exploran y examinan los posibles resultados en un formato de debate abierto.  
**Ataques físicos** - Un ataque a un recurso físico, como una instalación o un edificio, para probar escenarios
basado en rutas de ataque que involucran activos físicos.  
**Ataques humanos** - Un ataque que implica la ingeniería social y la manipulación de personas para
para lograr los objetivos del Equipo Rojo.  
**Ejercicios cibernéticos** - Un ejercicio rojo contra azul diseñado para entrenar o evaluar al personal y las defensas de las operaciones de seguridad.
defensas. Los ejercicios pueden ir desde un escenario de amenaza ofensiva focalizada hasta un juego de guerra rojo contra azul.
juego.  
**Operación cibernética a gran escala** - El ataque más realista que una organización puede soportar fuera de un ataque
de una amenaza real. Los elementos de la operación evalúan colectivamente todos los aspectos de un escenario específico.
El escenario impulsa la necesidad y puede aprovechar las debilidades físicas, humanas y cibernéticas para lograr
objetivos deseados.

El Red Teaming no se centra en una vulnerabilidad o debilidad como un único "hallazgo". Durante un compromiso de Red Team
un operador puede encontrar un sistema sin parches o mal configurado. Este defecto puede ser utilizado para
para proporcionar un compromiso más extenso en una red o para pivotar desde el sistema
sistema vulnerable para lograr un objetivo específico o puede no ser utilizado en absoluto. Aunque un solo sistema no parcheado o
sistema no parcheado o mal configurado puede dar a un operador del equipo rojo los medios para comprometer una red, es sólo un
medio para un fin. Este es un distintivo crucial para el Red Teaming.

#### Los compromisos de los equipos rojos se centran en metas y objetivos específicos.

Estos objetivos pueden incluir comprometer una aplicación o red, robar datos, emular un objetivo específico, medir la eficacia de las defensas técnicas.
emular un objetivo específico, medir la eficacia de las defensas técnicas, medir la eficacia de un equipo de seguridad, etc.
equipo de seguridad, etc. Las vulnerabilidades y debilidades identificadas durante una evaluación pueden necesitar ser
Las vulnerabilidades y debilidades identificadas durante una evaluación pueden necesitar ser abordadas y mitigadas, pero este no es el objetivo del Red Teaming. El Red Teaming se centra en el panorama general
El Red Teaming se centra en el panorama general al proporcionar una visión de las capacidades de detección y respuesta de un objetivo. Permite comprender
El tiempo medio de detección (MTTD) y el tiempo medio de recuperación (MTTR) de las infracciones individuales. En
ejercita la relación entre sus equipos de respuesta a incidentes y de caza de amenazas poniendo a prueba a los defensores de la red y sus herramientas de forma
defensores de la red y sus herramientas de maneras que no se pueden lograr a través de la inteligencia de amenazas tradicional,
la literatura, o las pruebas estructuradas.

Las siguientes categorías resumen los objetivos del Red Teaming.

**Medir la eficacia de las personas, los procesos y la tecnología utilizados para defender una red**.  
Cuando un equipo rojo utiliza técnicas de ataque del mundo real contra la red de producción de un objetivo, el alcance
de las defensas de la organización. Por ejemplo, un compromiso tiene el objetivo de robar
datos críticos de un objetivo. Un ataque de phishing dirigido pone a prueba la voluntad del usuario final de participar en
un ataque. La carga útil del ataque pone a prueba las defensas de la red y del host contra la entrega de
malware y, en última instancia, contra la ejecución de código. Si el ataque desencadena un control defensivo, la
respuesta mide las acciones del defensor para identificar, responder o detener el ataque. Red
El Red Teaming proporciona un medio para medir las operaciones de seguridad en su conjunto y no sólo centrarse en los controles técnicos.
controles.

**Formación o medición de las operaciones defensivas o de seguridad**

### "No nos elevamos al nivel de nuestras expectativas; caemos al nivel de nuestra formación". 
### - Arquíloco, poeta griego, alrededor del año 650 a.C.

La formación del Equipo Azul (defensores de una red) es uno de los aspectos más valiosos de los Equipos Rojos.
Sin formación, ¿cómo se espera que los defensores se defiendan de un ataque real? Los ejercicios en el aula
Los ejercicios en el aula y la formación conceptual son valiosos; sin embargo, los equipos rojos ofrecen la posibilidad de que las operaciones defensivas
para desarrollar habilidades contra una amenaza en un entorno seguro y productivo. El liderazgo que espera que su
equipo de defensa responda a esa amenaza sin practicar y se defienda con éxito se está engañando
a sí mismos. Esta forma de formación es más práctica que los típicos cursos de seguridad. El mundo real
La práctica del mundo real de las personas que utilizan la tecnología y siguen sus procesos es necesaria para comprender la capacidad de defensa de las operaciones de seguridad.
de las operaciones de defensa.

**Prueba y comprensión de amenazas específicas o escenarios de amenazas**


Un equipo rojo puede ejecutar y emular una amenaza actual, nueva o personalizada como parte de un compromiso para probar
o validar la eficacia de los controles de seguridad. Los escenarios de emulación de amenazas distinguen el red teaming
de otros tipos de evaluaciones de seguridad y pueden utilizarse para comprender la postura de una organización
contra diversas amenazas. Este enfoque proporciona los medios para probar escenarios basados en nuevas
amenazas no descubiertas o explotaciones de día cero. Un gran ejemplo es el exploit EternalBlue[7]. Este exploit
implicaba la ejecución remota de código utilizando el protocolo SMB, un protocolo clave utilizado en los entornos de Microsoft
de Microsoft. Antes de que se conociera el exploit, un Red Team podría haber diseñado fácilmente un escenario
donde un atacante fuera capaz de propagarse a través del protocolo SMB para medir el impacto de este tipo de
ataque peligroso. Los equipos rojos no necesitan (o no deberían) esperar a que se desarrolle una amenaza y las vías de ataque.
Los escenarios personalizados son una gran manera de entender las amenazas actuales y futuras. Se puede encontrar más información
encontrar en ExternalBlue en CVE-2017-0144.

```
Recuerde esto
Los equipos rojos se utilizan para medir la eficacia de las personas, los procesos y la tecnología utilizados para defender una
red, entrenar o medir a un Equipo Azul (operaciones de seguridad defensiva), y probar y comprender amenazas específicas o
escenarios de amenazas.
```
Hemos descrito lo que hacen los Equipos Rojos, pero vamos a darles una definición para añadirla a nuestro léxico común.
Un Equipo Rojo es un grupo independiente que, desde la perspectiva de una amenaza o adversario, explora
planes y operaciones alternativas para desafiar a una organización a mejorar su eficacia.

Los equipos rojos llevan a cabo acciones durante un compromiso de Red Teaming, que se describen en las Reglas de Enfrentamiento
(ROE). Más adelante hablaremos en detalle de estas reglas. Por ahora, considérelas como una guía utilizada por un Equipo
de los equipos rojos sobre cómo deben realizar sus acciones. Los Equipos Rojos son grupos independientes que están técnicamente
técnicamente y capaces de ejecutar un plan basado en amenazas de forma segura y profesional.

Seguimos describiendo a los Equipos Rojos como "independientes". ¿Por qué? Como se ha dicho, muchas organizaciones o grupos
tienen importantes prejuicios y suposiciones basadas únicamente en información no probada o no confirmada. Un
Un equipo rojo independiente, que no esté obstruido por los prejuicios del objetivo, puede proporcionar una revisión limpia, una perspectiva
perspectiva fresca, y una evaluación precisa de cómo una amenaza puede causar un impacto en varias funciones de negocio.
funciones empresariales. Este equipo puede ser un consultor externo o un equipo interno gestionado y operado
separado del resto de la organización. Las revisiones independientes tienen un valor incalculable para determinar los riesgos y las consecuencias del mundo real.
de los riesgos y consecuencias del mundo real y un componente clave del Red Teaming.

```
Considere lo siguiente
Los equipos rojos independientes tienen un valor incalculable para determinar los riesgos del mundo real y las posibles consecuencias.
La independencia permite que el equipo rojo revise o evalúe con precisión, limitando muchos de los sesgos y
suposiciones del objetivo.
```

¿Cuál es la diferencia entre un Equipo Rojo y un atacante del mundo real? Un Equipo Rojo proporcionará un
informe, u otros entregables, con el objetivo de comprender los riesgos basados en las amenazas. Las organizaciones que utilizan
Los equipos rojos no necesitan esperar para aprender de una violación en el mundo real. Los equipos rojos son
beneficiosos para analizar los sistemas en busca de debilidades de seguridad que pueden no ser conocidas o comprendidas. El
La mentalidad y los procesos de pensamiento utilizados por un operador de equipo rojo profesional pueden
suposiciones comunes que debilitan gravemente la seguridad de un sistema. Los equipos rojos hacen preguntas del tipo "qué pasaría si" para
desafiar las defensas del sistema en su núcleo. El uso eficaz de los equipos rojos puede sacar a la luz fallos de seguridad
de seguridad que han plagado un sistema durante años y permitir que una organización desarrolle soluciones de mitigación altamente efectivas.
soluciones de mitigación muy eficaces.

Aunque los equipos rojos tienen enormes ventajas, su uso puede resultar complicado. Son
comúnmente utilizados sólo de nombre. Las actividades realizadas durante un compromiso no son más que una
prueba de vulnerabilidad o de penetración. El resultado puede ser algo tan simple como una lista de hallazgos. Red
Los equipos deben ser capaces de pensar y actuar como si se tratara de una amenaza. Estos compromisos pueden ser una
guante, una amenaza avanzada o acciones limitadas para emular una amenaza simple o directa. En este sentido
discutiremos cómo hacer esto "ajustando el volumen" de los ataques y la gestión del Indicador de Compromiso (IOC)
más adelante. Por ahora, entienda que un Equipo Rojo debe operar dentro de sus reglas y límites
y centrarse en los objetivos establecidos en el plan de compromiso.

El Red Teaming se centra en la historia general. Los equipos rojos pueden documentar las vulnerabilidades y debilidades
identificadas durante una evaluación, pero se centran en la historia completa del atacante a lo largo de un compromiso.

```
Tenga en cuenta lo siguiente
Las suposiciones, los prejuicios, los malentendidos y la incredulidad tienen un impacto considerable en los fallos de seguridad de
un entorno.
Un Equipo Rojo imparcial ayuda a medir la brecha entre "lo que es" y "lo que debería ser" para llegar a la verdad de
las operaciones de seguridad en su conjunto.
```
#### Consideremos lo siguiente.

Durante la planificación temprana del escenario del equipo rojo, la dirección de seguridad de una organización describe quién tiene
acceso a sus sistemas contables. Dicen: "5 personas de contabilidad tienen acceso al sistema de
sistema de contabilidad". En sus mentes, esto es lo que " **es** ". Cuando se planifica un escenario de amenaza, hay que pensar que esto es lo que
" **Debería ser". Este escenario es la oportunidad perfecta para que un Equipo Rojo valide las suposiciones en un
profesional e imparcial. El objetivo no es demostrar que se puede "hackear" el sistema, sino
entender lo que " **es** " frente a lo que " **debería ser** ".

![Alt Image](./Images/2.png)

Otra forma de describir esto:

**Es** - La verdad real sobre la postura de seguridad de una organización. (Por ejemplo, 20 personas tienen acceso al
sistema contable sensible).

**Debería ser** - La postura de seguridad percibida de una organización. (Por ejemplo, sólo 5 personas de contabilidad pueden
acceder al sistema contable sensible).

Desafiar las suposiciones es un concepto fundamental de los equipos rojos.


### Los equipos rojos en las pruebas de seguridad

La evaluación de la vulnerabilidad, las pruebas de penetración y el Red Teaming se utilizan comúnmente (aunque erróneamente)
indistintamente y caen bajo la categoría general de hacking ético. Esta clasificación puede ser
adecuada para las conversaciones de alto nivel sobre seguridad, pero hay que hacer distinciones. Seguridad
Los profesionales de la seguridad y los clientes de los servicios de seguridad seguirán desdibujando las líneas entre estos tipos de evaluación
de evaluación si no se establecen diferencias. Nos hacemos un flaco favor si definimos los términos de forma imprecisa. Esto perjudica
a la industria de la seguridad y a los propios profesionales. Esta es una razón más para nivelar las definiciones y
llegar a un entendimiento común. La incomprensión de los tipos de evaluación ha dado lugar a evaluaciones de baja calidad
de baja calidad que pretenden ser de alto nivel. Los términos deben definirse en una fase temprana del contrato para establecer
expectativas y prestar el servicio que el cliente necesita.

#### Evaluación de la vulnerabilidad

Según la Publicación Especial 800-53 del NIST (Rev. 4)[8], una evaluación de la vulnerabilidad es un
"Examen sistemático de un sistema o producto de información para determinar la adecuación de las medidas de seguridad
seguridad, identificar las deficiencias de seguridad, proporcionar datos para predecir la eficacia de las
medidas de seguridad propuestas, y confirmar la adecuación de dichas medidas después de la implementación". En
En resumen, una evaluación de la vulnerabilidad es un análisis de un sistema que se centra en encontrar vulnerabilidades y
priorizarlas por riesgo.

La verificación de las vulnerabilidades identificadas se deja a la salida de las herramientas y al mejor juicio del analista.
del analista. La validación o explotación de una vulnerabilidad no se realiza durante una evaluación de
vulnerabilidad. Cuando se comparan con los compromisos del Equipo Rojo, las evaluaciones de vulnerabilidad son como una buena
de la casa. Las mitigaciones aplicadas debido al resultado de una evaluación de vulnerabilidad son un esfuerzo de
reducción de la superficie de ataque con la intención de reducir la capacidad que tiene una amenaza para obtener una ventaja de un
defecto identificado. Un Red Teamer o amenaza asume que este tipo de evaluaciones se están realizando y
mitigado adecuadamente. Estos pasos en la mitigación tienen un impacto en el panorama de las amenazas y pueden reducir
rutas de ataque, pero no abordan directamente la amenaza. Es mejor considerar las evaluaciones de vulnerabilidad como
un esfuerzo en la reducción de la superficie de ataque.

```
Considere esto
Los equipos rojos rara vez, si es que alguna vez, ejecutan herramientas estándar de evaluación de vulnerabilidades.
Estas herramientas son ruidosas y generan más tráfico del que un equipo rojo está dispuesto a aceptar. Si una herramienta de
Si una herramienta de evaluación de la vulnerabilidad debe ser utilizada, debe haber una pregunta en cuanto al tipo de evaluación de seguridad que se
realizada, o deben ser ejecutadas con un alto enfoque desde un lugar de ataque "quemado". Las evaluaciones de vulnerabilidad son
siguen siendo un componente crítico del programa de seguridad, pero son bastante diferentes en cuanto a su alcance y objetivos de un compromiso del equipo rojo.
```

#### Prueba de Penetración

Según la Publicación Especial 800-53 (Rev. 4) CA-8 1 del NIST, las pruebas de penetración se definen como "...
un tipo de evaluación especializada realizada en sistemas de información o componentes individuales del sistema
para identificar las vulnerabilidades que podrían ser explotadas por los adversarios...". En otras palabras, las pruebas de penetración
es un ataque simulado autorizado contra un sistema diseñado para identificar y medir los riesgos
asociados a la explotación de la superficie de ataque de un objetivo. Esto puede sonar como un equipo rojo
de equipo rojo. Las diferencias son a menudo malinterpretadas, pero son fundamentales para el éxito de ambos.

Las pruebas de penetración llevan una evaluación de vulnerabilidad al siguiente nivel introduciendo la explotación en
la prueba. El objetivo de una prueba de penetración es determinar el riesgo asociado a las vulnerabilidades y
defectos. Una prueba de penetración puede parecerse mucho a una intervención del Equipo Rojo y, en muchos casos, utilizar las mismas herramientas.
casos, utiliza las mismas herramientas. Estas similitudes no deben hacer que nadie confunda los dos. Penetración
se centran en explotar las debilidades para determinar el riesgo empresarial. Es común que una prueba de penetración
explorar una amplia gama de vulnerabilidades para descubrir sus riesgos. Durante un compromiso del Equipo Rojo, las fallas
se explotarán, pero sólo en el grado necesario para alcanzar las metas u objetivos. Si una sola
vulnerabilidad permite a un Equipo Rojo avanzar, el equipo sólo la utiliza para avanzar. Los otros
veinte defectos encontrados (por el Equipo Rojo o por una evaluación de vulnerabilidad anterior) serán documentados pero
pueden permanecer sin actuar durante el compromiso del Equipo Rojo. Las pruebas de penetración, aunque más
que una evaluación de vulnerabilidad, tiene un enfoque mucho más amplio que un compromiso del Equipo Rojo.
Red Team. Al igual que una evaluación de vulnerabilidad, la mitigación realizada después de una prueba de penetración reduce la
superficie de ataque. Esta mitigación es una forma efectiva de dificultar a los atacantes, pero no
minimiza el riesgo operativo a cero. Los esfuerzos de reducción de la superficie de ataque son buenos para limitar la capacidad de una amenaza
de una amenaza, pero no miden la capacidad de una amenaza para impactar en una organización. Las pruebas de penetración
deben considerarse un esfuerzo de validación de la ruta de ataque con el objetivo de reducir la superficie de ataque.

Las pruebas de penetración se realizan a menudo para apoyar los requisitos de auditoría, como los de PCI/DSS[9] o
HIPAA[10]. El Red Teaming no suele estar motivado por el cumplimiento de la normativa, sino por el deseo de probar a fondo la capacidad de una organización para defenderse, responder a los ataques, etc.
la capacidad de una organización para defenderse, responder y reaccionar ante una amenaza.

El riesgo para las operaciones de la empresa es, sin duda, la consideración más importante a la hora de medir el riesgo general de seguridad.
de la seguridad. Las evaluaciones de seguridad que relacionan los hallazgos y las observaciones con el riesgo operativo pueden obtener el apoyo
necesario para lograr una mejora significativa. Comparemos estos tipos de evaluaciones en términos de
riesgo operativo. Un triángulo invertido puede ilustrar la relación entre el Red Teaming, las pruebas de
y las evaluaciones de vulnerabilidad en términos de riesgo organizativo u operativo. La profundidad y
La profundidad y la amplitud de cada tipo de evaluación de la seguridad, como puede verse, es bastante diferente.

![Alt Image](./Images/3.png)

Las evaluaciones de vulnerabilidad tienden a ser amplias en su cobertura pero estrechas en su alcance. Considere una evaluación de vulnerabilidad
donde el objetivo es medir todas las estaciones de trabajo en una empresa. El alcance es muy amplio
pero no muy profundo en el contexto de los riesgos de la organización. ¿Qué se puede decir sobre el riesgo para las operaciones
cuando se identifican los fallos? ¿El riesgo organizativo sólo puede entenderse a nivel de los puestos de trabajo? El
El riesgo global de una organización puede extrapolarse hasta cierto punto, pero generalmente se queda en ese
nivel de la estación de trabajo. Las evaluaciones de vulnerabilidad son buenas para reducir la superficie de ataque pero no proporcionan
mucho detalle en términos de riesgo organizativo. Este malentendido común lleva a que la evaluación de la vulnerabilidad
vulnerabilidad que se utiliza para medir mal el riesgo de seguridad.

Las pruebas de penetración llevan las evaluaciones de vulnerabilidad al siguiente nivel, explotando y probando las rutas de ataque.
de ataque. Aunque las pruebas de penetración a menudo pueden parecer y sentirse como un compromiso del equipo rojo a nivel técnico
la diferencia fundamental radica en los objetivos y la intención. El propósito de una prueba de penetración es ejecutar
un ataque contra un sistema objetivo para identificar y medir los riesgos asociados a la explotación de una
superficie de ataque del objetivo. Considere una prueba de penetración contra el límite externo de una red. A
Un probador de penetración explota una falla identificada que permite el acceso entrante a la organización objetivo.
Desde el punto de vista de las pruebas de penetración, esto fue la identificación de una deficiencia. ¿Qué significa esto
para la organización? ¿Cuál es el riesgo? Si este defecto se mitiga, ¿cómo afecta esto al riesgo de la organización?
organizacional? Los riesgos organizativos pueden medirse indirectamente como un fallo que permite a una amenaza obtener acceso remoto, pero los riesgos más graves para las operaciones deben extrapolarse a partir de este ataque.
acceso remoto, pero los riesgos más graves para las operaciones deben extrapolarse a partir de este ataque. La mitigación ayudará a
abordar las deficiencias técnicas y reducir la superficie de ataque. ¿Qué pasa con las personas y los procesos o
acciones de detección y respuesta? ¿Se detectará este tipo de ataque en el futuro, o la organización está
¿o la organización está jugando a un juego de "golpear al topo" con las vulnerabilidades individuales? Tapar los agujeros es bueno y reduce la
reducir la superficie de ataque, pero aquí es donde entra el red teaming. El Red Teaming se centra en las operaciones de seguridad
seguridad en su conjunto e incluye a las personas, los procesos y la tecnología. El Red Teaming se centra explícitamente
en objetivos relacionados con la formación de equipos azules o la medición de cómo las operaciones de seguridad pueden afectar a la capacidad de actuación de una amenaza.
de una amenaza. Los fallos técnicos son secundarios respecto a la comprensión de cómo la amenaza ha podido impactar
las operaciones de una organización o cómo las operaciones de seguridad pudieron afectar a la capacidad de una amenaza para operar.
operar.

#### Resumen de la comparación

```
| Método | Descripción | Objetivo en términos de riesgo |
|-------------------------- |-------------------------- |-------------------------- |
| Prueba de Penetración | Un ataque contra | La reducción de la superficie de ataque |
| | un sistema, red, o | | | aplicación
| | aplicación diseñada para | | | identificar y medir
| | identificar y medir | | | los riesgos asociados a
| | los riesgos asociados con | | | | la explotación de un
| | | la explotación de un | | | | objetivo.
 	| |
| | | Piensa: Ruta de ataque.
| ...validación...
| | | |
| Evaluación de la vulnerabilidad | Una evaluación utilizada para | Reducir la superficie de ataque |

| | medidas de seguridad, | | | identificar la seguridad
| Identificar las deficiencias de seguridad
| | deficiencias de seguridad, y | | |
| | confirmar las mitigaciones | | |
| | | están en marcha con el | | | | objetivo de reducir un
| | | objetivo de reducir un | | | | objetivo.

| | | Piensa: Identificación de fallos.
| | identificación | | | | | | | | | | | |
| | | |
| Compromiso del Equipo Rojo | El proceso de usar | Entrenamiento y medir |

| y procedimientos (TTPs) | las personas, procesos, |
| | para emular un mundo real | y la tecnología (seguridad |

| | formación o medir | | | la eficacia de la
| La eficacia de las personas, los procesos y la tecnología.

| | | tecnología utilizados para | | | | | | defender un entorno.
| | defender un entorno.   	| |
| | | Pensar: Medir las operaciones de seguridad...
| ...las operaciones de seguridad...
| ...como un todo...
```

### Red Teaming Organizations

El NIST ha proporcionado orientación general en forma de Marco de Ciberseguridad[11] para
mejorar la ciberseguridad de las infraestructuras críticas. Este marco proporciona una taxonomía común y
mecanismo para que las organizaciones:
1. Describir su postura actual de ciberseguridad
2. Describir su estado de ciberseguridad objetivo
3. Identificar y priorizar las oportunidades de mejora en el contexto de un
proceso continuo y repetible
4. Evaluar el progreso hacia el estado objetivo
5. Comunicar a las partes interesadas internas y externas el riesgo de ciberseguridad

Este marco presenta las normas, directrices y prácticas de la industria de manera que permite
comunicación de las actividades y resultados de ciberseguridad en toda la organización, desde el nivel ejecutivo
desde el nivel ejecutivo hasta el nivel de implementación/operaciones. El núcleo del marco consta de cinco funciones concurrentes y
funciones concurrentes y continuas: Identificar, Proteger, Detectar, Responder y Recuperar. Cuando se consideran conjuntamente, estas
funciones proporcionan una visión estratégica de alto nivel del ciclo de vida de la gestión de los riesgos de ciberseguridad de una organización.
de los riesgos de ciberseguridad de una organización. El núcleo del marco identifica categorías y subcategorías clave subyacentes para
cada función. Las empareja con referencias informativas de ejemplo, como las normas existentes,
directrices y prácticas existentes para cada subcategoría. Para más detalles, visite
https://www.nist.gov/cyberframework/cybersecurity-framework-faqs-framework-components.

En términos de Red Teaming, este documento se centra en cómo el Red Teaming puede ser utilizado por una organización
para entender su capacidad de Identificar, Proteger, Detectar, Responder y Recuperar contra una amenaza. Estas categorías de
categorías son en las que deberíamos centrarnos en el sector de la seguridad. Las capacidades de detección y respuesta son
vitales y podría decirse que son el punto de las operaciones de seguridad.

**Identificar** - Las funciones de identificación son fundamentales para el uso eficaz del Marco. El
organización ha asociado el contexto empresarial, las funciones, los activos, las personas y las tecnologías con posibles
debilidades, vulnerabilidades y amenazas para determinar los riesgos.  
**Proteger** - La función de Proteger apoya la capacidad de limitar o contener el impacto de un posible
evento de ciberseguridad. La organización está preparada y configurada para prevenir la intrusión, explotación o
manipulación de la información.  
**Detectar** - La función de Detectar permite descubrir a tiempo los eventos de ciberseguridad. La organización
lleva a cabo una supervisión e identificación fiables de las actividades o entidades no autorizadas.  
**Responder** - La función Responder apoya la capacidad de contener el impacto de un potencial
incidente de ciberseguridad. La organización realiza una identificación y un análisis precisos de las actividades detectadas
actividades detectadas que dan lugar a informes y respuestas eficaces.  
**Recuperación** - La función de recuperación apoya la recuperación oportuna de las operaciones normales para reducir el impacto
de un incidente de ciberseguridad. Las capacidades se restauran efectivamente cuando los procesos/producciones
procesos/producciones operativos se han visto perjudicados.

![Alt Image](./Images/4.png)


Este diagrama ayuda a ilustrar la cobertura del IPDRR por tipo de compromiso.

Las evaluaciones de vulnerabilidad proporcionan a una organización la medida o comprensión de la capacidad de identificar o
proteger contra una amenaza. Esto es genial pero no proporciona los medios para entender las operaciones de seguridad como
en su conjunto. Las evaluaciones de vulnerabilidad tienden a centrarse en los controles preventivos.

Como las pruebas de penetración se centran en la validación de la ruta de ataque, pueden utilizarse para medir no sólo
la identificación o la protección, sino la detección de la actividad de las amenazas y, posiblemente, un poco de respuesta. En general,
las pruebas de penetración tienen un alcance de máxima cobertura en un tiempo relativamente corto. Estas pruebas conducen a
de la protección y la detección contra la actividad de las amenazas, pero hacen poco para comprender la respuesta o la recuperación.
la respuesta o la recuperación.

El Red Teaming permite a una organización explorar completamente todos los aspectos de la actividad de las amenazas. El Red Teaming
proporciona el estímulo necesario para comprometer las operaciones de seguridad en su conjunto. El Red Teaming puede emplear
una organización para permitir que las operaciones de seguridad (Equipo Azul) utilicen sus TTPs a través de la identificación
protección, detección, respuesta y recuperación de una amenaza. El nivel de medición está conformado por
el plan de compromiso y está determinado por los objetivos.


### Puntos clave del capítulo

El Red Teaming es el proceso de utilizar Tácticas, Técnicas y Procedimientos (TTPs) para emular una amenaza del mundo real con el objetivo de entrenar y
con el objetivo de entrenar y medir la eficacia de las personas, los procesos y la tecnología utilizados para defender un entorno.
tecnología utilizados para defender un entorno.

El Red Teaming se centra en objetivos relacionados con la formación de los equipos azules o la medición de cómo las operaciones de seguridad pueden
de seguridad pueden afectar a la capacidad de actuación de una amenaza. Los fallos técnicos son secundarios a la comprensión de cómo la amenaza
de una organización o cómo las operaciones de seguridad pueden afectar a la capacidad de actuación de una amenaza.
en la capacidad de actuación de una amenaza. Las evaluaciones de vulnerabilidad y las pruebas de penetración se centran en los fallos técnicos
que dan como resultado la mitigación y la reducción de la superficie de ataque.

```
Considere lo siguiente
El Red Teaming puede utilizar técnicas de seguridad ofensivas, pero no es de naturaleza ofensiva. Podría decirse que forma parte de la comunidad
defensiva de la seguridad.
El rojo no puede existir sin el azul
```

### ``Trabajo en casa

```
1. Desarrollar un léxico de términos para mantener una base común e imparcial de entendimiento
que pueda ser compartida y referenciada entre las partes interesadas internas y externas.
2. Crear o adoptar una definición de red teaming y guardarla en el léxico.
3. Adoptar el enfoque "Es" frente a "Debería ser" al desarrollar escenarios basados en amenazas.
4. 4. Realizar el desafío de la mentalidad adversaria que figura en el apéndice para comprender mejor el punto de vista del adversario.
el punto de vista del adversario.
```

## Planificación del compromiso

![Alt Image](./Images/5.png)

Todos los compromisos deben comenzar con la Planificación del Compromiso, el primer paso en un compromiso del Equipo Rojo. No es posible
No es posible llevar a cabo una ejecución profesional y satisfactoria sin comprender plenamente los objetivos
objetivos y el alcance de la intervención, comprender los recursos necesarios para la ejecución y crear un plan sólido.
plan.


### Coste y financiación

Al igual que con cualquier esfuerzo de seguridad, el coste y la financiación influyen significativamente en la planificación, programación y ejecución de un compromiso de equipo rojo.
y la ejecución de un compromiso del Equipo Rojo. Varios factores contribuyen al coste global y al alcance de una
de una intervención. Cada elemento debe ser cuidadosamente revisado y documentado explícitamente en un contrato o
acuerdo. Independientemente del estado del equipo (proveedor de servicios interno o externo), cada factor es aplicable.


### Alcance

El alcance desempeña el papel más importante en el coste global de un encargo. Considere el alcance de una
evaluación de la vulnerabilidad. A menudo hay un beneficio considerable y la necesidad de llevar a cabo un alcance completo, una revisión en profundidad de cada nodo en un entorno. El equipo y el software empleados suelen ser
El equipo y el software empleados suelen ser parte del precio (menos los requisitos de licencia adicionales), la instalación y la configuración ya se están
y la adición de espacio de destino al contrato suele ser rentable. Este esfuerzo de alcance
es un esfuerzo sencillo y normalmente se divide en el tipo de activo que se está evaluando. El alcance
podría dividirse en estaciones de trabajo, servidores, componentes de red o cualquier categoría lógica de activos.

Ahora considere la determinación del alcance de un compromiso del Equipo Rojo. Hay diferencias significativas entre una evaluación en profundidad
evaluación en profundidad de 1.000 nodos frente a una de 14.000 nodos. Se pueden hacer suposiciones precisas sobre el entorno
de los datos obtenidos de unos pocos nodos similares; sin embargo, estos datos no
Sin embargo, estos datos no permiten necesariamente al Equipo Rojo cumplir con los objetivos del compromiso. En general, a medida que el entorno del objetivo
de seguridad (e idealmente su eficacia).
A veces, esa complejidad beneficia al entorno. Otras veces, introduce debilidades que un Equipo Rojo puede utilizar ventajosamente para obtener acceso.
El equipo rojo puede utilizarlo de forma ventajosa para obtener acceso o alcanzar objetivos basados en amenazas. En cualquier caso, el Equipo Rojo
En cualquiera de los casos, el Equipo Rojo tiene que gestionar la complejidad de las tácticas para probar y validar con precisión la estrategia global de la amenaza.
Los Equipos Rojos son conocidos por aprovechar múltiples sistemas o puntos de datos y "doblar" las configuraciones para
para satisfacer las necesidades del compromiso. Las herramientas y aplicaciones de seguridad comunes no suelen descubrir muchos
de estas fallas o caminos. Esta comprensión impulsa el desarrollo del alcance hacia un escenario en lugar de
probar cada nodo en un entorno objetivo utilizando herramientas estándar de pruebas de seguridad. El alcance debe
siempre apoyar directa y eficazmente los objetivos operativos que se miden.


### Duración

La duración puede ser un marco de tiempo determinado por el objetivo o el Equipo Rojo; sin embargo, se recomienda que la duración se establezca después del objetivo.
Sin embargo, se recomienda que la duración se establezca después de determinar los objetivos, los requisitos y el alcance del objetivo.
Un marco temporal realista puede entonces situarse en el contexto del alcance, y aumentarse o reducirse
según sea necesario. Es fundamental no utilizar el plazo para fijar el alcance. Fijar un plazo de forma arbitraria puede
La fijación arbitraria de un plazo puede repercutir negativamente en la calidad del alcance de un encargo al imponer restricciones artificiales. Aunque esto
Aunque esta es la mejor práctica, y la duración debe establecerse después de determinar los objetivos y el alcance, es útil
tener unas directrices. Para la mayoría de los encargos se puede utilizar un periodo de dos a cuatro semanas. Este es un buen
Este es un buen punto de partida, pero debe ajustarse en función del alcance real.

```
Área de enfoque
La recomendación de dos a cuatro semanas es para estimar un compromiso individual, que puede ser parte de una campaña más grande
de una campaña más amplia compuesta por varios compromisos. Al determinar la duración del alcance, deben tenerse en cuenta los objetivos.
```

### Coste de la mano de obra del personal

Al mismo tiempo que se determina el alcance y la duración, la dirección del Equipo Rojo debe estimar el
número de personal necesario para un compromiso. Estos pasos deben ser simultáneos, ya que dependen el uno del otro.
entre sí. Al dimensionar un Equipo Rojo, se debe considerar el número, tamaño y duración de los compromisos.
El compromiso más básico del Equipo Rojo consistirá en al menos dos personas. Se recomienda
Un tamaño inicial recomendado para la planificación es de cuatro personas: tres operadores y un líder. Ajuste el
número en función del tamaño, la duración y los objetivos.

¿Cómo se puede ajustar el alcance utilizando un factor de tiempo o de personal? Considere este ejemplo: un
de seis semanas con tres operadores y una red de 14.000 nodos.
nodos. Este compromiso podría ampliarse a ocho semanas reduciendo los operadores o podría reducirse a
cuatro semanas añadiendo personal. Esta elasticidad de tiempo y personal debe tenerse en cuenta al planificar
para ayudar a abordar las limitaciones financieras, de calendario y de otro tipo. Esta elasticidad tiene límites y rendimientos decrecientes.
esta elasticidad. Los ajustes podrían comprometer la capacidad de alcanzar los objetivos de compromiso. Se recomienda
Se recomienda tener siempre un mínimo de dos operadores dedicados para un compromiso.


### Coste del equipo y del software

Los equipos rojos deben mantener un conjunto de herramientas comunes listas para ser utilizadas en cualquier intervención. El conjunto de herramientas puede
puede estar compuesto por herramientas gratuitas y de pago. Este conjunto de herramientas puede personalizarse aún más para satisfacer las necesidades específicas
necesidades específicas una vez que el compromiso ha sido alcanzado (o contratado si es externo). En muchos casos, un objetivo
En muchos casos, el objetivo tiene un equipo, una herramienta o un programa informático poco conocido que requiere un dispositivo de hardware o una interfaz de software especializados.
un dispositivo de hardware especializado o una interfaz de software. Se recomienda que el objetivo proporcione
Se recomienda que el objetivo proporcione acceso a un sistema de referencia para el uso del Equipo Rojo para reducir el coste. Si esta opción no está disponible, o el
objetivo es comprender cómo obtiene el acceso el Red Team, la sobrecarga y el coste adicionales pueden
y los costes adicionales pueden incluirse en los costes generales de la intervención. La personalización de herramientas, software
La personalización de herramientas, software o hardware especializado debe identificarse en una fase temprana de la planificación del alcance para captar el impacto en el mismo.


### Coste de los viajes

Los viajes no pueden olvidarse durante la planificación. Deben asignarse fondos si la intervención se lleva a cabo en
Si la intervención se lleva a cabo en un lugar específico o en una ubicación remota, deben asignarse fondos. Estos fondos deben incluir el alojamiento, los vuelos, el transporte local
transporte local, gastos de dietas y gastos varios. En el caso de los equipos con sede en Estados Unidos, se pueden aplicar las tarifas de viaje y dietas de la GSA.
puede ser un buen punto de partida para establecer los presupuestos de viaje. Muchas organizaciones
Muchas organizaciones utilizan estas tarifas y, opcionalmente, añaden un porcentaje como beneficio e incentivo para reducir el estrés y la carga de los viajes.
de los viajes. Por ejemplo, puede ser habitual utilizar las tarifas de la GSA x 1,25. Este ha sido un método exitoso
Este ha sido un método exitoso para proporcionar a los operadores una buena tarifa para cubrir el alojamiento, las comidas y los imprevistos.


### Coste previo y posterior a la contratación

Los equipos inexpertos a menudo no asignan tiempo y fondos para las actividades previas y posteriores a la contratación (tiempo de no ejecución).
tiempo de ejecución). La mayoría de los compromisos requieren alguna forma de recopilación de información o inteligencia
(OSINT), y el reconocimiento pasivo del objetivo antes de la ejecución. También necesitan tiempo para la preparación de la infraestructura
de infraestructura y, ocasionalmente, para el desarrollo de herramientas personalizadas. Todos ellos requieren una planificación antes de la ejecución
y el análisis y la elaboración de informes después de la ejecución. No olvide tener en cuenta estos esfuerzos en el proceso de
planificación y el proceso de cálculo de costes y presupuestos.

Esta sección no cubre todos los elementos posibles necesarios para presupuestar, financiar o cotizar adecuadamente un
presupuestar, financiar o cotizar adecuadamente una intervención del Equipo Rojo. Se ha redactado para estimular la reflexión y el debate sobre los costes reales y las
y las partidas previstas para una intervención. La planificación real requiere tiempo y repetición para desarrollar un proceso
proceso.


### Frecuencia

Un compromiso del Equipo Rojo puede ser una experiencia muy estresante. Las personas pueden reaccionar de forma negativa o
a la defensiva cuando se cuestionan su carácter, sus herramientas o sus procesos. Incluso un compromiso bien gestionado
incluso un compromiso bien gestionado en el que la atribución individual se mantiene al mínimo puede suponer un enorme estrés para el personal.
Hacer esto con demasiada frecuencia puede no dar tiempo a la organización para aplicar mitigaciones, puede hacer que la
organización trate los resultados con poca consideración, o que se produzca una baja moral y pocos beneficios positivos.
Hacer pruebas con poca frecuencia puede ser tan perjudicial como hacerlas con demasiada frecuencia. Cuando las pruebas se realizan
Cuando las pruebas se realizan con poca frecuencia, la organización puede volverse complaciente y poco rigurosa en sus operaciones de seguridad. Los equipos rojos
Los compromisos de los equipos rojos se dividen normalmente en tres categorías: Único, Periódico o Continuo. La frecuencia
La frecuencia adecuada depende de la organización objetivo y de los objetivos del compromiso.

#### Individual

La realización de un compromiso de Red Team como una actividad única se realiza normalmente para las organizaciones nuevas en Red
Red Teaming o las que tienen una gran huella y recursos limitados. Esto les permite mojarse los pies
sin un compromiso significativo. Un compromiso único puede ser tan simple o complejo como sea necesario.
Las organizaciones que desean un compromiso de Red Team de una sola vez pueden no saber específicamente lo que necesitan.
Un equipo rojo eficaz entrevistará e interrogará a la dirección de la organización para determinar mejor
la necesidad y los requisitos. Si el Equipo Rojo no guía esta discusión, es probable que un compromiso
Si el Equipo Rojo no guía esta discusión, es probable que un compromiso se convierta en otra evaluación de vulnerabilidad o prueba de penetración. Los compromisos puntuales
son una buena forma de introducir a las organizaciones en el Red Teaming siempre que la planificación se gestione y
siempre que la planificación se gestione y se centre en las metas y objetivos del Red Teaming.

#### Periódico

Los compromisos periódicos, anuales o bianuales de Red Team son muy comunes. Las organizaciones maduras que
que llevan a cabo compromisos integrales de Red Team equilibran el estímulo necesario para mantener las operaciones de seguridad
seguridad y el tiempo necesario para mejorar las defensas. Cuando se realiza un compromiso anual,
tenga cuidado de no tratarlo como una auditoría de cumplimiento. Será tentador limitarse a los movimientos.
Cuando las pruebas se convierten en rutina, una organización puede no tratar los resultados con la misma seriedad que una prueba única.
Para combatir esta complacencia, los compromisos deben ser desafiantes y atractivos. Deben centrarse en
áreas graves de riesgo y no ser "una prueba más para ver si los malos pueden entrar". Escenarios enfocados,
el uso estratégico de la tarjeta blanca (que se discutirá más adelante), y la incorporación de las amenazas actuales mantendrán un compromiso fresco y proporcionarán mejores resultados.
un compromiso fresco y proporcionará mejores resultados.

#### Continuo

El Red Teaming continuo es un concepto más reciente. Piensa en esto como una emulación de amenaza persistente. Cuando una
Cuando una organización tiene un equipo rojo que ataca e interviene constantemente en su red, puede comprender
las debilidades asociadas a las amenazas avanzadas y persistentes a largo plazo. Constante no significa 24
horas al día / 365 días al año. Significa que los objetivos de un Equipo Rojo se extienden a lo largo de un tiempo. Los objetivos
podrían ser en semanas, meses o incluso años en lugar de en compromisos de una o dos semanas. Este enfoque de
Este enfoque permite a un equipo realizar acciones más realistas, intentar permanecer en la red durante un periodo más
de la red durante un período más prolongado, y posicionarse de manera que una amenaza real pueda causar daños graves a una organización.
una organización. También son capaces de emular las actividades y los plazos reales de las amenazas. En este modelo,
¿qué ocurre si el equipo no es detectado? El equipo puede utilizar los impactos operativos. Estos son los pasos
tomados para impactar a una organización para provocar una respuesta directamente. Un equipo rojo puede exponer su actividad lo suficiente
lo suficiente para provocar una reacción de las operaciones de seguridad. Los equipos rojos pueden aumentar o disminuir su actividad según
necesaria sólo para exponer lo que quieren. Pueden proporcionar a los defensores una oportunidad para aprender,
proporcionar métricas y mediciones a la dirección, y mantener el acceso para realizar futuras operaciones.
Las operaciones continuas tienen un coste de tiempo, esfuerzo y dinero y requieren más recursos que cualquier otro tipo de prueba.
otro tipo de pruebas. Las organizaciones maduras o con amenazas graves son los mejores candidatos
para las operaciones continuas.


### Notificaciones de compromiso

Cuando se planifica un compromiso del Equipo Rojo, se debe tomar una decisión sobre a quién informar. ¿Sólo algunas
¿Sólo unas pocas personas de confianza sabrán que su red está siendo atacada? ¿O la organización en su conjunto será consciente de ello?
en su conjunto? Ninguna de las dos opciones es mejor que la otra. La decisión de notificar se basa en los objetivos de
objetivos o el tipo de compromiso. En el caso de los ejercicios rojo-azul, la decisión es fácil. Todo el mundo
sabe. Cuando se realiza un compromiso del Equipo Rojo contra un objetivo vivo y activo, hay que tomar una decisión.
Esta decisión puede tener un impacto considerable en los resultados y debe tomarse cuidadosamente.

#### Compromiso de Equipo Rojo anunciado

La organización (o al menos el equipo de operaciones de seguridad) tiene conocimiento de que un compromiso está
en curso.

Esto puede afectar a un compromiso de las siguientes maneras.  
Una organización puede aumentar la seguridad, parchear los sistemas, cambiar las contraseñas o prepararse para un ataque conocido.
prepararse para un ataque conocido. Esto puede tener un impacto dramático en los resultados.  
● La planificación puede incluir a todos los miembros clave de una organización. Esto ayuda a garantizar que los activos
activos críticos están incluidos, y los objetivos del Equipo Rojo pueden establecerse en consecuencia.  
● Los temores de un Equipo Rojo rebelde pueden tratarse con antelación mediante una comunicación eficaz.
Esto suele conducir a un compromiso más profundo en el que los riesgos pueden ser explorados con
reglas de compromiso bien planificadas.

#### Participación de un equipo rojo sin previo aviso

La organización (especialmente el equipo de operaciones de seguridad) no sabe que se está llevando a cabo una intervención.
en curso.

Esto puede afectar a un compromiso de las siguientes maneras.  
Una organización actuará y responderá como lo haría en un día cualquiera. Esto proporciona resultados muy
resultados muy realistas al medir la postura real de las operaciones de seguridad.  
● El miedo a lo desconocido hace que algunas organizaciones reaccionen con la mentalidad de "el cielo se está cayendo".
mentalidad de "el cielo se está cayendo". Este miedo puede causar daños autoinfligidos no deseados si no se siguen las políticas y
procedimientos no se siguen.  
● Los objetivos y las metas pueden no estar incluidos en la planificación. Cuando sólo un pequeño número del equipo de una
Cuando sólo un pequeño número del equipo de una organización forma parte de la planificación, pueden perderse activos críticos y no incluirse en
el alcance. Este descuido puede hacer que un compromiso pierda el enfoque en áreas que pueden
exponer a la organización a un riesgo considerable.

#### ¿Cómo decidir?

Los dos consejos siguientes pueden servir para responder a la pregunta sobre la elección de una auditoría anunciada o no anunciada.  
1. Si el objetivo general es medir la eficacia de las operaciones de seguridad de una organización
seguridad de una organización, comience la planificación con un compromiso no anunciado. Incluso con las
limitaciones, los resultados serán los más precisos y realistas en términos de comprensión
el impacto de una amenaza.  
2. Si el objetivo general es medir la eficacia de una capacidad, herramienta, proceso o tecnología específica
o tecnología, comience la planificación con un compromiso anunciado. Cuando los objetivos son
Cuando los objetivos son específicos o dirigidos, incluir a los defensores puede garantizar que el alcance y las reglas estén
adecuadamente diseñadas para lograr los resultados deseados.

```
Consejo del Equipo Rojo  
Notificación anunciada vs. No anunciada

1) Si el objetivo general es medir la eficacia de las operaciones de seguridad de una organización, comience la planificación con
un compromiso no anunciado. Incluso con las limitaciones, los resultados serán los más precisos y realistas en términos de
comprender el impacto de una amenaza.  

2) Si el objetivo general es medir la eficacia de una capacidad, herramienta, proceso o tecnología específicos, comience la
planificación con un compromiso anunciado. Cuando los objetivos son específicos o dirigidos, incluir a los defensores puede garantizar que el
alcance y las reglas están adecuadamente diseñadas para lograr los resultados deseados.
```

### Roles y responsabilidades

Un Equipo Rojo eficaz está compuesto por un equipo de individuos que pueden contribuir al
éxito general. La diversidad es crucial, pero el equipo en su conjunto debe estar compuesto por los rasgos básicos del operador. A
equipo puede tener aún más éxito cuando varios miembros del equipo contribuyen en diversas áreas. En
Además del propio Equipo Rojo, la ejecución con éxito de un compromiso requiere la participación de
numerosas funciones y grupos.

#### Célula Blanca

(Normalmente se utiliza durante la ejecución de un "estilo de juego")
La Célula Blanca se encarga principalmente de hacer cumplir las reglas del combate para garantizar que ni el Equipo Rojo ni las actividades del defensor
defensores causen problemas inesperados en el entorno operativo o en el objetivo. La Célula Blanca
a menudo tiene la tarea de:
```
Servir de árbitro entre las actividades del Equipo Rojo y las respuestas del defensor durante un compromiso  
● Establecer métricas para el compromiso  
● Coordinar las actividades de ambas partes para garantizar que se alcancen los objetivos del compromiso  
● Proporcionar la información necesaria para llevar a cabo un compromiso eficiente  
Ayudar en las actividades de desconflicción entre el Equipo Rojo y los defensores  
● Calificar el compromiso (si procede)  
● Proporcionar una lista consolidada de las lecciones aprendidas obtenidas a través de la observación durante y la solicitud posterior a la acción inmediatamente después del compromiso  
```
La Célula Blanca también es responsable de correlacionar las actividades realizadas por el Equipo Rojo con las acciones
realizadas por los defensores (incluyendo tiempos, sistemas, redes, comunicaciones del equipo, etc.). Este
datos son beneficiosos tanto para los defensores como para el grupo de control a la hora de identificar deficiencias en la
seguridad del entorno y de las acciones defensivas.

Es importante tener en cuenta que la Célula Blanca es un papel de observador y correlacionador de datos, y no forma parte del
del entorno del objetivo o del equipo de intervención. La Célula Blanca debe recibir información del defensor
pero nunca entregar información al defensor. Cualquier información proporcionada al defensor debe ser
debe ser dirigida a través del Grupo de Control de Enfrentamiento o de Ejercicio.

#### Grupo de Control de Entablamiento (ECG)

El Grupo de Control del Entablamiento (o del Ejercicio) es el responsable último de todas las actividades realizadas
durante el combate. Esta responsabilidad incluye: 
```
Aprobar el cronograma, los objetivos y las directivas del compromiso  
● Aprobar las metas de los objetivos del Equipo Rojo para su inclusión en la planificación del compromiso  
● Establecer una lista negra coordinada en el tiempo para el entorno (si es necesario)  
● Proporcionar la información del entorno necesaria para construir escenarios que cumplan todos los objetivos del compromiso  
● Proporcionar gestión y dirección para la ejecución del compromiso  
● Determinar si, cuándo y qué información debe proporcionarse al defensor durante la ejecución (también conocido como inyecciones)  
● Determinar cuándo deben implementarse las acciones como parte de un impacto operacional del compromiso  
```
La mayoría de las veces, el ECG está compuesto por uno o dos altos directivos del entorno objetivo (por
ejemplo, un Director de Información o un Director de Operaciones), un miembro del departamento de
de tecnología de la información de la organización, un enlace de la Célula Blanca y un enlace del Equipo Rojo. Pueden añadirse otros
Otros pueden ser añadidos según sea necesario. Todos deben ser agentes de confianza. Algunas comunidades consolidan el GEC y la Célula Blanca
Algunas comunidades consolidan el GEC y la Célula Blanca en un único grupo con diferentes funciones individuales. Cuando esto ocurre, debe seleccionarse un Director de Control del Compromiso
Cuando esto ocurre, se debe seleccionar un Director de Control de Enfrentamiento para que interactúe con el Equipo Rojo y controle el flujo de información a los
defensores.

#### Agente de confianza (AT)

Un agente de confianza es un miembro de la organización objetivo que sabe que hay un compromiso en curso. El
El papel principal del agente de confianza es limitar el daño irreversible y el riesgo para la vida, las extremidades, la vista y el equipo.
equipo; sin embargo, se utilizan más a menudo para evitar que los defensores se autoinflijan daños inesperados.
daños inesperados. Un AT tiene un conocimiento privilegiado y detallado de las actividades del compromiso, los hitos
condiciones, y el estado del compromiso que podría sesgar o influir indebidamente en las acciones del
personal del entorno y de los defensores. Un Agente de Confianza debe proteger toda la información para que no sea proporcionada a
a cualquier parte sin la aprobación expresa del GEC. Cada compromiso debe establecer un Acuerdo de Agente de
Acuerdo de Agente de Confianza que especifique a quién se pueden entregar los datos y bajo qué proceso de aprobación.
Cada AT debe ejecutar el acuerdo antes de recibir cualquier información sobre el compromiso.

#### Observadores

Si se requieren observadores, su función es documentar las acciones y reacciones de cada célula durante la
fase de ejecución del compromiso. No tienen conocimiento del compromiso o del escenario y no proporcionan
No proporcionan información, sugerencias, asistencia, orientación, etc. a ninguna célula; sin embargo, el observador
puede informar de acciones potencialmente perjudiciales a la célula blanca para asegurarse de que se abordan.

#### Célula Roja

El término "célula roja" se ha tomado prestado del ejército. Se asocia comúnmente con un grupo que desempeña
OPFOR (fuerza opositora) durante los ejercicios de rojo contra azul. Una célula roja son los componentes que conforman la
parte ofensiva de un compromiso del Equipo Rojo. La célula roja suele estar formada por los líderes y operadores del Equipo Rojo
y operadores y se denomina comúnmente Equipo Rojo en lugar de Célula Roja.

#### Líder del Equipo Rojo

Un Equipo Rojo debe tener un líder para cada compromiso. El líder puede desempeñar el papel de oficial de acción
de acción, de líder del compromiso, de operador, de interfaz con el cliente y, a menudo, de analista. En general, el
líder del Equipo Rojo:  
```
● Proporciona dirección y orientación general al equipo  
● Proporciona información y datos de investigación para todas las leyes, reglamentos, políticas, programas y operaciones  
● Proporciona la supervisión de la planificación y ejecución operativa  
● Se coordina con cada una de las funciones dentro del compromiso del Equipo Rojo
● Planifica y gestiona el presupuesto, el personal y el equipo  
Supervisa el calendario del equipo  
● Proporciona información relacionada con los compromisos, las capacidades, la tecnología y las tendencias  
● Proporciona los requisitos de formación y desarrollo del personal  
● Realiza un análisis del presupuesto, incluyendo el equipo y los viajes  
● Identifica las direcciones de investigación y desarrollo técnico
```
Al planificar o ejecutar un compromiso, el Jefe del Equipo Rojo:  
```
● Supervisa la coordinación con todas las partes interesadas a efectos de la ejecución del compromiso  
● Supervisa las actividades de formación  
Es responsable del mantenimiento y la coordinación de la logística y de la programación del espacio, el tiempo y el equipo de la intervención.  
● Supervisa el cumplimiento de todas las leyes, reglamentos, políticas, programas y operaciones  
● Es responsable de garantizar la finalización precisa y oportuna de un informe final del compromiso  
```
#### Operador del Equipo Rojo

Los operadores del Equipo Rojo son las personas que ejecutan las acciones necesarias para que un compromiso cumpla
los objetivos. Cada operador del Equipo Rojo cumple con todas las políticas y normas del Equipo Rojo bajo la
bajo la dirección del Jefe del Equipo Rojo. En general, el operador:  
```
● Ejecuta los requisitos de compromiso según las instrucciones  
Cumple con todas las leyes, reglamentos, políticas, programas y Reglas de Intervención  
● Implementa la metodología operativa del equipo y las TTPs  
Identifica y contribuye a las deficiencias del entorno objetivo  
● Investiga y desarrolla nuevos exploits y prueba la funcionalidad de las herramientas  
● Realiza inteligencia de fuente abierta según se requiera para el compromiso  
● Identifica y evalúa acciones que revelan vulnerabilidades y capacidades del sistema  
● Asiste al líder del equipo rojo en el desarrollo del informe final del compromiso  
● Realiza apoyo de evaluación física bajo la dirección del Red Team Lead  
● Ejecuta los impactos operativos según lo aprobado por el ECG  
```

#### Célula Azul

La célula azul es el lado opuesto a la roja. Son todos los componentes que defienden una red objetivo. La célula azul
célula azul suele estar compuesta por miembros del equipo azul, defensores, personal interno y la
dirección de la organización.

![Alt Image](./Images/6.png)

Este diagrama muestra la relación y las vías de comunicación entre los diferentes grupos en un
compromiso. El líder del equipo rojo mantiene una comunicación constante con el ECG y la célula blanca. El
El jefe de equipo azul y los agentes de confianza mantienen la comunicación con la célula blanca. La línea discontinua de
los observadores representa las comunicaciones limitadas a los individuos que supervisan un compromiso.


### Reglas de Enfrentamiento (ROE)

Las reglas de intervención establecen la responsabilidad, la relación y las directrices entre el equipo rojo, el propietario de la red y el sistema.
Team, el propietario de la red, el propietario del sistema y cualquier parte interesada necesaria para la ejecución del compromiso.

Este documento contiene todas las reglas acordadas para un compromiso, debe ser un acuerdo oficial firmado por todas las partes involucradas, y se utiliza para la ejecución del compromiso.
acuerdo oficial firmado por todas las partes implicadas, se utiliza como el acuerdo formal que autoriza las
y debe ser tratado como una ley. Las ROE rigen todo el proceso de un compromiso del Equipo Rojo
y debe ser respetada durante la ejecución. La violación de las ROE puede poner en riesgo a la organización objetivo o a los
de la organización objetivo o a los operadores de la intervención. La seriedad de las ROE no debe tomarse a la ligera. Todas las partes deben
aprobar cualquier desviación de las normas establecidas en las ROE antes de la ejecución.

#### Documento de las ROE

Las ROE documentan la información del objetivo, las aprobaciones, la implementación de la amenaza, las actividades y los asuntos
necesarios para dotar de personal, coordinar y ejecutar los compromisos dentro del entorno del objetivo.

El cuerpo principal de las ROE (a menudo derivado de una plantilla permanente) proporciona información sobre:  
```
La metodología del Equipo Rojo  
● Una descripción de alto nivel de los tipos de actividades que pueden ejecutarse  
● Los tipos de hardware y software que pueden emplearse  
● Un proceso de desconflicción recomendado  
● Los niveles de amenaza disponibles (comparación)  
● Las funciones y responsabilidades de cada grupo funcional (ECG, White Cell, TA, etc.)  
● La identificación y referencias a los requisitos legales apropiados (PCI, FERPA, HIPAA, HITEC, SOX, GLBA, etc.)  
● Una exención de responsabilidad legal (requisitos de mandato federal para que el equipo rojo informe de hallazgos específicos)  
```
La información específica de cada compromiso debe documentarse en anexos a las ROE. Como mínimo,
Los anexos de las ROE deben detallar:

**El objetivo de la intervención  
```
● Nombre de la organización  
● Dirección  
● Grupos o divisiones específicas  
● Identificadores de la organización  
● Información de contacto de la alta dirección  
```

**Una lista de contactos de compromiso (nombre, función, teléfono, correo electrónico, ubicación de la oficina)**  
```
● Personal de ECG  
● Célula Blanca  
● Agentes de confianza  
● Jefe del equipo rojo  
● Jefe de equipo rojo  
```

**Objetivos de compromiso**  
```
● Condiciones  
● Nivel de amenaza  
● Objetivos de oportunidad  
● Objetivos de oportunidad  
● Medidas de éxito/fracaso  
```

**Espacio de objetivos autorizados**  
Red
```
● Los límites de la IP del evento 
● Dominios y grupos de trabajo 
● Áreas y recursos específicos fuera de los límites (por ejemplo, compartir archivos de propiedad intelectual no objetivo)  
● Máquinas, redes, equipos o aplicaciones fuera de los límites (lista negra)  
● Ventanas de mantenimiento  
```

Físico
```
● Áreas del campus  
● Edificios  
● Oficinas  
● Áreas fuera de los límites (por ejemplo, el sector de servicios de emergencia de un complejo médico)  
● Materiales no permitidos dentro del espacio objetivo (por ejemplo, documentos o equipos sensibles)  
```

**Acciones autorizadas:** Tipos de actividades aprobadas para el compromiso  
**Acciones restringidas:** Tipos de actividades restringidas durante el compromiso (si las hay)  
**Proceso de aprobación:**
El proceso para solicitar la aprobación de actividades adicionales durante la ejecución del compromiso    
● Proceso de aprobación  
● Puntos de contacto (nombre, función, teléfono, correo electrónico, ubicación de la oficina)  
● POC alternativo  

Las ROE deben ser actualizadas cuando el espacio objetivo, las acciones autorizadas, los objetivos o el alcance son
alcance. Por ejemplo, el alcance original puede limitarse a los ataques a la red informática. Si se planean
Si se planean ataques físicos, las ROE deben ser actualizadas para reflejar las actividades y controles adicionales. El
El Jefe del Equipo Rojo abordará las sugerencias o ajustes a las ROE. Cada revisión debe ser proporcionada
al iniciador. Las ROE finales deben ser firmadas por un agente de confianza de la alta dirección del entorno objetivo.
entorno.


### Gestión del riesgo

Esta sección analiza el riesgo (como resultado de las actividades del Equipo Rojo) para el entorno objetivo, NO
las vulnerabilidades o debilidades inherentes.

La gestión de riesgos es el proceso de identificar, evaluar y controlar los riesgos derivados de
de los factores de compromiso y tomar decisiones que equilibren los costes del riesgo con los beneficios del objetivo. El objetivo de
El objetivo de la gestión del riesgo no es eliminar todo el riesgo, sino eliminar el riesgo innecesario.

El proceso de planificación del compromiso debe identificar y minimizar cualquier riesgo que pueda producirse
directamente o indirectamente como resultado de las actividades del Equipo Rojo. El objetivo es implementar los esfuerzos
El objetivo es implementar los esfuerzos descritos en las ROE sin causar ningún daño irreversible al entorno objetivo. El GEC tiene
responsabilidad general de aplicar la gestión de riesgos y aceptar el riesgo para el entorno objetivo
objetivo durante el compromiso. El Jefe del Equipo Rojo tiene la responsabilidad de implementar la gestión de riesgos
y aceptar las directrices de riesgo en los objetivos del equipo durante el compromiso.
Antes y durante el evento, el Jefe del Equipo Rojo puede solicitar a la AT y al GEC que evalúen todos los riesgos
asociados a las actividades actuales del Equipo Rojo y viceversa.

La gestión de riesgos ayuda a la planificación del compromiso mediante  
```
● La conservación de los limitados recursos utilizados a lo largo de un compromiso
● Identificar los riesgos potenciales con antelación para evitar este riesgo injustificado
● Tomar una decisión informada sobre el curso de implementación de la acción (o alternativa)
● Identificar medidas de control factibles y eficaces para garantizar que un compromiso cumpla los objetivos de la evaluación sin introducir riesgos innecesarios para la seguridad y la salud del objetivo
● Proporcionar alternativas para el cumplimiento del objetivo o la meta cuando un riesgo es demasiado alto.
```

La gestión de riesgos no:  
```
● Limitar la capacidad del Equipo Rojo para operar hasta el punto de no poder cumplir los objetivos del compromiso  
● Disuelve completamente todo el riesgo (gestiona el riesgo)  
● Ordenar una decisión sobre la actividad (proporciona orientación al GEC sobre mitigaciones o decisiones alternativas)  
● Tener la autoridad para violar la ley incluso para apoyar la ejecución exitosa de un compromiso  
● Eliminar los requisitos para el ejercicio de SOP y TTP  
```
¿Qué significa esto en la ejecución práctica?

Cada compromiso debe incluir la gestión de riesgos en la planificación y ejecución. Los probadores de seguridad y los operadores de Red
Los operadores del Equipo Rojo han sido invitados a jugar en el campo de juego de otra persona. El cuidado y la consideración deben
ser manejados apropiadamente a través de la gestión de riesgos. La gestión de riesgos no significa la eliminación de los mismos.
El propósito es identificar el riesgo con antelación y desarrollar un plan para manejar situaciones en las que un riesgo preidentificado
riesgo identificado previamente o desconocido.


El proceso de gestión de riesgos:
1. Identificar los posibles problemas, conflictos o peligros (de vida, de
producción)
2. Evaluar cada uno de ellos para determinar el impacto directo en el entorno objetivo
3. Desarrollar controles diseñados para mitigar los riesgos
4. Tomar una decisión sobre los riesgos
5. Implementar los controles
6. Identificar el riesgo residual (modificar los controles hasta que el riesgo residual sea aceptable o no pueda
reducirse más)
7. Evaluar continuamente el riesgo


### Planificación de la amenaza

Un factor importante del compromiso es el tipo de amenaza y las características que debe representar el Equipo Rojo.
Esto se consigue mediante la planificación de la amenaza. El estado final de la planificación de la amenaza es la capacidad de representar la
El estado final de la planificación de la amenaza es la capacidad de representar la amenaza lo más fielmente posible y asesorar al objetivo de las implicaciones en el entorno del objetivo.
La planificación efectiva mediante la construcción de TTPs, perfiles y escenarios mejora significativamente
la capacidad del Equipo Rojo para garantizar que la intervención identifique los posibles vectores de amenaza y ayude a las operaciones defensivas a identificar las deficiencias en el entorno del objetivo.
a las operaciones defensivas en la identificación de lagunas en los procesos, procedimientos, conjuntos de herramientas y formación.

El nivel y la profundidad de la planificación de las amenazas dependen de los objetivos y son diferentes en cada intervención. En
Como mínimo, la planificación de la amenaza debe incluir el uso de las TTPs de amenaza específicamente requeridas para lograr un
objetivo y, opcionalmente, las características de los actores o grupos de amenaza específicos. Considere lo siguiente
Cuando se planifique cómo se utilizará una amenaza durante un enfrentamiento, hay que tener en cuenta lo siguiente.

```
● Panorama de la amenaza  
    ● ¿Cuáles son las características del objetivo?  
    ● ¿Qué TTPs específicos serán necesarios para operar en ese entorno?  
● Amenaza en el entorno del objetivo.  
    ● ¿Cuáles son las amenazas actuales a un entorno identificado a través de OSINT?  
    ● ¿Cuáles son las preocupaciones de amenazas actuales del cliente, problema actual o eventos anteriores?  
● Ejemplos de amenazas en el mundo real  
    ● ¿Qué amenazas actuales o anteriores son preocupantes?  
● Amenaza en el escenario o condiciones de compromiso.  
    ● ¿Cómo impactará el escenario del compromiso en el panorama de las amenazas?  
● Nivel de capacidad de amenaza que el equipo intentará emular  
    ● ¿Es importante la capacidad o el nivel de la amenaza (de simple a avanzado) en el escenario de compromiso?  
```
Un factor que los líderes de los equipos rojos deben considerar es el realismo de la amenaza. Aunque algunas organizaciones pueden
Si bien algunas organizaciones pueden decidir intencionadamente no dar rienda suelta a todas las capacidades de la amenaza (por ejemplo, debido al nivel de
aptitud del público objetivo o las limitaciones del entorno), la mayoría de los Equipos Rojos seleccionan tipos y estrategias de ataque para
simular amenazas realistas. La explotación por la explotación o una demostración de fuerza del Equipo Rojo no es
no es apropiado y no proporcionará resultados significativos. La definición de ataques basados en amenazas proporcionará un
mecanismo viable para entrenar al público objetivo y reforzar el entorno objetivo. El jefe del
El jefe del Equipo Rojo debe sopesar cuidadosamente las diferentes opciones en el contexto del compromiso. Esta lista
Esta lista constituirá la base de la estrategia de compromiso emergente.

La inteligencia sobre amenazas proporciona información para el análisis, la creación de un perfil de amenaza y la
caracterización de la amenaza. Un factor importante en la construcción de esta caracterización es la
de la amenaza, que puede ser desde el interior del objetivo, desde el exterior o desde un acceso limitado al objetivo.
tener un acceso limitado al objetivo. Esta información sobre el perfil y la caracterización se utiliza para crear
escenarios de amenaza. La inteligencia sobre amenazas también alimenta la réplica de la intención, las capacidades y las
TTPs. Estos datos pueden utilizarse para clasificar y caracterizar una amenaza.


#### Intención

La intención es el "por qué" de las operaciones de las amenazas. La intención de la amenaza puede variar mucho dependiendo del
objetivo, la sensibilidad y el valor de la información del objetivo, y los impactos deseados tanto en el objetivo
y la amenaza. La intención de una amenaza se basa en los detalles de un compromiso.

Una amenaza puede simplemente querer reunir información sobre el objetivo. Esta información suele ser algo
Esta información es normalmente algo clasificado como confidencial, de propiedad, o propiedad intelectual, y si se pierde, sería perjudicial para una
organización. Por ejemplo, los datos robados podrían proporcionarse a los competidores para que construyan y lancen a tiempo
con o por delante del objetivo.

La intención puede ser insertar código defectuoso o malicioso en el proyecto de software actual del objetivo. Este código
Este código podría causar fallos o vulnerabilidades de seguridad en el lanzamiento del software. Los escenarios de manipulación son
una excelente opción para apoyar un escenario de ataque a la cadena de suministro.

La amenaza puede querer impactar en las ventas del objetivo y posiblemente causar un fracaso empresarial al liberar
información del objetivo al público.

La intención que impacta directamente a una organización debe ser considerada durante la planificación sobre la intención que
que simplemente identifique fallos técnicos.

#### Capacidades

Las capacidades son simplemente la habilidad de una amenaza para realizar acciones dada la financiación actual, el conocimiento y la habilidad técnica, y el conocimiento del objetivo.
conocimiento técnico y habilidad, y conocimiento del objetivo. Un problema común observado en muchas industrias diferentes es
la subestimación de la capacidad de una amenaza. Es esencial tener en cuenta que la información, las herramientas, los scripts
diseños, formación, etc. disponibles para la mayoría de los profesionales de la tecnología de la información y la seguridad también están
disponibles para la amenaza.

#### TTPs

Las TTPs son el "cómo" de las operaciones de las amenazas. Los TTPs dependen de la intención y las capacidades de la amenaza.
Entender las TTPs de las amenazas es extremadamente útil tanto para el Equipo Rojo como para el Azul, ya que el uso y
comprensión de las TTP es una de las formas más eficaces de clasificar y caracterizar las amenazas por
acciones.

Considera estas preguntas cuando planifiques los TTP's de las amenazas  
(No olvides considerar la capacidad del equipo rojo para aplicarlas)  
```
¿Cuál es el método preferido de la amenaza para obtener el acceso inicial? ¿Malas configuraciones de la web? ¿Vulnerabilidades conocidas? ¿Phishing? 
● ¿Existen tendencias en los Indicadores de Compromiso (IOC)? Cosas como ubicaciones de archivos, nombres de archivos, llamadas al sistema, tráfico anómalo, etc.    
● ¿Cómo realiza la amenaza las operaciones y el mantenimiento contra un objetivo? ¿Residencia en la memoria? ¿Binarios? ¿Python? ¿WMI? ¿PowerShell? ¿VBS?  
● ¿Cómo funciona el Mando y Control (C2)? Utilizando qué protocolos?  
● ¿Se establece la persistencia? Cuáles son los métodos preferidos de la amenaza?  
● ¿Tiene la amenaza un motivo e intención estándar o común?  
```

El análisis del Equipo Rojo sobre la intención, las capacidades y las TTP de una amenaza proporciona la información necesaria
para crear el perfil de la amenaza. Este perfil permite la caracterización de la amenaza utilizada para las revisiones específicas,
evaluaciones, formación y ejercicios.


### Perfil de la amenaza

La planificación es vital para emular una amenaza o sus TTPs. Sin un plan, modelar un actor sofisticado puede
puede resultar extremadamente difícil, lento y costoso. Con demasiada frecuencia, los equipos rojos intentan emular a un
muy avanzado, como el "grupo APT X" o el "estado-nación" con poco o ningún tiempo o presupuesto.
Los actores sofisticados tienen tiempo, dinero y recursos para construir y desarrollar herramientas, explotaciones o técnicas personalizadas.
técnicas personalizadas. Esto puede parecer obvio, pero es importante recordar que un Equipo Rojo
encargado de emular a un actor específico no es ese actor. El equipo puede no tener el tiempo o el presupuesto
necesario para emular una amenaza a la perfección. Sin embargo, se puede emular una amenaza lo suficiente para mantenerse dentro de un
presupuesto razonable, así como la cantidad de tiempo y esfuerzo necesarios para modelar los componentes centrales de una amenaza.
de una amenaza.

El Equipo Rojo debe ayudar al personal a entender cómo una amenaza específica afecta a su
organización. Para facilitar esta práctica, se utiliza un perfil de amenaza para establecer las reglas sobre cómo actuará y operará un Equipo Rojo.
El Equipo Rojo debe ayudar al personal a entender cómo una amenaza específica afecta a su organización. Estas reglas sirven como hoja de ruta para un Equipo Rojo al guiar cómo y qué
tipo de acciones deben realizarse. Incluso durante una intervención en profundidad del Equipo Rojo, debe crearse un perfil de amenaza
para describir la amenaza y sus TTPs.

Hemos hablado de las TTPs, pero hasta este momento, no hemos proporcionado un medio para utilizarlas para apoyar un
compromiso. Empecemos por explicar las TTP a través del marco ATT&CK de MITRE. MITRE's
Adversarial Tactics, Techniques, and Common Knowledge (ATT&CK™) es una base de conocimiento curada
de conocimientos y un modelo de comportamiento de las ciberamenazas, que refleja las distintas fases del ciclo de vida de una amenaza y las
plataformas a las que se sabe que se dirigen. ATT&CK es útil para comprender el riesgo de seguridad frente al comportamiento conocido de las
comportamiento conocido de las amenazas, para planificar mejoras de seguridad y para verificar que las defensas funcionan como se espera.
El ATT&CK se divide en Tácticas, Técnicas y Procedimientos. Las tácticas son los objetivos tácticos que una amenaza puede
utilizar durante una operación. Las técnicas describen las acciones que las amenazas realizan para alcanzar sus objetivos.
Los procedimientos son los pasos técnicos necesarios para realizar una acción. Este marco proporciona una
clasificación de todas las acciones de las amenazas, independientemente de las vulnerabilidades subyacentes.

Los equipos rojos pueden emular TTPs realistas a través de la investigación y la experiencia, pero gran parte de esta información
ha sido recopilada en ATT&CK. El ATT&CK puede considerarse como un menú de TTPs. Los equipos rojos pueden utilizar
pueden utilizarlo para asegurarse de que tienen un perfil de amenaza válido con un conjunto completo de TTPs de amenaza, y los equipos azules
pueden usar esto para construir una tarjeta de puntuación de lo bien que pueden defenderse contra las diversas TTPs.

![Alt Image](./Images/7.png)

#### Tácticas de MITRE ATT&CK

**Acceso inicial  
```
La táctica de acceso inicial representa los vectores que los adversarios utilizan para obtener un punto de apoyo inicial dentro de una red.
```

**Ejecución  
```
La táctica de ejecución representa las técnicas que dan lugar a la ejecución de código controlado por la amenaza en un sistema local o remoto.
sistema local o remoto. Esta táctica se utiliza a menudo junto con el acceso inicial como medio para ejecutar
código una vez obtenido el acceso, y el movimiento lateral para ampliar el acceso a sistemas remotos en una red.
```

**Persistencia  
```
La persistencia es cualquier acceso, acción o cambio de configuración en un sistema que da a una amenaza una presencia persistente en ese sistema.
presencia persistente en ese sistema. Los adversarios a menudo necesitan mantener el acceso a los sistemas a través de
interrupciones tales como reinicios del sistema, pérdida de credenciales u otros fallos que requerirían una herramienta de acceso remoto para reiniciar o una herramienta de acceso alternativo.
herramienta de acceso remoto para reiniciar o una puerta trasera alternativa para que vuelvan a tener acceso.
```

**Escalada de privilegios  
```
La escalada de privilegios es el resultado de acciones que permiten a una amenaza obtener un nivel superior de permisos
en un sistema o red. Ciertas herramientas o acciones requieren un nivel de privilegio más alto para funcionar y son
probablemente necesarias en muchos puntos de una operación. Los adversarios pueden entrar en un sistema con
acceso sin privilegios y deben aprovechar una debilidad del sistema para obtener privilegios de administrador local o de dominio o de nivel de sistema/raíz.
local o de dominio o privilegios de nivel SYSTEM/root. Una cuenta de usuario con acceso de tipo administrador puede
también puede ser utilizada. Las cuentas de usuario con permisos para acceder a sistemas específicos (o realizar funciones específicas
funciones necesarias para que los adversarios logren su objetivo) también pueden considerarse una escalada
de privilegios.
```

**Evasión de la defensa**  
```
La evasión de la defensa consiste en técnicas que una amenaza puede utilizar para evadir la detección o evitar otras defensas.
A veces estas acciones son las mismas o variaciones de técnicas en otras categorías que tienen el
beneficio de subvertir una defensa o mitigación particular. La evasión de defensas puede considerarse un
conjunto de atributos que la amenaza aplica a todas las demás fases de la operación.
```

**Acceso a credenciales  
```
El acceso a credenciales representa las técnicas que resultan en el acceso o el control de credenciales de sistemas, dominios o servicios que se utilizan en un entorno empresarial.
credenciales de servicio que se utilizan en un entorno empresarial. Los adversarios probablemente intentarán
obtener credenciales legítimas de usuarios o cuentas de administrador (administrador del sistema local o
usuarios de dominio con acceso de administrador) para utilizarlas dentro de la red. Esto permite a la amenaza asumir
la identidad de la cuenta, con todos los permisos de esa cuenta en el sistema y la red, y
hace que sea más difícil para los defensores detectar la amenaza. Con suficiente acceso dentro de una red, una amenaza puede
crear cuentas para su posterior uso dentro del entorno.
```

**Descubrimiento  
```
El descubrimiento consiste en técnicas que permiten a la amenaza obtener conocimientos sobre el sistema y la red interna.
red interna. Cuando los adversarios obtienen acceso a un nuevo sistema, deben orientarse sobre lo que
ahora tienen el control y qué beneficios les da operar desde ese sistema a su objetivo actual o
objetivos generales durante la intrusión. El sistema operativo proporciona muchas herramientas nativas que ayudan en esta tarea
fase de recopilación de información posterior al compromiso.
```

**Movimiento lateral  
```
El movimiento lateral consiste en técnicas que permiten a una amenaza acceder y controlar sistemas remotos en
una red y podría, pero no necesariamente, incluir la ejecución de herramientas en sistemas remotos. Las técnicas de movimiento lateral
técnicas de movimiento lateral podrían permitir a una amenaza recopilar información de un sistema sin necesidad de
herramientas adicionales, como una herramienta de acceso remoto.
```

**Recogida**  
```
La recolección consiste en técnicas utilizadas para identificar y reunir información, como archivos sensibles, de
una red objetivo antes de la exfiltración. Esta categoría también cubre las ubicaciones en un sistema o red
donde la amenaza puede buscar información para exfiltrar.
```

**Exfiltración  
```
La exfiltración se refiere a las técnicas y atributos que resultan o ayudan a la amenaza a eliminar archivos e
información de una red objetivo. Esta categoría también cubre las ubicaciones en un sistema o red donde
la amenaza puede buscar información para exfiltrar.
```

**Mando y control  
```
La táctica de mando y control representa cómo los adversarios se comunican con los sistemas bajo su
bajo su control dentro de una red objetivo. Hay muchas formas en las que una amenaza puede establecer el mando y el control,
con varios niveles de cobertura, dependiendo de la configuración del sistema y la topología de la red. Debido a
Debido al amplio grado de variación de que dispone la amenaza a nivel de red, sólo se utilizaron los factores más comunes
para describir las diferencias de mando y control. Sigue habiendo una gran cantidad de
técnicas específicas dentro de los métodos documentados, en gran parte debido a lo fácil que es definir nuevos
protocolos y utilizar protocolos y servicios de red existentes y legítimos para la comunicación.
```


### Creación de un perfil de amenaza mediante la descomposición de una amenaza

Los perfiles de amenazas se pueden construir descomponiendo las amenazas existentes en componentes básicos y luego recomponiéndolos
en perfiles que un Equipo Rojo puede utilizar para describir y ejecutar una intervención del Equipo Rojo.


El reto de la gestión
```
Cuando se pide a un Equipo Rojo que realice una emulación de amenaza de un actor específico, 
los límites del presupuesto, el tiempo y el esfuerzo pueden ser fácilmente llevados al límite.  
Se requiere un fuerte liderazgo del Equipo Rojo para salvar la brecha de realismo y efectividad al emular una amenaza.
Desglosar una amenaza en sus componentes y elegir los elementos que mejor ejercen los objetivos del compromiso
proporciona al liderazgo una hoja de ruta sobre cómo se representará la amenaza con precisión. De este modo, una amenaza puede ser
emular una amenaza dentro de un entorno con presupuesto, tiempo y recursos limitados.
```
La creación de un perfil de amenaza es una buena manera de establecer las reglas sobre cómo actuará y operará un Equipo Rojo.
actuará. Estas actúan como una hoja de ruta para un Equipo Rojo al proporcionar orientación sobre cómo y qué tipo de
acciones deben realizarse. Ayudan a todas las partes (Roja y Azul) a asegurarse de que el Equipo Rojo está emulando
la amenaza correcta. Recuerde que un compromiso del Equipo Rojo no es un festival de hackeo. En muchos casos, un Equipo Rojo
En muchos casos, un Equipo Rojo ayuda al personal a entender cómo una amenaza específica afecta a una organización. Incluso durante un
Incluso durante un compromiso de Equipo Rojo en profundidad y a gran escala, se debe crear un perfil de amenaza. Ayuda a describir la
amenaza y sus TTPs. Este material es ideal para establecer el escenario, enhebrar la historia de una amenaza, y puede
mejorar enormemente el informe final.

#### Ejemplo de perfil de amenaza (simplificado)

```
| Categoría Descripción
|----------------- |---------------------------------------------------------------- |
| Descripción: Amenaza general de nivel medio que utiliza herramientas y técnicas ofensivas comunes.
| | herramientas y técnicas ofensivas comunes.                         	

| Objetivo e intención | Existir en la red para enumerar |
| | sistemas e información con el fin de | | | | mantener el Mando y Control.
| | mantener el mando y el control para | | | apoyar futuros ataques.
| | apoyar futuros ataques.                                        	
| | |
| IOCs clave | Cobalt Strike HTTPS beacon on TCP | |
| | 443, Payload:                                                  	|
| c:Datos del programa - Microsoft - Explore.exe.
| ...y la fecha..: 13/7/2009 10:04 PM, MD5: ...
| a7705501c5e216b56cf49dcf540184d0
| | |
| C2 Overview HTTPS en el puerto 443 Cobalt Strike
| | Beacon con un tiempo de devolución de llamada de cinco minutos.                       	
| | Llamar directamente a los dominios de propiedad de la amenaza | |
| | dominios propiedad de la amenaza. TTPs (Enumeración, Entrega, Movimiento
| Movimiento lateral, escalada de privilegios, etc.
| | | etc.) Modelo de Brecha asumido, sin entrega inicial | | | | | a través de explotación.
| | Entrega a través de explotación. Explotación POST a través de comandos Cobalt Strike.
| | | comandos. Enumeración y movimiento lateral
| Enumeración y movimiento lateral a través de Cobalt Strike y comandos nativos de Windows.
| | comandos de Windows. Escalada de privilegios
| | escalada limitada y determinada POST-explotación | | |.
| | |
| Explotación | Modelo de violación asumido, sin explotación.                         	
| | |
| Persistencia: Persistencia a nivel de usuario utilizando la regla de Microsoft Outlook.
| | Regla de Outlook activada por un correo electrónico específico.                      	|
```
Lo anterior es un perfil de ejemplo simplificado de un compromiso real de Red Team. Esta intervención
parte de una serie de evaluaciones diseñadas para probar la capacidad del Equipo Azul de detectar y
detectar y perfilar una amenaza. Requiere el uso de TTPs definidos y específicos. Este es el corazón de la emulación
emulación de amenazas. La definición del perfil permitió a todas las partes estar en la misma página. Al final de la
evaluación, el perfil se compartió con los miembros del Equipo Azul para ayudar a descubrir cualquier cosa que
que pudiera haberse pasado por alto. Esto proporcionó a los defensores la información necesaria para identificar cualquier laguna en
sus TTPs, lo que les ayudó en gran medida a mejorar.

El proceso de descomposición de una amenaza implica
1. Investigación de la amenaza existente
2. Desglosar los elementos clave del perfil de una amenaza. (descripción, objetivo e intención, IOCs
IOCs, visión general del C2, explotación y persistencia)
3. Recomponer la amenaza en forma de perfil utilizando la información aprendida y llenando
(MITRE ATT&CK es una gran fuente para ayudar a llenar estas lagunas)

#### Uso del perfil de la amenaza

Los perfiles de amenaza suelen apoyar la historia de compromiso y se utilizan para describir los aspectos técnicos
de un único canal C2. Se utiliza un único perfil de amenaza para cada canal C2.

![Alt Image](./Images/8.png)

Al final de este capítulo, tendrá la oportunidad de trabajar en un ejercicio de perfil de amenaza.
Vamos a examinar un ejemplo de un ataque real para ilustrar el concepto de un perfil de amenaza.


### Un repaso a la técnica de un blackhat

Este ataque del mundo real proporcionará el contexto y la comprensión de cómo puede ocurrir un ataque. A medida que
Mientras lees el resumen, piensa en cómo podrías usar esto en la planificación y el alcance de un compromiso del equipo rojo.
de un equipo rojo.

#### Cómo hackearon a HackingTeam

Phineas Fisher, también conocido como Hack Back, reclama la responsabilidad del ataque a Hacking Team y la publicación de documentos.
documentos. Los documentos fueron publicados en WikiLeaks el 8 de julio de 2015. En abril de 2016, Phineas
Fisher publicó un informe en el que explicaba cómo se llevó a cabo el ataque de Hacking Team. Primero fue
escrito en español y posteriormente traducido al inglés.

![Alt Image](./Images/9.png)

Hacking Team, una empresa italiana, es conocida por vender software de intrusión y vigilancia a
gobiernos, agencias policiales y corporaciones. No nos centraremos en si usted está de acuerdo
con sus prácticas o no. Lo que es interesante aquí es la oportunidad de revisar un sombrero negro de
El oficio de un sombrero negro. ¿Por qué? Un equipo rojo puede necesitar defender su posición sobre cómo y por qué actuó de una
determinada manera. Es habitual que las organizaciones objetivo afirmen que determinadas técnicas no son reales o que
una amenaza "no haría eso". Este artículo es una gran referencia para usar en la emulación de amenazas. Las TTPs
Las TTPs descritas no sólo son útiles para llevar a cabo un compromiso, sino que pueden ayudar a confirmar que las acciones de un Equipo Rojo
de un Equipo Rojo son fieles a la amenaza. Los enfrentamientos fieles a la amenaza que imitan de cerca una amenaza realista, son muy
muy creíble y una gran manera de demostrar la actividad práctica de los adversarios.

Para obtener información más detallada sobre este ataque, lea lo siguiente:  
```
1. Hack Back!, [http://pastebin.com/raw/0SNSvyjJ.](http://pastebin.com/raw/0SNSvyjJ.)
2. Hacking Team, https://wikileaks.org/hackingteam/emails/.
3. Hacking Team, https://en.wikipedia.org/wiki/Hacking_Team.
4. ¡Hack Back!, http://pastebin.com/raw/GPSHF04A.
5. Traducción completa al inglés del relato de Phineas Fisher sobre cómo derribó a HackingTeam,
https://www.reddit.com/r/netsec/comments/4f3e6p/full_english_translation_of_phineas_fishers/d25qbci/.
6. https://www.vice.com/en_us/article/3k9zzk/hacking-team-hacker-phineas-fisher-has-
HackingTeam,
```
#### Cómo se produjo el hackeo[12]

![Alt Image](./Images/10.png)

```
Diagrama de ataque del equipo de hackers destacando los principales pasos
```
Fisher comenzó por analizar el objetivo. Fisher reconoció que el spear-phishing era arriesgado. "No quería
intentar hacer spear phishing a Hacking Team, ya que todo su negocio es ayudar a los gobiernos a hacer spear phishing
a sus oponentes, por lo que es mucho más probable que reconozcan e investiguen un intento de spear phishing.
Los primeros análisis mostraron que la red de Hacking Team parecía estar reforzada y tener una
pequeña superficie de ataque. El análisis inicial reveló una versión actualizada de Joomla, un servidor de correo, un par de
un par de routers, un dispositivo VPN y un filtro de spam. Conseguir el acceso inicial no fue sencillo.
Atacar a Joomla! con un exploit o un día cero, o atacar un dispositivo integrado con una ruta aún por determinar parecía la mejor opción para el acceso inicial.
aún por determinar, parecía la mejor opción para el acceso inicial. Tras unas semanas de desarrollo, se creó un
se creó un exitoso exploit de día cero para un dispositivo incrustado sin nombre. Este día cero proporcionaba
Este día cero proporcionó acceso a la raíz del dispositivo y se utilizó como punto de entrada inicial. La enumeración interna se realizó
después de este acceso inicial. La enumeración reveló una instancia de MongoDB que no requería
autenticación. Esta base de datos proporcionaba acceso a una grabación de audio que formaba parte de una aplicación de espionaje de audio.
de audio. Estas grabaciones eran interesantes pero no perjudiciales. Fisher quería dañar a esta
empresa y exponerla por estar involucrada en algo más grave que la venta de software de espionaje.
Una exploración más profunda llevó a la identificación de esta información perjudicial. Los datos significativos fueron
encontraron en un servidor iSCSI no seguro que contenía archivos de copia de seguridad de VMware .vmdk y otra información beneficiosa.
información beneficiosa. Finalmente, se volcaron los hashes de las contraseñas de nivel administrativo de las copias de seguridad. Muchos
de las contraseñas administrativas fueron descifradas con éxito. Estas contraseñas permitían el acceso
a otros sistemas, incluyendo un servidor de correo electrónico. PowerShell fue utilizado para acceder y descargar los correos electrónicos actuales.
correos electrónicos. Se descargaron más de un millón de correos electrónicos.

En total, Phineas Fisher estuvo en la red del Hacking Team durante unas seis semanas y pasó unas 100
horas moviendo y robando datos. El ataque tenía una motivación principalmente política.

Este ejemplo es casi idéntico al de un compromiso del Equipo Rojo.
Un actor inteligente analizó un objetivo para determinar el mejor camino a seguir, elaboró un ataque personalizado,
elevó los privilegios, identificó la información y robó datos sensibles.

Referencias adicionales:
1. Cómo fue hackeado Hacking Team, [http://arstechnica.com/security/2016/04/how-](http://arstechnica.com/security/2016/04/how-)
hacking-team-got-hacked-phineas-phisher/.
2. El vigilante que hackeó a Hacking Team explica cómo lo hizo,
[http://motherboard.vice.com/read/the-vigilante-who-hacked-hacking-team-](http://motherboard.vice.com/read/the-vigilante-who-hacked-hacking-team-)
explains-how-he-did-it.

Analizar las TTPs descritas en el ataque de Hacking Team es una buena manera de entender cómo una amenaza real ataca un objetivo.
amenaza real ataca a un objetivo. El análisis puede utilizarse para validar los planes de TTPs o para aprender nuevas técnicas que
pueden aplicarse a futuros compromisos. Aunque se trataba de un ataque ilegal contra una empresa, proporcionó
de una empresa, proporcionó información útil sobre la forma de pensar y actuar de una amenaza.

![Alt Image](./Images/11.png)

Se puede desarrollar un perfil de amenaza simple para proporcionar una descripción general de la amenaza utilizando el ataque de HackingTeam.

![Alt Image](./Images/12.png)

**Preguntas a tener en cuenta sobre el alcance del Red Team.**

```
1) ¿Podría su Red Team realizar estas acciones?  
Si no es así, considere la capacidad de su equipo para emular estas acciones y posiblemente mejorarlas con
formación o desarrollo interno.  

2) ¿Tiene acceso a los días cero? Si no es así, ¿cómo podría emular este tipo de ataque?  
Muchos equipos no tienen días cero ni tiempo para desarrollarlos. Considere la posibilidad de utilizar escenarios
de la tarjeta blanca para emular este tipo de ataques.  

3) Este ataque ha necesitado seis semanas, más de 100 horas y una sola persona para completarlo. Esta es una gran métrica para la duración del alcance. ¿Podría su equipo hacer lo mismo?
¿Tiene tu equipo las habilidades, conocimientos, capacidades, herramientas, TTPs, etc. necesarios para realizarlo
en el mismo plazo? Considere la posibilidad de ajustar el calendario y la asignación de horas para adaptarse a las capacidades de su equipo.  

4) ¿Accedería a un encargo con el mismo personal y los mismos parámetros de tiempo?  

Los equipos no deben actuar solos. No importa el problema que tenga un equipo con el personal o el presupuesto,
un encargo debería tener al menos el doble de personal. En cuanto al tiempo, seis semanas pueden ser más
de lo posible. Si es así, considere lo que está dentro o fuera del alcance. Considere la posibilidad de utilizar el modelo de incumplimiento asumido
para ayudar a utilizar los recursos de forma eficiente.  
```

### Perspectiva de la amenaza

Como se ha mencionado brevemente antes, la perspectiva de la amenaza es el punto de vista inicial de la misma. Esta
perspectiva se utiliza para construir y dar forma a un perfil o escenario de amenaza. La perspectiva de una amenaza puede ser la de
de una persona ajena, cercana o interna.

```
|---------------------------------------------------------------------------------------|
| Outsider |
|---------------------------------------------------------------------------------------|
| Una entidad que no tiene | Un ejemplo sería un |
| acceso legítimo a un empleado específico | de la competencia que |
| software, sistemas, y | no tendría autorización |
| redes. Un outsider es | el acceso físico o digital a |
| cualquier persona ajena a | cualquier sistema, red, |
| organización.                 	| software, o hardware.                     	|
| | |
|---------------------------------------------------------------------------------------|
| Nearsider |
|---------------------------------------------------------------------------------------|
| Una entidad que no tiene | Un ejemplo sería |
| acceso legítimo a personal específico | de conserjería. Ellos |
| software, sistemas, y | no es probable que tengan autorización |
| redes pero pueden tener | acceso digital a cualquier |
| acceso físico a los edificios | sistemas o redes, pero |
| y equipos o acceso a | | pueden tener acceso físico a |
| sistemas que se integran con | edificios, comunicación |
| activos de destino | instalaciones, sistemas, |
| | redes, etc.                             	
| | |
|---------------------------------------------------------------------------------------|
| Insider |
|---------------------------------------------------------------------------------------|
| Una entidad que tiene | un acceso legítimo | Un ejemplo de
| acceso a un software específico, | insider es un sistema | falso
| sistemas y redes y | administrador que ha |
| tiene acceso físico a | autorizados, privilegiados |
| edificios y equipos | acceso y voluntariamente |
| | elimina información de | |
| | activos de destino o modifica | | | | activos de destino para causar
| | activos de destino para causar un fallo | | |
| |-----------------------------------------------|
| Un ejemplo de información privilegiada no maliciosa es un empleado...
| | empleado del personal de ventas | | | que tiene acceso autorizado
| que tiene acceso autorizado a los sistemas...
| | a los sistemas, redes, | | software y hardware.
| | software y hardware | | | necesarios para realizar las ventas.
| ...necesarios para realizar las ventas.                 	|
| El individuo puede ser un objetivo
| ...sin saberlo, durante el acceso inicial...
| | el acceso inicial | |
|---------------------------------------------------------------------------------------|
```
Hay varios métodos utilizados para obtener acceso a un sistema objetivo. El acceso inicial se debate muy a menudo
durante la planificación del Equipo Rojo. El uso de un diagrama como el siguiente durante la planificación puede ayudar a decidir un
punto de partida basado en los objetivos. Cada punto representa un posible punto de partida. El tipo de acceso necesario
en cada punto es diferente. Inclúyalo en el plan del Equipo Rojo. El proceso de decidir la perspectiva de la amenaza
amenaza es fundamental. El escenario y los objetivos de la intervención impulsan esta decisión. Por ejemplo, los
Por ejemplo, los objetivos de un compromiso incluyen la medición de la capacidad de las operaciones de seguridad para identificar y responder a
una amenaza que se mueve a través de la red de la empresa. El uso eficaz de los recursos sería comenzar el
El uso eficaz de los recursos sería comenzar el compromiso en algún lugar dentro de esta red. Obligar a un equipo a establecer el acceso desde fuera de la
de la red podría desperdiciar el limitado tiempo de la intervención en pasos que no apoyan directamente los objetivos de la intervención.
objetivos.

![Alt Image](./Images/13.png)

Cómo utilizar este diagrama en la planificación
```
Este diagrama puede utilizarse para ayudar a planificar puntos de partida basados en la perspectiva de la amenaza. No empieces con la
No comience con la suposición de que todos los compromisos deben comenzar desde el exterior. Discuta los objetivos del compromiso junto con
el escenario deseado. Proponga algunos puntos en el diagrama que mejor ilustren el escenario. Discuta cómo este punto
representa el escenario del compromiso. Utilice el punto que mejor conduzca a la consecución de los objetivos del compromiso.
```

### Escenario de amenaza

Un aspecto fundamental del Red Teaming son los escenarios de amenaza. Los escenarios proporcionan una visión de cómo una solución defensiva
solución defensiva se comportará y ajustará a los procesos, procedimientos, políticas, actividades, personal
personal, organizaciones, entorno, amenazas, limitaciones, suposiciones y apoyo relacionados con la misión de seguridad.
de seguridad. Los escenarios generalmente describen el papel de la amenaza, cómo interactuará con los sistemas y
redes dentro del entorno objetivo, y suscita la verdad del mundo real sobre cómo se emplean las prácticas internas esenciales.
prácticas internas esenciales. En resumen, responde a cómo las operaciones de seguridad del objetivo realizarían dinámicamente
realizarían una acción para obtener resultados, productos o demostrar su capacidad.

Un compromiso del Equipo Rojo impulsado por un escenario específico reduce el enfoque a un área particular. Este
permite explorar un concepto a un nivel más profundo. Los escenarios permiten emular una amenaza específica
y exponerla a una organización objetivo. Un enfoque basado en escenarios puede ofrecer un valor adicional sobre
pruebas de penetración estándar o evaluaciones de vulnerabilidad. Las observaciones y la comprensión de cómo
una amenaza específica puede impactar en una organización proporcionan el conocimiento necesario para asignar eficientemente el
tiempo, dinero y recursos limitados de una organización para defender mejor sus activos.

Para simplificar, los equipos rojos exploran la "historia de la amenaza". Un escenario proporciona el guión de esa historia y
impulsa la forma en que un Equipo Rojo emula una amenaza. Un Equipo Rojo utiliza el argumento para dar forma a sus acciones y
desarrollar sus TTPs. Todos estos aspectos combinados crean un escenario de amenaza completo.

¿Cómo se utiliza esto en la práctica? Tal vez un objetivo se entere de un nuevo tipo de malware a través de un
de inteligencia de amenazas. El malware está atacando activamente las aplicaciones móviles de otras organizaciones similares.
organizaciones similares. La organización puede utilizar un equipo rojo para diseñar y emular un escenario específico utilizando
los TTPs del malware. Utilizando los informes de inteligencia sobre amenazas o los informes de análisis de malware, un Equipo Rojo
puede desarrollar código personalizado o simulaciones que reflejen las acciones del malware. Los escenarios permiten a la
institución realizar una evaluación de Red Team basada en el escenario para medir la capacidad de sus sistemas para resistir un ataque del nuevo malware.
sus sistemas ante un ataque del nuevo malware y, potencialmente, cómo se comportarían ante acciones similares de un malware desconocido.
acciones similares de un malware desconocido.

El diseño de escenarios puede ser un reto. Es habitual seleccionar un modelo de escenario que no permitirá a un
Es común seleccionar un modelo de escenario que no permita al Equipo Rojo alcanzar con éxito sus objetivos en los límites de tiempo de un compromiso. Recuerde que los Red
Recuerde que los equipos rojos no encuentran fallos o vulnerabilidades como en una prueba de penetración, sino que estimulan y realizan
impactos contra una organización para medir las operaciones de seguridad en su conjunto.


### Emulación de amenazas

La emulación de amenazas es el proceso de imitar los TTPs de una amenaza específica. Un Equipo Rojo realiza
emulación de amenazas actuando como una amenaza representativa. Se pueden emular amenazas de cualquier tipo. Esto puede
incluir:  
Ataques de día cero o personalizados  
Desde el script kiddie hasta la amenaza avanzada  
Emulación de herramientas o técnicas de amenazas específicas (botnets, DDOS, ransomware, malware específico, APT, etc.)  

Las evaluaciones basadas en escenarios suelen estar impulsadas por la emulación de algún nivel de amenaza. Puede tratarse de
ser una amenaza específica, como el troyano Havex utilizado por Energetic Bear / Crouching Yeti / Dragonfly, o
una amenaza general, como una simple red de bots de mando y control. Independientemente del escenario, las TTPs
que se describen conducen a las reglas que un Equipo Rojo debe seguir para llevar a cabo un compromiso. Cuando se diseña un escenario de emulación de amenaza
Cuando se diseña un escenario de emulación de amenaza, deben definirse los componentes clave de la misma. Aunque puede ser difícil
emular una amenaza específica en detalle, esto no significa que la amenaza no pueda ser emulada, o que no haya
que no haya valor en intentarlo. Un Equipo Rojo debe centrarse en seguir los componentes clave de una amenaza y utilizar
sus propios TTPs para rellenar los huecos. Un Equipo Rojo no es el diseñador o autor original de una amenaza, pero es un grupo altamente cualificado y capaz que puede
un grupo altamente cualificado y capaz que puede (y debe) reforzar las TTPs de una amenaza emulada con su
con su propia Tradecraft y procesos desarrollados. De este modo, el Equipo Rojo puede modelar un actor de la amenaza de manera
que apoye los objetivos de un escenario basado en la amenaza.

El mayor reto en la emulación de amenazas es ejecutar hasta un nivel en el que un analista crea que la amenaza
es real. Los enfoques pueden incluir el uso de malware malo conocido, el desarrollo de malware personalizado que
que modele una amenaza, el uso de herramientas que generen los Indicadores de Compromiso (IOC) de una amenaza conocida, o
simplemente utilizar herramientas y comandos nativos del sistema y de la red. Una planificación eficaz y la determinación de los
componentes críticos de una amenaza conducirán a un mejor diseño de emulación de la misma.


### Modelos de escenarios

Como ya se ha dicho, es habitual seleccionar un modelo de escenario que no permitirá al Equipo Rojo
alcanzar con éxito sus objetivos dentro de los límites de tiempo de un compromiso. Al seleccionar un modelo de escenario
de escenario, elíjalo en función de los impactos operativos que deben medirse. Estos modelos sólo ayudan a
diseñar un escenario. La ejecución de un escenario puede ajustarse durante un compromiso. Ser flexible
y estar preparado para hacer ajustes es fundamental. Si un equipo rojo tiene éxito demasiado rápido, las observaciones
pueden no ser valiosas. Si un equipo rojo se detiene demasiado pronto, es posible que la organización no obtenga el
impacto deseado. La selección del modelo correcto ayudará a garantizar el equilibrio adecuado.

¿Qué significa realmente "modelo de escenario"? Los modelos de escenario de emulación de amenazas incluyen el Modelo de Compromiso Completo, el Modelo de Supuesta Infracción y el Modelo de
Modelo de Compromiso Completo, Modelo de Supuesta Infracción y Modelo de Escenario Personalizado.

#### Modelo de compromiso total

El Modelo de Compromiso Completo es una emulación completa, de extremo a extremo, de una amenaza y es el modelo más común
más común deseado por las organizaciones. Piense en esto como el compromiso sin restricciones (aunque siempre hay
siempre hay restricciones). Este modelo trata de emular una amenaza desde el primer día hasta que se alcanza el objetivo final.
objetivo final.

Un modelo de compromiso total comienza con la amenaza fuera de una organización. La amenaza debe realizar
La amenaza debe realizar inteligencia de fuente abierta (OSINT), reconocimiento y enumeración para determinar un camino hacia la red.
red. Una vez dentro de la red, el Equipo Rojo continuará ejecutando su plan utilizando sus TTPs. Este
Esto continuará hasta que el Equipo Rojo sea detenido o complete su objetivo. Características del modelo de compromiso total:  
```
● Comienza el día 1 de la actividad adversaria  
● El Equipo Rojo debe realizar todas las fases (Entrar, Permanecer y Actuar; se discutirá más adelante en el texto)  
● Suele ser más largo que otros tipos de compromiso, ya que se necesita el tiempo adecuado para realizar todas las fases  
● El Equipo Rojo debe ser capaz de entrar o tener un plan de "tarjeta blanca" de respaldo  
● Con plazos de ejecución condensados, es habitual que el tiempo se agote antes de poder ejecutar los impactos operativos  
● Deben hacerse planes de contingencia para asegurar que se ejecuten los impactos requeridos  
```
#### Modelo de incumplimiento supuesto

El Modelo de Supuesta Violación asume que una amenaza tiene cierto nivel de acceso a un objetivo al inicio del
el compromiso. Este modelo es posiblemente el más beneficioso de todos los modelos. Se supone que la amenaza
que la amenaza tiene cierto nivel de acceso a un objetivo antes de comenzar. Esto hace que el escenario comience mucho más adelante en la
línea de tiempo del ataque. Asumir que alguien puede violar una red es a menudo argumentado por las organizaciones menos maduras
que asumen que los equipos rojos deben probar que pueden "entrar" antes de comenzar. ¿Cuándo es importante esta prueba?
Es importante SÓLO si es importante medir la capacidad que tiene una amenaza para "entrar". Si esto no es un objetivo
objetivo clave, el uso del Modelo de Supuesta Infracción ahorrará tiempo, esfuerzo y dinero; y liberará al Equipo Rojo
para explorar objetivos de mayor impacto.  
Características del Modelo de Supuesta Infracción:  
```
● Comienza después de que una amenaza haya vulnerado una organización  
● El Equipo Rojo se centra en las fases de Permanecer y Actuar  
● Uso más eficiente de los recursos limitados (tiempo, dinero y personal)  
● Requiere proporcionar acceso al Equipo Rojo. Esto se hace comúnmente lanzando un malware del Red  
● El malware del Equipo Rojo, proporcionando acceso a un activo específico, o proporcionando contraseñas.  
● Los impactos y objetivos operacionales deben seguir siendo alcanzados  
```
```
Considera esto
Asumir una brecha puede llevar a no creer en los resultados. Con demasiada frecuencia, el personal de defensa e incluso los altos directivos
intentan restar importancia a las actividades legítimas del Equipo Rojo. Con la supuesta violación, las organizaciones más inmaduras pueden
intentan hacerlo basando el éxito de una actividad en que se les "facilite el acceso al sistema o a la red" en lugar de
reconocer las lecciones aprendidas al entender cómo el equipo defensor fue capaz de ejecutar sus estrategias defensivas.
```
#### Modelo de violación personalizado

Los modelos de violación personalizados permiten al equipo rojo diseñar escenarios que permiten probar o medir
áreas específicas de interés para el objetivo. Un modelo de compromiso personalizado:  
```
● Puede comenzar en cualquier punto del ciclo de la amenaza  
● Se centra en cualquiera de las fases diseñadas por las metas y objetivos  
● Es altamente eficiente cuando se dispone de personal, tiempo y fondos limitados  
● Casi siempre se anuncia y se coordina con la interacción en tiempo real  
```
El Equipo Rojo debe utilizar con mayor frecuencia una estrategia de **_Asumir la Violación_**. Esta estrategia fue popularizada por
Microsoft y hay que reconocer que es más filosofía que deducción. Esperar reactivamente la evidencia de una
de una brecha hace que las compañías revelen no sólo que han sido comprometidas sino que han sido
comprometidas durante años.


### Indicadores de compromiso

Aunque se suele pensar que los adversarios pueden limpiar después de sí mismos, es casi
imposible eliminar todas las pruebas. Un buen equipo de operaciones de seguridad tiene el potencial de encontrar incluso a los
adversarios más avanzados. Siempre quedan pruebas. Los indicadores de compromiso (IOC) son
artefactos (trozos de información) que identifican o describen las acciones de la amenaza. Un IOC puede ser cualquier cosa utilizada para
identificar una acción de amenaza, incluyendo, pero no limitado a:  
```
Tráfico de red inusual  
● Actividad inusual de los usuarios  
● Conexiones geográficas específicas  
● Aumento del tráfico de red  
● Aumento de las lecturas de la base de datos  
● Cambios o modificaciones inusuales de archivos  
● Cambios o modificaciones en el registro  
● Convenciones específicas de nomenclatura o uso  
● Identificación de acciones o intentos de acción  
● Señales de DOS/DDOS  
```
La mayoría de las organizaciones de seguridad se basan en algún desencadenante para tomar medidas. Sistemas como los sensores de red,
sensores de seguridad, o incluso los usuarios finales suelen desencadenar una investigación de un comportamiento "extraño". Cuando un
Cuando un equipo de seguridad responde a un desencadenante, se enfrenta al reto de poner a prueba su capacidad de aprovechar los COI para
identificar, contener y erradicar una amenaza. Este juego entre rojos y azules generando e identificando
IOCs está en el corazón del Red Teaming. Para replicar a un actor malicioso, un equipo rojo debe
comprender las TTP de una amenaza. Estas TTP se emulan controlando el "cuándo" y el "cómo", así como
el tipo de IOC generado o dejado atrás. Teniendo en cuenta este concepto, los operadores del Equipo Rojo deben saber qué
indicadores son realizados por una herramienta o acción. Si esos IOC son aceptables, pueden proceder. Si los COIs
no son aceptables, y la acción se lleva a cabo, existe un riesgo significativo de exponer al Equipo Rojo
antes de lo previsto. No sólo es necesaria la gestión de un COI para la emulación de amenazas,
sino que un COI puede hacer que te atrapen cuando el momento no es el adecuado y también puede poner todo un
compromiso si no se controla y gestiona.

#### Herramientas de control

Para controlar los COIs, debe existir un sólido conjunto de TTPs. Parte de estas TTPs son herramientas que
que apoyan la capacidad de un Equipo Rojo. Las herramientas no sólo deben proporcionar capacidad, sino que también deben ser
comprender. Esto se hace a menudo mediante el uso y la modificación de las herramientas. El uso y la modificación de las herramientas
deben integrarse en una plataforma de ataque estándar. Si la plataforma se gestiona y se mantiene, una línea de base común
una línea de base común está lista para su uso. Como regla general, un Equipo Rojo debería:  
● Conocer las herramientas utilizadas, cómo funcionan y qué acciones se llevan a cabo  
● Recompilar las herramientas (cambiar el nombre de las funciones; eliminar la ayuda, los comentarios y las cadenas/códigos no utilizados; etc.)  
● Controlar los agentes de usuario  
● Entender qué COIs son generados por una acción  
● Mezclar hasta que el tiempo sea el adecuado  

Los siguientes son indicadores comunes y sólo un pequeño ejemplo para ayudar a pensar en los indicadores que
deben ser controlados.

```
Agentes de usuario - Las cadenas de agente de usuario pueden ser un indicio para las herramientas
Por ejemplo, la herramienta de inyección SQL SQLMAP tiene una cadena de agente de usuario por defecto que incluye
la palabra sqlmap sqlmap/1.0-dev-xxxxxxx (http://sqlmap.org) Esto es muy común.
```
```
Los binarios pueden tener firmas que pueden ser detectadas
● Puede ser necesario modificar y recompilar para cambiar la firma
● La probabilidad de detección del antivirus puede disminuirse eliminando los comentarios y otras salidas del usuario antes de compilar
```
```
Punto de enfoque
El estado final de la planificación de la amenaza es la capacidad de representar la amenaza lo más fielmente posible para permitir la capacidad de asesorar al objetivo de las implicaciones para el entorno de destino.
```

### Conceptos de compromiso

Los compromisos del Equipo Rojo pueden pasar por varios pasos complejos y detallados durante la ejecución, pero
utilizar tres fases simples ayuda a mantener el enfoque en los objetivos. Aunque el Red Teaming tiene un enfoque ofensivo
Aunque el Red Teaming se centra en la ofensiva, en última instancia se utiliza como herramienta para mejorar la seguridad. El Red Teaming se ejecuta en tres fases
directamente relacionadas con las áreas de defensa que se pueden probar y medir contra una amenaza. Es habitual que las
Es común que las operaciones de seguridad se centren en una enorme cantidad de tiempo y energía en los controles preventivos para "mantener
la amenaza". La prevención es importante; sin embargo, la prevención al 100% no es factible. Una organización
debe comprender los impactos potenciales si una amenaza tiene éxito.

#### Fases de ejecución

![Alt Image](./Images/14.png)

En un nivel alto, un Equipo Rojo debe moverse a través de estas tres fases para completar un compromiso.

**Entrar -** Obtener acceso a una red. El Equipo Rojo debe tener acceso a su objetivo. El acceso puede ser
a través de un compromiso legítimo o el acceso se concede directamente como parte de un supuesto escenario de violación,
como un escenario de amenaza interna.

¿Puede una organización detectar una amenaza que accede a su red? ```  

**Permanecer -** Establecer una persistencia o una presencia permanente. Los compromisos de los equipos rojos suelen ser más largos
que otros tipos de pruebas. Un equipo rojo suele establecer una persistencia o una presencia permanente para
para sobrevivir a la duración del compromiso.

``¿Puede una organización detectar o evitar que una amenaza viva en su red? ```  

**Actuar -** Por último, un Equipo Rojo realiza impactos operativos contra el objetivo

¿Qué impactos puede realizar una amenaza basándose en las capacidades adquiridas durante la entrada y la permanencia?   

#### Mapa de fases

La mayoría de los marcos de pruebas de penetración se dividen en fases individuales que se centran en
la identificación y la explotación de la vulnerabilidad. La metodología de Red Team clasifica muchas de las
mismas acciones en sólo tres fases distintas con un enfoque en los impactos causados al entorno
objetivo. A continuación se ofrecen varios ejemplos de esta categorización.

![Alt Image](./Images/15.png)

##### ENTRAR

Reconocimiento  
```
● Realizar inteligencia de fuente abierta (OSINT) contra el objetivo.  
● Buscar utilizando fuentes abiertas y no autenticadas:  
        ○ Sitios web del objetivo  
        ○ Medios sociales  
        ○ Motores de búsqueda  
        Repositorios públicos de código  
        ○ Sitios de destino alternativos  
```
Enumeración externa  
```
● Identificar los activos externos:  
        ○ Realizar un escaneo DNS inverso para identificar los hosts registrados.  
        ○ Identificar las URL y otros puntos de contacto externos a partir del escaneo y la OSINT  
● Evaluar la presencia en la web:  
        ○ Navegar como un usuario normal a través de un proxy web para capturar inteligencia y comprensión  
        ○ Identificar las vulnerabilidades conocidas y las condiciones vulnerables  
        ○ No enviar código de ataque en este momento.  
● Ejecución y explotación  
        ○ Intentar explotar los objetivos basándose en los conocimientos actuales  
        ○ Realizar el conocimiento de la situación del objetivo  
        ○ Intentar la elevación local de privilegios  
        Intentar elevar los privilegios a nivel de dominio o de sistema.  
```
##### QUEDARSE EN

Post-explotación  
```
● Continuar con la enumeración interna y de dominio  
● Identificar los usuarios/grupos/membresías del dominio  
● Identificar el espacio IP  
● Identificar los recursos compartidos de archivos  
● Establecer la persistencia  
● Utilizar el plan de persistencia para colocar agentes en los sistemas de destino  
● Mover lateralmente  
```

**ACT**

Impactos operativos  
```
● Realizar una simulación realista contra los sistemas objetivo  
● No necesita ser altamente complejo  
● No necesita aprovechar vulnerabilidades conocidas o tradicionales  
● No siempre requiere privilegios administrativos (local/dominio)  
● Requiere un impacto real en el entorno objetivo  
Requiere la aportación del GEC y de la AT  
● Requiere la notificación al GEC y a la AT cuando se ejecuta el impacto operativo  
        ○ Evita acciones defensivas no deseadas (y posiblemente catastróficas)  
● Sí necesita ejercitar al menos uno de los planes y procedimientos de detección, respuesta a incidentes, continuidad y recuperación del objetivo  
```

Los impactos operativos son un elemento clave para distinguir los compromisos de Red Teaming de otros tipos de pruebas y proporcionan una visión real de la capacidad de las operaciones de seguridad para defenderse de las amenazas  
```
Se descubrirán y aprovecharán las vulnerabilidades; sin embargo, las vulnerabilidades son un subproducto de un compromiso de Red Team
de un equipo rojo, no el objetivo. El verdadero valor de un Red Team es ayudar al objetivo a identificar los controles administrativos, técnicos y
y procedimentales que limiten el impacto en la organización incluso cuando sea vulnerable a la última "vulnerabilidad de día cero".
```

#### Impactos operativos

Como en cualquier evaluación de seguridad, el riesgo es lo que mueve a una organización a actuar. Los impactos operativos son una
herramienta del Equipo Rojo para demostrar estos riesgos. El impacto en la capacidad operativa de una organización es uno de los métodos más eficaces para mostrar el riesgo a una organización.
de los métodos más eficaces para mostrar el riesgo a los altos cargos de una organización.

Los impactos operativos son acciones o efectos realizados contra un objetivo y están diseñados para demostrar
las debilidades físicas, informativas y operativas de la seguridad. Los impactos operativos pueden considerarse
acciones realizadas contra una organización que afectan a su funcionamiento. Estos impactos pueden ser tan generales
como realizar un ataque de denegación de servicio o más específicos, como utilizar equipos ICS secuestrados para
controlar la red eléctrica de una ciudad.

Los impactos se suelen realizar al final de un compromiso; sin embargo, es mejor planificar los efectos deseados con antelación.
efectos deseados. La planificación temprana permite al Equipo Rojo utilizar el acceso y las capacidades obtenidas para posicionarse mejor para la ejecución del impacto.
para posicionarse mejor para la ejecución del impacto, lo que se conoce como preposicionamiento. Además de obtener y mantener
Además de obtener y mantener el acceso, el Equipo Rojo debe limitar la interacción con los objetivos del impacto operativo. Este
Esto garantiza que todos los objetivos del impacto operacional puedan ejercerse en el momento adecuado. A menudo, el Equipo Rojo
A menudo, el Equipo Rojo recibirá una solicitud para causar impactos prematuros en el entorno del objetivo. Estas acciones
necesitan una cuidadosa revisión y consideración antes de su ejecución. Si estas acciones no ponen en peligro la capacidad del equipo
Si estas acciones no ponen en peligro la capacidad del equipo para cumplir con otros objetivos del compromiso, pueden ser ejecutadas desde otros espacios de ataque y
sistemas que no sean críticos para los objetivos del compromiso. Si las acciones entran en conflicto directo con los objetivos del compromiso,
el jefe del equipo rojo debe asegurarse de que el GEC y el AT comprendan plena y completamente las
ramificaciones de cada acción (para incluir futuros impactos operativos).

El nivel de profundidad y el impacto pueden ser tan "dolorosos" como una organización esté dispuesta a explorar. Estos impactos de
impactos se realizan normalmente contra sistemas de producción en vivo para tener el mayor nivel de fidelidad
pero pueden ejecutarse en entornos de prueba y desarrollo si son representativos.

```
Punto de atención
Los entornos de prueba rara vez modelan la producción al nivel en que se sienten los impactos operativos. Las tecnologías pueden
Las tecnologías pueden coincidir, pero las personas y los procesos no suelen hacerlo. Centrarse sólo en el entorno de pruebas puede llevar a una
una visión poco realista de cómo el impacto afecta a una organización.
```

Puede ser muy difícil obtener el permiso de la dirección para realizar impactos operativos. Si una
Si una organización es muy reacia al riesgo, estos impactos pueden parecer demasiado costosos o peligrosos. Las organizaciones que
que expongan sus sistemas a un ataque a gran escala que incluya impactos operativos sentirán definitivamente el
dolor. Sin embargo, la planificación y ejecución detalladas limitan los impactos en el mundo real, gestionan los riesgos potenciales,
identifica las deficiencias tanto en la seguridad como en las operaciones, y proporciona lecciones extremadamente valiosas a todas las partes interesadas.


### Desconflicción

La desconflicción es la capacidad de identificar qué actividad genera el Equipo Rojo y cuál no.
En general, la desconflicción:  
```
● Separa la actividad del Equipo Rojo de la actividad del mundo real  
● Requiere una coordinación previa a través de un proceso de desconflicción  
● Obliga a que el Equipo Rojo reciba los registros defensivos específicos del incidente  
● No debe utilizarse como un proceso de identificación del Equipo Rojo  
● Requiere que todos los incidentes detectados, ya sea en el mundo real o en la supuesta actividad del Equipo Rojo, sean reportados inmediatamente usando los procesos normales de reporte de incidentes  
● Puede requerir que el POC de Células Blancas se ponga en contacto con el POC del Equipo Rojo para determinar si las actividades descubiertas son el resultado del Equipo Rojo
```
Es fundamental que el personal de todos los niveles del compromiso sea capaz de distinguir rápida y correctamente
distinguir la actividad del Equipo Rojo de los ataques del mundo real. Varios factores pueden aliviar la confusión y la
confusión y la difusión de información errónea; sin embargo, estas cuatro sencillas acciones son de gran ayuda en el
proceso de desconflicción:  
```
● Asegurarse de que los agentes de confianza/célula blanca comprenden las acciones y los impactos de las actividades a medida que se producen  
● Asegurarse de que todos los registros de los operadores (OPLOGS) se completan de forma precisa y exhaustiva  
● Proporcionar los OPLOGS y las listas de actividades al ECG según se solicite  
● Intercambiar informes de situación periódicos con la Célula Blanca
```
#### Proceso de desconflicción y documentación

Como mínimo, la documentación de desconflicción debe incluir:
```
● Las fechas del compromiso  
● POC para el compromiso  
        Dirección  
        ○ Técnico  
        ○ ECG/TA/Whitecell  
● Origen de las actividades  
● Destino de las actividades (según corresponda al tipo de compromiso)  
        ○ Segmento, rango, aplicación, host, IP, edificio, campus, etc.  
        ○ En la mayoría de los escenarios, no se proporciona el destino  
                ■ Desconflicción realizada a través de la AT/celda blanca  
● Descripción de la actividad
```
En el caso de que se solicite la desconflicción, el Jefe del Equipo Rojo debe trabajar con el responsable
TA/Célula Blanca POC, evaluar la información y aislar la información de la actividad del Equipo Rojo. Este
proceso puede incluir:  
```
● Detener todas las actividades en el área del incidente  
● Revisar las ROE para ver las limitaciones, los objetivos y las instrucciones de desconflicción  
● Revisar los OPLOGS para determinar las actividades que el equipo estaba realizando en el momento indicado  
● Confirmar o negar las actividades del Equipo Rojo para cada incidente de desconflicción  
● Confirmar los hallazgos con el ECG, Célula Blanca y el AT  
● Asegurar que los hallazgos sean transmitidos por correo electrónico así como por teléfono  
● Mantener los registros de la información, las acciones, la evaluación y los hallazgos de la desconflicción  
```
Si el proceso de desconflicción indica que el Equipo Rojo es el iniciador:  
```
● Determinar y aislar las actividades específicas y los guiones empleados (si es necesario)  
● Determinar y aislar los registros específicos que soportan el marco temporal del incidente  
● Notificar al Grupo de Control del Compromiso  
```
El proceso de desconflicción proporciona una vía para que un compromiso sea "jugado" y es susceptible de
flujos de información sesgados. Parte del proceso de planificación del compromiso debe incluir la determinación de la
tiempo necesario para ejecutar el proceso de desconflicción y cuándo utilizarlo adecuadamente.

Siempre hay que enfatizar que no hay ningún escenario en el que la desconflicción sea utilizada por el entorno del objetivo o
defensores para identificar las fuentes o actividades del Equipo Rojo. En ningún momento se debe proporcionar al entorno del objetivo o a los defensores
defensores deben recibir información fuera del proceso de desconflicción, excepto en el caso de incidentes legales o de seguridad.
de seguridad o legales.

#### Proceso de desconflicción

```
1. Todas las alertas e incidentes, ya sean del mundo real o de supuesta actividad del Equipo Rojo, deben ser reportados inmediatamente y se debe actuar de acuerdo con las políticas y prácticas estándar de respuesta a incidentes.  
2. 2. El personal apropiado de operaciones de seguridad, respuesta a incidentes, inteligencia de amenazas o gestión (por ejemplo, el Agente de Confianza) notificará inmediatamente al Jefe del Equipo Rojo (o al apoderado designado) de cualquier incidente reportado. Esta notificación debe incluir la fuente, el destino, la acción, la hora de la acción y la fuente de la alerta.  
3. El equipo de respuesta apropiado continuará realizando las operaciones según la política y la práctica.  
4. El jefe del equipo rojo determinará si la alerta o actividad fue generada o realizada por el equipo rojo. Esta determinación se hará mediante una revisión exhaustiva del registro del operador de eventos, así como mediante la interacción directa del operador.  
5. El Jefe del Equipo Rojo proporcionará al Agente de Confianza una confirmación o negación de la actividad del Equipo Rojo.  
        a. Si la actividad es real, la desconflicción está completa.
                i. El Equipo de Lectura se retirará de cualquier activo involucrado en el incidente (si se utiliza) o añadirá temporalmente esos activos a una lista de activos restringidos.  
                ii. El equipo de respuesta continuará las operaciones  
        b. Si hay actividad del Equipo Rojo, las actividades de desconflicción continuarán.
                i. El agente de confianza no debe proporcionar esta información al equipo de seguridad o de respuesta hasta después de completar el proceso  
6. El jefe del equipo rojo y el agente de confianza evaluarán lo siguiente para determinar qué información (si la hay) debe proporcionarse al equipo de respuesta:  
        a. La medida en que la actividad causará una notificación innecesaria a la alta dirección de la organización  
        b. Las actividades que debe realizar el equipo de respuesta de acuerdo con las políticas y prácticas  
        c. Cómo afectarán las actividades de respuesta a la disponibilidad y eficacia del equipo para detectar, identificar y responder a otros incidentes  
        d. Cómo afectarán las actividades de respuesta a los sistemas y redes del lugar del incidente  
        e. Cómo afectarán las actividades de respuesta a las operaciones diarias de quienes no pertenecen a los equipos de respuesta correspondientes  
        f. Cantidad de esfuerzo requerido para identificar y aislar con precisión al equipo rojo frente a los beneficios de responder al incidente a efectos de formación, herramientas y métricas  
7. Las acciones de evaluación pueden ser acordadas por el líder del equipo rojo y el agente de confianza o, si es necesario, escaladas al nivel de gestión apropiado (ECG) para su aprobación.  
8. La recomendación de evaluación del incidente debe indicar si el Equipo Rojo y los equipos de respuesta continuarán con las actividades de alcance total, si se proporcionará la información para limitar las actividades a un nivel de esfuerzo aceptable, o si se detendrán las operaciones.  
        a. Si no se proporciona información al equipo de respuesta, las actividades de alcance total deben reanudarse. Los equipos de respuesta no deben ser notificados de la actividad del Equipo Rojo.  
        b. Si se proporciona información, todos los equipos deben registrar la información y la hora proporcionada y los equipos de respuesta deben proceder con las actividades de respuesta utilizando la información proporcionada como "Inteligencia de Amenazas" o "directrices".  
        c. Si se determina que las acciones específicas tienen un nivel de esfuerzo demasiado alto, todos los equipos deben ajustar la actividad actual para acomodar la exclusión de esfuerzo. Esto puede ser:  
                i. Continuación del Equipo Rojo pero detención de las actividades de respuesta  
                ii. Continuación de la respuesta pero interrupción de las actividades del Equipo Rojo  
                iii. Continuación del Equipo Rojo pero reducción de las actividades de respuesta  
                iv. Continuación de la respuesta pero reducción de las actividades del Equipo Rojo  
                v. O cese de todas las actividades  
9. Las determinaciones finales de desconflicción se llevarán a cabo y se registrarán para informar sobre el evento, así como para la revisión posterior a la acción  
Las revisiones posteriores a la acción pueden utilizarse para estimular mejoras en el proceso de desconflicción, así como
respuesta a incidentes u otras operaciones de seguridad.
```

### Manejo de datos

Las directrices generales para el manejo de los datos generados o recopilados durante un compromiso del Equipo Rojo son fundamentales.
Todos los miembros del Equipo Rojo deben ser responsables de salvaguardar todos los datos del objetivo (es decir, del cliente),
incluyendo:
```
● Información personal identificable (PII): información que puede utilizarse para identificar, contactar o localizar de forma exclusiva a una sola persona o que puede utilizarse con otras fuentes para identificar de forma exclusiva a un solo individuo.  
● Información de la Ley de Privacidad de acuerdo con las regulaciones, políticas y procedimientos establecidos para el manejo de información restringida y sensible  
● Otros datos de BBP de la industria
```
Un Equipo Rojo debe evitar la extracción de datos de archivos que contengan información de la Ley de Privacidad, médica, de justicia, de culto
o religioso, o cualquier otra información protegida o privilegiada. Si se encuentra información protegida o privilegiada
Si se encuentra información protegida o privilegiada, el Equipo Rojo debe detener las acciones para obtener o proporcionar acceso, proteger
la información, notificar al GEC y devolverla al entorno de destino (o eliminarla adecuadamente según
de acuerdo con el tipo de datos según las reglas de juego).

Un Equipo Rojo normalmente está autorizado a explotar archivos, correo electrónico o tráfico de mensajes almacenados en la red o
comunicaciones que transitan por la red para el análisis específicamente relacionado con el cumplimiento de los
objetivos (por ejemplo, identificar identificaciones de usuarios, contraseñas o direcciones IP de la red para obtener más
acceso); sin embargo, cada miembro del Equipo Rojo debe asegurarse de que toda la información explotada es necesaria y
dentro del alcance del compromiso.
Un Equipo Rojo no debe modificar o borrar ningún dato de usuario de producción ni realizar ningún ataque de denegación de servicio
de servicio a menos que el ECG o la ROE lo soliciten o autoricen específicamente. El equipo no debe
El equipo no debe degradar o interrumpir intencionalmente las operaciones normales de los sistemas objetivo que se están explotando.

Los operadores del equipo rojo deben seguir las disposiciones establecidas en las ROE. Unas ROE debidamente documentadas
contener orientación y reglas relacionadas con los permisos, autorizaciones, acciones permitidas, requisitos de recolección de datos y detalles del espacio objetivo.
requisitos de recopilación de datos y detalles del espacio objetivo. Todos los miembros del Equipo Rojo deben adherirse a los permisos otorgados
durante la planificación del compromiso.

#### Controles

Los controles en torno al manejo de los datos de los clientes deben ser acordados y documentados en las ROE. Estos controles
controles son fundamentales. Recuerde que un equipo rojo tiene el privilegio de "jugar en el campo de juego de otra persona".
de otra persona". Este acceso debe ser respetado, y los datos capturados deben ser protegidos.

A continuación se presentan los controles generales y las sugerencias a tener en cuenta para salvaguardar los datos sensibles. Ajústelos según
ajustarlos como sea necesario e incorporarlos a su plantilla de ROE.

**Controles de política**  
Los controles de política implementados por el Equipo Rojo deben incluir:  
```
● Un acuerdo de no divulgación del equipo rojo firmado por cada miembro del equipo rojo  
● Formación en materia de datos (identificar y evitar la PII, los datos PIA, etc.)  
● Formación en materia de ética  
● Comprobación de los antecedentes individuales  
```
**Controles físicos  
Deben existir múltiples niveles de controles físicos para proteger las herramientas de compromiso y los sistemas operativos
de la pérdida intencionada o no intencionada. El personal del Equipo Rojo debe estar familiarizado con todos los controles físicos
controles físicos empleados (por ejemplo, cerraduras, pegatinas de identificación, cajas fuertes, armarios
cajas fuertes) y su uso adecuado. Cada miembro del Equipo Rojo es personalmente responsable de la
protección de los datos del objetivo.

Los mecanismos de seguridad recomendados para asegurar los activos del objetivo incluyen:  
```
● Las herramientas, los sistemas informáticos y los datos del objetivo deben almacenarse dentro de una sala aislada y segura, y ser controlados únicamente por el Equipo Rojo.  
● Minimizar el contacto entre el equipo y las entidades externas (controles de acceso físicos internos/externos al espacio/configuración del Equipo Rojo).  
● Cuando no se utilicen, todos los datos y equipos deben retirarse y colocarse en maletines con cerradura, cajas fuertes o armarios de almacenamiento.  
● Cuando se viaja, los ordenadores portátiles y los discos duros deben estar protegidos (en una caja fuerte del hotel, atados, en una caja de seguridad atada, etc.) en todo momento y nunca deben dejarse sin asegurar en un coche, hotel, espacio del cliente, etc.  
● Todos los visitantes a un espacio del Equipo Rojo serán escoltados.  
● Los datos del objetivo deben ser manejados únicamente por el personal del Equipo Rojo que tenga necesidad de conocerlos.  
● Al finalizar el compromiso, toda la información del objetivo se devolverá al cliente o se destruirá siguiendo los procedimientos definidos.  
```
**Controles de software**  
Se deben emplear los siguientes controles de software, diseñados para garantizar la confidencialidad, el anonimato y la seguridad de la información:  
```
● Cada sistema operativo anfitrión e invitado debe estar encriptado  
● Utilizar una política de contraseñas eficaz, y considerar (debería utilizar) una base de datos de contraseñas protegida por múltiples factores para almacenar contraseñas únicas para cada compromiso  
● Cada sistema operativo anfitrión e invitado debe estar protegido con una contraseña "fuerte"  
● Cada sistema operativo anfitrión e invitado debería emplear un cortafuegos basado en el anfitrión específico para el compromiso  
● Cuando sea posible, las comunicaciones deben estar cifradas  
● Tenga en cuenta que el Equipo Rojo nunca debe utilizar sistemas de archivos o comunicaciones no seguros para las operaciones de compromiso desarrolladas por el equipo (es decir, FTP, Telnet, HTTP, VNC, WEP, etc.)  
Utilizar mecanismos (más) seguros para las comunicaciones (es decir, HTTPS, WebDAV, SSH, radmin, RDP, etc.)  
● Los datos y las herramientas utilizadas durante un compromiso deben almacenarse en un contenedor cifrado y trasladarse al directorio de trabajo sólo cuando sea necesario  
Todos los sistemas, el almacenamiento, los datos y las herramientas deben estar cifrados en todo momento (datos en tránsito, datos en reposo).  
● Se recomienda el uso de algoritmos de cifrado de alta resistencia conocidos y probados por la comunidad  
● Todos los datos y herramientas transferidos hacia o desde los sistemas de destino deben tener hash usando MD5, SHA1, o SHA256 y añadirse al OPLOG como se discute en la sección de Recogida de Datos  
● Todo acceso, movimiento y uso de datos y herramientas debe añadirse al OPLOG  
● Si una herramienta ya no es necesaria para una tarea, debe eliminarse del entorno de destino  
● Todas las herramientas y el software del Equipo Rojo deben eliminarse del entorno de destino al final del compromiso. Si la limpieza no es posible, se debe notificar al AT y al ECG y proporcionarles los detalles adecuados.
```
**Integridad de dos personas (TPI)**  
Un factor clave en la recogida y ejecución de datos es la integridad de dos personas (TPI). La integridad de dos personas
(utilizada para verificar las actividades realizadas durante el compromiso) debe mantenerse en todo momento. Un miembro del equipo
Un miembro del equipo debe revisar, comprender y proporcionar una "comprobación de cordura" para cada acción/comando
realizada. Ese miembro del equipo debe verificar las acciones del miembro del equipo ejecutor, así como
verificar la finalización de la entrada en el registro. El TPI ayuda a proteger tanto al Equipo Rojo como al objetivo/cliente
contra la posible divulgación de información sensible, la violación de requisitos legales/leyes y la
violación de las ROE. Más a menudo, la TPI evita que el Equipo Rojo cometa simples errores y
errores en la operación (esto se explora más a fondo en la sección Ver orientación sobre el oficio, consultar con los compañeros
sección).


### Conclusiones clave del capítulo

La planificación del compromiso es crucial para gestionar eficazmente los posibles riesgos del compromiso, ejecutar con éxito
ejecutar con éxito para lograr las metas y objetivos deseados, y proporcionar la información necesaria para
mejorar las capacidades organizativas y defensivas. Aunque todos los elementos de la planificación desempeñan un
Aunque todos los elementos de planificación desempeñan un papel importante en el éxito de la intervención, hay que prestar especial atención a los siguientes aspectos
```
Roles y responsabilidades
Las reglas del combate
Planificación de la amenaza
Impactos operacionales
Deconflicción
Manejo de datos
Financiación
```

### ```Tareas

```
1) Crear una carta de operaciones del equipo rojo y una guía metodológica
2) Crear un documento de funciones y responsabilidades
3) Crear una plantilla de perfil de amenaza
4) Desarrollar una plantilla de ROE estándar
5) Desarrollar una plantilla de desconflicción
6) Desarrollar una guía de manejo de datos
7) Seguir añadiendo definiciones al léxico del equipo rojo
```

## Ejecución del compromiso

![Alt Image](./Images/16.png)

La ejecución del compromiso comienza cuando se finaliza la información del evento y la documentación de planificación, y
y comienzan las acciones preparatorias para llevar a cabo el compromiso. La fase de ejecución es simplemente la aplicación práctica
la aplicación práctica del "por qué" y el "cómo" de la planificación (piense en la construcción de la infraestructura y las actividades de participación).
actividades de participación).


### Repositorio de datos

Todos los datos recogidos durante la intervención deben registrarse, archivarse según el tipo de datos y almacenarse en un
repositorio específico de la intervención. Este repositorio debe estar ubicado en un volumen encriptado dentro de un
servidor centralizado / NAS / archivo compartido que se pueda montar o al que sólo se pueda acceder tras la autenticación.

Si se encuentra en una ubicación externa, un enfoque práctico es designar un ordenador portátil y crear un directorio
para almacenar los datos del compromiso. Asegúrese de que este directorio se copie diariamente en otro portátil.
Recuerde que el sistema de archivos debe almacenarse de acuerdo con la política, los controles físicos y de software
y de software, tal y como se ha comentado anteriormente.

Al comenzar las operaciones, el jefe del equipo rojo debe montar el volumen específico del compromiso dentro del
(un volumen cifrado que requiere autenticación). Una vez completado, cada Operador del Equipo Rojo
deberá montar el directorio localmente para su uso en el compromiso (requiere autenticación del usuario). Al final del
día, cada operador deberá desmontar el directorio, y el jefe del equipo rojo deberá desmontar el volumen del repositorio
volumen.

Un método probado y recomendado para el acceso colaborativo seguro a un repositorio común es
montar un sistema de archivos remoto a través de SSH. Este método requiere autenticación para el acceso y
aprovecha un mecanismo de transporte encriptado.

Existen numerosas formas de realizar esta tarea. A continuación se muestra un ejemplo rápido:

```
1) Instalar SSHFS:
apt-get install sshfs
```
```
2) Crea un directorio "data" que se utilizará para la recolección:
Mkdir /data
```
```
3) Monte el repositorio común a través de SSHFS introduciendo la contraseña. Nota: El jefe del equipo rojo
debería haber creado una jerarquía de eventos (como se discute en Jerarquía de Archivos) antes de este paso.
sshfs -o allow_other,defer_permissions
redteammember1@<target>:/ruta_al_repositorio_de_compromiso/ /datos
```
```
4) Alternativamente, monte el repositorio común a través de SSHFS usando claves:
sshfs -o allow_other,defer_permissions,IdentityFile=~/.ssh/id_rsa
redteammember1@<target>:/ruta_al_repositorio_de_compromiso/ /datos
```
```
5) Utilizar:
ls /data
```
```
6) Desmontar el sistema de archivos:
unmount /data
```

Puede encontrar más orientación sobre el uso de sshfs en la página man de sshfs (man sshfs) o en
https://linux.die.net/man/1/sshfs.

Aunque la siguiente estructura y método no son necesarios para las operaciones de Red Team, es MUY
recomendado si no existen otros procesos o herramientas de recolección de datos. Aprovechando las lecciones aprendidas, esta
estructura fue diseñada para facilitar el flujo operativo eficiente de almacenamiento de datos durante un compromiso
durante un compromiso, al tiempo que mejora la capacidad del líder del Equipo Rojo para controlar la adquisición, el flujo y la notificación de la información.
información.

#### Jerarquía de archivos

//repositorio/nombre_del_compromiso/0-admin

```
● Información administrativa de eventos-listas de IPs aprobadas, ROE, briefings, etc.
```
//repositorio/nombre_del_compromiso/1-osint

```
Información OSINT recopilada antes del evento
```
//repositorio/nombre_del_compromiso/2-recon

Información de reconocimiento (búsquedas DNS, escaneos NMAP, información de testigos oculares, etc.)
//repositorio/nombre_del_compromiso/3-objetivos

```
● Información específica de cada objetivo (usuarios locales, árboles de archivos, salida de comandos, etc.)  
● Información específica del dominio (DSQUERY, usuarios del dominio, controladores del dominio, archivos compartidos)
```
//repositorio/nombre_de_compromiso/3-objetivos/nombre_de_hosting/exfil

```
● Datos exfiltrados por objetivo (archivos de contraseñas, datos de usuarios, diagramas, etc.). Debe haber una
carpeta separada por objetivo (ip_hostname o URL).
● Los servidores de archivos deben tener cada uno su propia carpeta EXFIL y ser tratados como objetivos separados a
para el propósito de EXFIL.
```
//repositorio/nombre_del_compromiso/4-pantallas

```
● Las capturas de pantalla con el formato YYYYMMDD_HHMM_IP_Description.jpg/png deben almacenarse
aquí sin importar su origen. Las capturas de pantalla generadas por el anfitrión, el invitado, la aplicación, la herramienta y la pantalla de impresión
generadas por el host, la aplicación, la herramienta y la impresión de pantalla deben ser copiadas en esta ubicación.
```
//repositorio/nombre_del_compromiso/5-cargas_de_pago

```
● TODOS los payloads (EXEs, scripts, correos electrónicos de phishing) deben ser almacenados en el subdirectorio apropiado
subdirectorio y entrar en el OPLOG.
● Esto permite al equipo rastrear todas las cargas útiles que se crean y empujan en una red de destino
para su posterior limpieza, desconfiguración, etc.
```

//repositorio/nombre_del_compromiso/6-logs

```
● Almacena todos los registros exportados en el directorio correspondiente.
● El OPLOG final se almacena aquí (ejemplo: //repositorio/nombre_del_compromiso/6-
logs/20190301_170100_OPLOGredteamconsole1.xls|csv|etc.).
```
//repositorio/nombre_del_compromiso/6-logs/redteamconsole1

```
● Copie todos los registros en el directorio del sistema de Red que corresponda.
Datos brutos de la consola (ejemplo: //repositorio/nombre_del_compromiso/6-
logs/redteamconsole1/20190308_151312_CDT.terminal.log.raw)
● Registros de herramientas/aplicaciones.
Los OPLOGs diarios se almacenan aquí (ejemplo: //repositorio/nombre_del_compañero/6-
logs/readteamconsole1/20190308_151820_OPLOG.xls|csv|etc.).
```

![Alt Image](./Images/17.png)

Ejemplo de la estructura de archivos del repositorio de datos


### Recogida de datos

La recogida de datos impulsa el valor del propio compromiso. La recogida de datos debe ser completa,
permitir la replicación de las actividades y los resultados, e identificar elementos de interés significativo para los
operadores. Los conjuntos de datos finales deben incluir:

```
● Datos previos al evento (OSINT, ROE, lista de POC, etc.)  
● Datos de ejecución  
        ○ Registros de los operadores (recopilación manual de datos).  
        ○ Recogida de datos y registros automatizados  
        ○ Capturas de pantalla  
● Datos posteriores al evento (archivo de datos, informe de cierre si se realiza, e informe final)  
```
#### Registros de actividad

Todas las actividades relacionadas con la operación del Equipo Rojo deben registrarse tan pronto como se inicie el compromiso
y sólo terminar después de que se haya completado toda la actividad relacionada con el compromiso.

Algunos ejemplos de eventos que deben registrarse son  
```
Actividades de escaneo  
Eventos de explotación  
● Esfuerzos de estimulación  
● Solicitudes de desconflicción  
● Información sobre los objetivos descubiertos  
● Objetivos adquiridos y perdidos  
● Eventos del sistema (cortes, tiempos de inactividad, etc.)  
● Intentos de inicio de sesión  
● Credenciales capturadas  
● Credenciales utilizadas  
● Modificaciones del sistema de archivos  
● Modificación o desactivación de los controles de seguridad  
● Modificación o supresión de alertas o registros de seguridad  
● Métodos de acceso  
● Métodos de persistencia empleados  
● Canales de mando y control establecidos  
● Solicitudes de aumento, disminución o pausa de la actividad  
● Conflictos, solicitudes y modificaciones de las ROE  
```

Todos los datos recogidos durante el compromiso deben ser registrados, archivados según el tipo de datos, y almacenados en
un archivo compartido específico del encargo, preferiblemente en tiempo real. Como se ha comentado en la sección Manejo de datos del cliente
como se ha comentado en la sección Manejo de datos del cliente, este archivo compartido debe estar ubicado en un volumen montable y encriptado dentro de un servidor o NAS centralizado.
centralizado o NAS.  

Punto de enfoque
```
Es importante imponer el valor de las acciones fallidas. Muchos operadores capturan sólo las acciones exitosas realizadas
durante el compromiso. En muchos casos, el fracaso de una acción específica (y sus detalles asociados) proporciona más
valor tanto para el objetivo como para el Equipo Rojo que muchos éxitos.
```
#### Registros del operador

Como se ha dicho anteriormente, todas las actividades deben registrarse de forma precisa y concisa. Como mínimo, se debe recoger y registrar la siguiente información
Como mínimo, se debe recopilar y registrar la siguiente información para cada acción realizada:  
```
● Marca de tiempo de inicio (se recomienda UTC)  
● Marca de tiempo de finalización (UTC recomendada)  
● IP de origen (dirección IP del sistema de ataque/prueba)  
● Nombre de host de origen  
● IP de destino (dirección IP de destino)  
● Nombre de host de destino  
● Puerto de destino (Puerto de destino)  
● Nombre del sistema de destino  
● IP de pivote (si procede, enumere la IP de cualquier sistema utilizado como pivote, reenviador de puertos, etc.)  
● Nombre del host pivote  
● Puertos del pivote (si procede, enumere los puertos de envío y recepción aprovechados en el sistema del pivote)  
● URL (Nota, es importante capturar la URL COMPLETA de la instancia de destino)  
● Herramienta/Aplicación  
● Acción (Qué actividad o acción se realizó)  
● Comando (Comando completo)  
● Salida (Salida o respuesta del comando)  
● Descripción (por qué o para qué se realizó la acción)  
● Resultado (Exitoso, Fallido, Logrado, etc.)  
● Modificación del sistema (Archivo modificado, ubicación binaria eliminada, funciones habilitadas, etc.)  
● Comentarios  
● Captura de pantalla (Nombre del archivo de la captura de pantalla)  
● Nombre del operador  
```
Recuerde: Al crear entradas de registro, documentar acciones, cargar/descargar archivos, soltar
binarios, etc. Es beneficioso registrar utilizando el formato YYYYMMDD_HHMM_IP_Description.

Ejemplos:
```
● Marca de tiempo de inicio: Acción de destino
        ○ 20170308_151801
● Captura de pantalla del puerto 445 de Nmap
        ○ 20170308_1518_10.10.1.106_nmap445.png
● Captura de pantalla del recurso compartido smb abierto
        ○ 20170308_1519_10.10.1.106_smb_share.png
● Captura de pantalla del archivo de contraseñas
        ○ 20170308_1525_10.10.1.106_smb_share_passwords.txt
```
Los registros detallados proporcionan una instantánea de dónde se encuentra un operador durante un compromiso y pueden utilizarse para
para conocer el estado de la operación en su conjunto. Este tipo de información es fundamental para rastrear los pasos
de un compromiso para gestionarlo adecuadamente, resolver las solicitudes de desconflicción y garantizar que los datos
de que los datos estén disponibles para producir un informe de calidad. Los registros deben contener todos los pasos principales que proporcionan
que proporcionan el quién, el qué, el cuándo, el dónde, el por qué y el cómo de una acción o serie de acciones. Además de un registro de texto,
una captura de pantalla es una forma excelente de visualizar una acción. Una vez que se ha completado un compromiso, los registros son todo lo que queda.
que quedan. La calidad de una intervención está directamente relacionada con la calidad de los registros.

#### Recogida de datos automatizada

Cuando esté disponible, el Equipo Rojo debe aprovechar el uso de herramientas y scripts para capturar y
consolidar los datos de la intervención.

La recopilación automatizada de datos por sí sola nunca será suficiente para capturar los detalles necesarios para un informe final bien escrito.
informe final bien redactado; sin embargo, puede ser útil para capturar los datos brutos necesarios para validar las actividades,
reproducir los resultados y apoyar las recomendaciones. La recopilación automatizada, si se emplea adecuadamente
complementa el flujo de trabajo del Equipo Rojo y permite al operador continuar las operaciones con la
captura manual de los datos pertinentes a la actividad realizada.

**Registros de terminales**  
Todos los sistemas de intervención del Equipo Rojo deben tener una recopilación automatizada de los datos brutos de la terminal/consola.
Cada comando debe llevar el prefijo de la dirección IP del operador y la marca de tiempo UTC. Aunque existen
Hay muchos métodos para automatizar el etiquetado y la recopilación (TMUX, Script, Pantalla, etc.), es más importante
importante que los datos sean capturados con precisión que ser capturados de una manera diferente. Simplemente guardando estos
etiquetados en una ubicación como /root/logs/terminal/ puede simplificar significativamente la consolidación de
registros de terminal.

**Herramientas comerciales  
La mayoría de las herramientas comerciales utilizadas para pruebas de penetración o Red Teaming tienen inherentemente algún nivel de
capacidad de registro. Algunas tienen la capacidad de redirigir las salidas de registro a una ubicación específica, mientras que otras
requieren que el operador active la generación de registros. En cualquier caso, se recomienda que estos registros sean
capturados y almacenados en una ubicación como /root/logs/commercial_tool/.

**Herramientas personalizadas**  
Cualquier equipo rojo capaz tendrá herramientas personalizadas generadas para todos los eventos o creadas para un compromiso específico.
compromiso. Estas herramientas deben aprovechar la capacidad de crear registros durante la ejecución. Al crear
Cuando se construyan estas herramientas, el equipo rojo debe considerar la posibilidad de capturar todos los datos requeridos del registro del operador y, muy posiblemente, crear entradas de registro en el proceso.
posiblemente la creación de entradas de registro en el proceso. Cada punto de datos debe ser capturado en el mismo
formato YYYMMDD_HHMM_IP_Description (por ejemplo, 20170308_151312_UTC.terminal.log.raw).

**Consolidación**  
Se recomienda la transferencia diaria de estos registros al repositorio de compromisos. La preferencia debe ser
crear una copia de seguridad o un script de rollup que copie cada conjunto de registros en el repositorio cuando se ejecute al
al final del día.

**Imágenes de pantalla  
Los detalles relativos a las acciones del equipo rojo son a menudo recibidos con incredulidad. Incluso cuando el equipo tiene
de acceso a una aplicación, una red o un área física altamente restringida, el personal
personal del objetivo (tanto de la dirección como de los empleados) a veces tiene problemas para admitir que se ha obtenido el acceso.
acceso. Las imágenes proporcionan la prueba visual que a menudo se necesita.

Las capturas de pantalla de las actividades proporcionan validez a las acciones que se produjeron en una evaluación. Tenga en cuenta que
un compromiso del Equipo Rojo no es una evaluación de vulnerabilidad o una prueba de penetración. El compromiso está
El compromiso está diseñado para "contar una historia" sobre cómo una amenaza legítima podría impactar en el funcionamiento del entorno objetivo.
objetivo. ¿Qué mejor manera de contar esa historia que incluir capturas de pantalla de aplicaciones, sistemas y
comandos en la historia?

Durante las evaluaciones físicas, las imágenes o el vídeo de los edificios, las oficinas, los escritorios, las salas de servidores, las zonas restringidas
áreas restringidas, etc., suelen ser necesarios como prueba de entrada. Una segunda recomendación es que el equipo físico
equipo físico genere pegatinas que contengan el logotipo del Equipo Rojo. Esas pegatinas (o marcadores) se colocan en
áreas de interés y se colocan dentro del marco cuando se capturan imágenes o vídeo.

Recuerda: Un nombre de archivo útil incluye la fecha, la hora, la IP y la descripción en el formato de
AAAAMMDD_HHMM_IP_Descripción.jpg|png (por ejemplo, 20170308_1518_servidor_sala_acceso.png).


### Tradecraft

El término tradecraft está tomado de la comunidad de inteligencia. El diccionario Merriam-Webster.com
define tradecraft como "las técnicas y procedimientos de espionaje". El término tradecraft en el Red Teaming se ha
se ha convertido en un término más general. Es el cómo y el porqué de la actuación de un equipo rojo. Básicamente, el Tradecraft de una amenaza
utiliza varias TTPs para emular una amenaza específica. Para minimizar la confusión, Tradecraft, TTPs y
técnicas se utilizarán indistintamente. Los requisitos de representación de la amenaza afectan directamente a la elección de las TTP por parte del Equipo Rojo.
elección de las TTP de un Equipo Rojo. Un Equipo Rojo puede elegir herramientas personalizadas y muy avanzadas para apoyar una APT (amenaza
(amenaza persistente avanzada) o utilizar técnicas simples de "script kiddie" para emular a un hacker ordinario. Esta gama
obliga a un Equipo Rojo a ser muy diverso. Deben tener la capacidad de emular amenazas muy avanzadas
y de limitarse a una amenaza simple. Recuerde que el Tradecraft y las TTPs son fundamentales para un Equipo Rojo.
Un Tradecraft débil equivale a un Equipo Rojo débil. Un Equipo Rojo debe ser muy capaz para
emular con éxito una amenaza con la fidelidad necesaria para lograr sus objetivos como amenaza.


### Orientación general

Mantener una TTP consistente es esencial durante los compromisos del Equipo Rojo. Quedar atrapado o estimular
un efecto en el momento equivocado del compromiso puede comprometer toda la misión. Orientación sobre las TTPs
"A continuación se incluyen orientaciones sobre lo que se debe y no se debe hacer en los enfrentamientos de los equipos rojos. Estas reglas deben aplicarse siempre
al primer conjunto de procedimientos operativos. Este conjunto de reglas es un gran punto de partida para desarrollar TTPs de alto nivel.
TTPs de alto nivel.

Si las circunstancias exigen una desviación, o si una regla no se ajusta a un compromiso, es necesario consultar con un operador de alto nivel del Equipo Rojo.
Se requiere una consulta con un Operador del Equipo Rojo de alto nivel. Cada vez que se infrinja una norma de TTP, el personal superior debe participar en la decisión y documentar el motivo y las circunstancias.
decisión y documentar la razón y las circunstancias.

#### Registrar todas las acciones significativas (éxitos y fracasos)

Lo más importante es lo siguiente: Registrar, registrar y registrar más. Haz capturas de pantalla de todas las acciones significativas,
incluyendo los intentos exitosos y fallidos.

Uno de los aspectos más importantes de la participación del Equipo Rojo es la recopilación de datos (también conocidos como registros).
Es muy común que un equipo inexperto complete un compromiso con una documentación deficiente.
documentación. Muchas acciones no se capturan en su totalidad, algunas acciones nunca se capturan y, a menudo, los fallos clave se ignoran.
y, a menudo, se ignoran los fallos más importantes. Cada acción realizada aporta valor tanto al objetivo como a los defensores del mismo.
defensores. Los registros incompletos impiden al Equipo Rojo proporcionar una descripción completa y precisa
de las acciones, los obstáculos y las fortalezas y debilidades defensivas del objetivo (es decir, el fracaso de la misión del Equipo Rojo).
fracaso de la misión).  

Como se ha explicado anteriormente, existen varios métodos para garantizar que los registros se capturen y
almacenados:  
```
● Registro automatizado del terminal: Todas las acciones de la terminal se registran, con sello de tiempo, y se guardan en una ubicación predefinida  
● Registros de herramientas: La mayoría de las herramientas comerciales tienen alguna capacidad para registrar las acciones y producir un informe bruto o final  
● Registros de herramientas personalizadas: Si escribes una herramienta/script personalizado, debería emitir un registro de acciones y resultados  
● Registros del operador: Con mucho, estos son los registros más importantes. Un registro puede mostrar la acción
acción realizada y el resultado; sin embargo, sólo el operador puede anotar con precisión la forma en que se realizó la acción
se realizó, lo que les llevó a la decisión, y su interpretación del resultado  
● Capturas de pantalla: Los registros de terminal son excelentes para el operador y aún mejores como artefactos de apoyo;
sin embargo, pueden no significar nada para los ejecutivos de alto nivel (o incluso para algunos profesionales de TI
profesionales de TI). Las capturas de pantalla antes, durante y después de la ejecución de una acción tienen
mucho más peso que un registro de terminal, un registro de herramienta o un registro de operador (a menudo, puede ser sólo una
una captura de pantalla del terminal durante la ejecución)  
```

#### Consultar con los compañeros

No importa cuánto tiempo lleves trabajando en TI o en seguridad, consulta a tus compañeros antes de actuar.
Esto es especialmente cierto durante la explotación y la configuración de Mando y Control. Los errores simples a menudo
errores simples a menudo conducen al descubrimiento del Equipo Rojo demasiado pronto en el compromiso. Fíjate en el siguiente comando. El comando
podría ejecutarse para proporcionar un conocimiento general de la situación en un sistema Linux. ¿Cuál es la salida esperada
salida esperada del siguiente comando?
``netstat -antb``

El comando anterior es un comando netstat que puede ser ejecutado en un host Windows. Linux no tiene
tiene la opción "b" y produce una respuesta de "opción inválida". Piensa en ello:  

¿Has escrito alguna vez ``ifconfig`` en lugar de ipconfig?  
¿Has escrito alguna vez ``rm *`` en el directorio equivocado?  
¿Has introducido alguna vez las credenciales sólo para descubrir que estaban "engordadas" (tras un error de acceso)?  

Aunque se trata de simplificaciones excesivas, representan la necesidad de revisar las herramientas, el C2, la configuración
la ejecución e incluso la limpieza. Los errores pueden llevar a una exposición accidental en un compromiso del Equipo Rojo.
Esto puede causar contratiempos significativos y reducir la calidad de un compromiso.

#### Comprender las herramientas y tecnologías utilizadas

Saber qué funcionalidad ofrece una herramienta es sólo un tercio de la ecuación. Antes de que una nueva herramienta
(script, aplicación, binario, proceso, etc.) se utilice en un sistema de destino, debe probarse, someterse a un
proceso interno de verificación y añadirse a un conjunto oficial de herramientas.  
Entonces, ¿cómo completamos la ecuación? Preguntando:  
```
¿Qué artefactos deja la herramienta?  
¿Se modifica algún archivo durante la ejecución?  
● ¿Hay cuentos en el tráfico de red?  
● ¿Tiene la herramienta impactos negativos en versiones específicas de un sistema operativo? (Funciona bien en
Windows 8 pero provoca un error de sistema en Windows 10)  
● ¿La herramienta intenta ejecutarse como un usuario específico o, peor aún, crea un usuario/grupo?  
● ¿Intenta la herramienta llamar a casa para las actualizaciones?  
        ○ Esto puede desencadenar alertas defensivas que identifiquen a personas o software no autorizados en la red  
```
Piensa en psexec.. ¿Qué es? La respuesta más común se refiere a la herramienta PsExec.exe de SysInternals[13].

¿Qué hace? A alto nivel, ejecuta comandos en el sistema Windows local o remoto.

¿Qué hace en términos de indicadores?
```
● Copia un archivo de servicio en el sistema remoto  
● Introduce una clave de servicio en el Registro   
● Crea un archivo de preconfiguración  
● Crea una entrada en la caché de compatibilidad de aplicaciones  
● Crea un evento de inicio de sesión  
● Crea una carpeta de perfil para el usuario remoto  
● Intenta eliminar el archivo de servicio y la clave al salir (no siempre tiene éxito)  
```
Qué ocurre cuando se utiliza la opción -e? ¿la opción -s?  
¿En qué se diferencia de psexec para PowerShell?  

En resumen, debe entender cómo las herramientas o la técnica interactúan con un objetivo, qué tráfico de red puede generar y qué rastros puede dejar.
puede generar y qué rastros puede dejar. En el caso de psexec, se puede considerar una
técnica de movimiento lateral en lugar de una herramienta específica. Existen múltiples métodos para lograr el
resultado que PsExec.exe proporciona sin la herramienta en sí.

#### Realizar un reconocimiento de la situación

Después de obtener acceso a un sistema o aplicación remota, realice un conocimiento de la situación antes de seguir
seguir adelante.
```
Comprende el entorno en el que te encuentras. (¿Está el objetivo dentro del alcance?)  
● ¿Qué protecciones existen en el sistema o la red?  
● ¿Cuáles son los riesgos de ser atrapado y qué vías de ataque ofrece el sistema?  
● ¿Hay conexiones preestablecidas a otros recursos de la red?  
● ¿Quién está actualmente conectado al sistema?  
● ¿Quién se ha conectado recientemente al sistema?  
```

#### Minimizar el volumen de llamadas de retorno (C2)

A menos que se active un mecanismo de protección basado en el host, es más probable que se descubra o atrape por
un reconocimiento o análisis del tráfico en la red por parte de un defensor. Para evitar la detección temprana sigue un buen
procedimiento comercial para limitar y controlar la cantidad de tráfico generado durante un compromiso. En
Hay varios conceptos generales que, si se siguen, aumentan el éxito del compromiso mientras
disminuyendo las posibilidades de ser descubierto:  
```
Mantener el tráfico interno de la red: Uno de los problemas más comunes, y que debería
siempre intentar cambiar, es el número limitado de sensores dentro de una red. La mayoría de las protecciones de la red
protecciones de la red se aplican actualmente en el límite.
● Pivotar el tráfico de mando y control a un número mínimo de fuentes salientes: Mantener al menos
mantener al menos dos fuentes de salida para la redundancia de C2; sin embargo, utilice sólo una para las operaciones
(considerado un nivel interactivo). La segunda (un nivel de larga o corta distancia) está inactiva o
extremadamente lento y se utiliza como respaldo si/cuando se descubre el primario.
```

#### No utilices canales no encriptados para C2 (a menos que se mezclen con el tráfico de la red)

Los datos de mando y control que salen de la red deben estar cifrados. Un IDS u otra defensa de la red
detectará los datos en texto claro, como la carga de un binario, la emisión de un comando del sistema operativo o el uso de
un shell web. Se ha vuelto común que los IPS/IDSs detecten cadenas específicas descubiertas en el tráfico de texto claro.
en el tráfico de texto claro. Por ejemplo, "C:\Windows\System32" se ha convertido en un disparador común para la investigación.

Algunos defensores incluso han ido más allá al legitimar una amenaza potencial. Supongamos que los defensores
o el personal de TI utiliza regularmente una herramienta de administración remota. Ignorando las recomendaciones, este tráfico está
sin cifrar. En lugar de provocar una alerta cada vez que la herramienta se utiliza legítimamente, la alerta está
configurada para buscar incoherencias en el uso. Por ejemplo, la mayoría de los atacantes están acostumbrados a
escribir comandos en minúsculas en Windows. El defensor ignora "C:\Windows\System32" pero alerta sobre
"c:\windows\system32"

El cifrado interno es otro ejemplo en el que se debe consultar a los compañeros para determinar el mejor
curso de acción antes de desplegar el C2 en una red.

El cifrado del tráfico interno de C2 depende de varios factores diferentes:  
```
● ¿Hay sensores dentro de la red?  
¿Hay otras comunicaciones cifradas entre los sistemas objetivo?  
¿El tráfico encriptado destacaría más que el no encriptado?  
```
#### No intentes explotar o atacar sitios web o aplicaciones no cifradas

Por muy tentador que sea, no ataques sitios web sin cifrar. Los ataques simples pueden activar los IDS.
Conozca siempre su espacio IP de destino. Es probable que haya varios sitios web disponibles para su revisión. Una adecuada
reconocimiento o la coordinación adecuada debería descubrir cada uno de ellos. Cree una lista de sitios en su registro de objetivos.
Incluya direcciones IP, URLs, una conjetura sobre las funciones, puertos, protocolos, etc.

```
Punto de enfoque
Antes de llevar a cabo cualquier explotación y ataque contra un servidor web, consulte sus Reglas de Compromiso y comprenda plenamente
comprender:  
¿Quién es el propietario del sitio web?  
¿Quién es el propietario del sistema en el que está alojado el sitio web?  
● ¿Quién es el propietario de la aplicación back-end?  
● ¿Se han obtenido las aprobaciones adecuadas para las pruebas?  
```

#### No ejecutar desde ubicaciones no ejecutables
```
● La ejecución en un entorno Windows debe producirse en una ubicación típica de Windows
Son comunes las ubicaciones ejecutables como c:\programdata, c:\gam files, y c:\windows\
● La ejecución desde ubicaciones como c:\dows\temp nunca debe ocurrir o ser utilizada con conocimiento del riesgo
```

#### No utilice binarios para las capacidades iniciales

Como regla general, no deje caer binarios en el sistema. Primero, utilice los comandos incorporados para lograr sus
objetivos. Esto no siempre es posible, y los binarios pueden ser necesarios; sin embargo, los binarios **deben** ser investigados
ofuscados, y probados contra la detección antes de su uso.
```
Asegúrese de que todos los binarios cumplen con lo que se debe y no se debe hacer.
Consulte a un operador de alto nivel antes de dejar cualquier binario.
```

#### No descargue conjuntos de datos restringidos

NUNCA descargue (ni retire de la red de destino) ningún conjunto de datos PII, HIPAA, PCI u otros restringidos.
restringidos. Una buena regla general es anotar en el registro el tipo de datos, la ubicación, el método de acceso y el nivel de
acceso a los datos restringidos en el registro.  
```
● Asegúrese de que las notas del registro incluyan una referencia al tipo de datos descubiertos para una referencia rápida  
● Realice una captura de pantalla del nombre del archivo mostrado y su ubicación (suponiendo que el nombre del archivo no tenga datos restringidos incluidos)  
● Hacer una captura de pantalla de una parte del conjunto de datos sin capturar los datos restringidos. El operador puede hacerlo como prueba de acceso.  
● Si el conjunto de datos es preocupante, intente copiar el archivo a un nuevo nombre en la misma ubicación. Esto validará el acceso sin exponer los datos.  
● ¡NO tome capturas de pantalla de los datos en sí!  
```

### Conceptos de ejecución

#### Explotación

La explotación es una técnica que utiliza una amenaza para aprovechar una vulnerabilidad o debilidad. Esto puede ser
debido a un fallo de software o a una mala configuración. A diferencia de las pruebas de penetración, donde la validación de los exploits
contra una vulnerabilidad es un objetivo principal, la explotación no es un objetivo final para los compromisos del Equipo Rojo.
Los exploits no son más que un medio para alcanzar un fin; sin embargo, esto no reduce su importancia. La explotación
puede ser una parte crítica de un compromiso del Equipo Rojo. La explotación debe utilizarse con precaución, ya que muchas
a menudo desencadenan una respuesta Azul. Al igual que con todas las decisiones tomadas durante un compromiso del Equipo Rojo, se debe medir el riesgo en comparación con la recompensa para determinar si el riesgo es mayor.
riesgo frente a la recompensa para determinar si el acceso obtenido de un exploit vale la pena la exposición potencial.
exposición.

Los exploits deben utilizarse para obtener acceso sólo como medio para alcanzar un fin. Una vez que se produce la explotación,
Una vez que se produce la explotación, deben establecerse puertas traseras u otros medios de acceso. El exploit no debe utilizarse como medio
para recuperar el acceso a un objetivo. Por ejemplo, supongamos que existe un defecto conocido de ejecución remota de código en una aplicación web.
aplicación web. Existe un exploit público fácilmente disponible, y el uso de dicho exploit puede activar un dispositivo de seguridad, como un IDS.
de seguridad, como un IDS. Un equipo rojo sopesa el riesgo y decide seguir adelante con el exploit. A
Operador del Equipo Rojo utiliza con éxito el exploit desde un espacio IP quemable. El exploit resulta en
ejecución remota de comandos en el servidor web objetivo. En lugar de utilizar el exploit repetidamente para emitir
comandos, se despliega un shell web. Ahora se puede acceder a este shell web desde una dirección de origen diferente
de origen. De esta manera, el exploit se utiliza sólo una vez. El shell web proporciona una puerta trasera utilizable para
acceder al servidor web para realizar otras acciones.

#### Explotación de vulnerabilidades conocidas

Una amenaza utilizará lo que esté disponible. Al igual que los atacantes reales, los equipos rojos se aprovecharán de una debilidad
para apoyar sus objetivos. Hay una diferencia clave en cómo un Equipo Rojo debe ver y usar un exploit
frente a otros tipos de pruebas de seguridad. En el Red Teaming, los exploits conocidos (incluidos los preempaquetados o "enlatados")
conocidos (incluidos los preempaquetados o "enlatados") sólo deben utilizarse para apoyar directamente un objetivo. Esto significa que un entorno puede tener múltiples
vulnerabilidades explotables que un Red Team no explota. Esto podría deberse a la minimización de la
la detección o al hecho de que la explotación no apoya un objetivo del Equipo Rojo. Es importante recordar
que un compromiso del Equipo Rojo no es una visión completa de las vulnerabilidades de un objetivo.

En resumen, muchos exploits tienen firmas conocidas y pueden ser fácilmente detectados o tienen código que causa
daños o impactos no deseados a un objetivo. Un operador del equipo rojo siempre debe entender el
exploit, su código y conocer sus IOC para gestionar el riesgo de exposición o daño a un objetivo.

Lugares populares para encontrar exploits:  
```
● Metasploit: [http://www.metasploit.com](http://www.metasploit.com) - exploits públicos y zero days  
● ExploitHub: [http://www.exploithub.com](http://www.exploithub.com) - centro de intercambio de exploits comerciales para días no cero  
● Exploit DB: [http://www.exploit-db.com](http://www.exploit-db.com) - repositorio de exploits mantenido por Offensive Security  
● Otros centros de intercambio de exploits  
```

Punto de atención
```
Un entorno objetivo puede tener múltiples vulnerabilidades explotables. Sólo aquellas que permitan cumplir con las metas
y objetivos del compromiso deben ser consideradas para su explotación. Documente todas las vulnerabilidades explotables identificadas
vulnerabilidades identificadas, pero utilice sólo las necesarias para alcanzar los objetivos de la intervención. Tenga siempre en cuenta el riesgo en cada acción que realice.
```
#### Explotación sin exploits

La explotación no siempre requiere un exploit basado en los defectos del código. Los probadores de penetración experimentados
y Red Teamers utilizarán el concepto de _Explotación sin Explotación._ Esta es la idea de explotar
o comprometer un sistema utilizando el diseño, las funciones y la configuración del sistema contra sí mismo. Los controles de seguridad y la mala configuración de
controles de seguridad pobres y configuraciones erróneas a menudo conducen a un compromiso. No sólo puede usar un sistema
contra sí mismo apoyar un compromiso, por lo general implica una menor huella IOC. En muchos casos,
atacar un sistema sin exploits se parece mucho a la misma actividad realizada por un administrador de red.
administrador de la red.

Hay varias técnicas que una amenaza puede utilizar para explotar, comprometer o ganar acceso a un sistema objetivo.
objetivo. No caiga en la trampa de que los exploits enlatados son necesarios para lograr los objetivos. Los exploits pueden ser
raros, costosos y efímeros. Cuando funcionan, son geniales, pero la mayoría de los exploits tienen una vida corta.
Los buenos operadores de equipos rojos exploran y practican regularmente muchos medios de explotación remota o
compromiso. Se trata de un área de seguridad en constante cambio. Es necesario investigar y practicar para mantenerse
actualizados en las técnicas modernas.

**Vulnerabilidad de las aplicaciones web**  
La seguridad ha aumentado a lo largo de los años, y el número de exploits de corrupción de memoria tradicionales ha
ha disminuido significativamente. Esto ha llevado a las amenazas a buscar medios alternativos para acceder a un
objetivo. Las aplicaciones web son excelentes objetivos para la explotación y ejecución remota de código. Aunque las aplicaciones web
Aunque las aplicaciones web existen desde hace años, su seguridad sigue siendo bastante débil e incomprendida.
Esto hace que las aplicaciones web sean las principales puertas de entrada a una red, ya que incluso la aplicación más básica puede
proporcionar una puerta trasera a una amenaza. En resumen, las aplicaciones web son una de las formas más efectivas de obtener
acceso remoto a un entorno.

**Desconfiguración de la seguridad**  
La seguridad ha mejorado a lo largo de los años, y el número de exploits tradicionales de corrupción de memoria ha
ha disminuido significativamente. Esto ha llevado a las amenazas a buscar medios alternativos para obtener acceso a un
objetivo. Las aplicaciones web son excelentes objetivos para la explotación y ejecución remota de código. Aunque las aplicaciones web
Aunque las aplicaciones web han existido durante años, sus defensas de seguridad son todavía bastante débiles y
incomprendidas. Esta incomprensión hace que las aplicaciones web sean las principales puertas de entrada a una red, ya que
incluso la aplicación más básica puede proporcionar una puerta trasera a una amenaza. En resumen, las aplicaciones web pueden ser
una de las formas más eficaces de obtener acceso remoto a un entorno.

Las reglas de seguridad de la red mal configuradas suelen ofrecer múltiples vías para atravesar las amenazas. Cuando los sistemas
pueden comunicarse libremente en una red, pueden intercambiar información rápidamente. Esto incluye el tráfico de una amenaza.
de una amenaza. Es frecuente que una organización configure reglas de tráfico orientadas al exterior y deje abiertas las comunicaciones de la red interna.
las comunicaciones de la red interna. También es común que las credenciales se almacenen en texto claro en
en texto claro en ubicaciones públicas de la red. Estas credenciales pueden ser de usuario o administrativas. De cualquier manera
De cualquier manera, cuando las amenazas utilizan credenciales válidas, se ven y se sienten como si estuvieran dentro de la red. Puede ser muy difícil para un
Equipo Azul distinguir entre una amenaza y un usuario válido. Estas son medidas importantes de
capacidad de las operaciones de seguridad.

**Monitoreo de seguridad deficiente o inexistente**  
La falta de supervisión de la seguridad permite a una amenaza utilizar un conjunto de herramientas más amplio. Las herramientas o técnicas que
pueden ser ruidosas o desencadenar una respuesta pueden funcionar perfectamente en un entorno no supervisado. Este descuido
proporciona a una amenaza una flexibilidad y capacidad mucho mayores. Un equipo rojo puede aprovecharse de una
red no supervisada. Un impacto operativo común es la exfiltración de datos. Quizás una organización objetivo
tiene propiedad intelectual sensible. La exposición de esta información podría dañar significativamente
la organización. Un equipo rojo puede comprobar la capacidad de una amenaza para obtener acceso y exfiltrar los datos. A
La falta de vigilancia puede permitir que la amenaza acceda a los datos y los robe sin ser advertida. Azul
Los equipos azules que tienen un proceso de monitorización de seguridad débil no identificarán el tráfico malicioso o los cambios
realizados por una amenaza. Las herramientas defensivas son excelentes, pero deben ser configuradas y probadas para asegurar que están
funcionan como se espera. Recuerde que el papel principal del Equipo Rojo es facilitar la mejora
de la postura defensiva de una organización.

**Ingeniería social (SE)**  
La ingeniería social consiste en explotar las debilidades de la naturaleza humana. Los compromisos del Equipo Rojo a menudo se basan en
ingeniería social para apoyar los objetivos. Esto se utiliza típicamente en las siguientes áreas:

Phishing  
```
● Envío de un correo electrónico para atraer a un usuario final para que proporcione información sensible o para entregar una carga útil  
● Puede utilizarse para entregar una carga útil maliciosa  
● Puede utilizarse para facilitar la SE en persona  
● Puede utilizarse para facilitar el acceso físico  
```

Teléfono/texto  
```
● Llamar o enviar mensajes de texto para incitar a un usuario final a proporcionar información sensible  
● Puede utilizarse para facilitar tanto el phishing como el SE en persona  
● Puede utilizarse para facilitar el acceso físico  
```

Pretexto en persona  
```
● La ingeniería social en persona se suele utilizar para apoyar una brecha física  
```

**Precaución**  
La ingeniería social (especialmente el Phishing) funciona, punto. Pero no siempre es la mejor opción. Hay
existen riesgos políticos asociados a la SE de un usuario. Por ejemplo, las campañas de Phishing que funcionan bien pueden
acosar o incluso avergonzar a los usuarios finales. Tenga cuidado al crear una campaña de phishing. Muchos objetivos de
phishing requieren que la campaña sea aprobada antes de enviar los correos electrónicos. Esto puede proteger a la
organización, pero también puede limitar la tasa de éxito de un phishing. En los casos en los que el phishing es arriesgado, considere
el "white carding". Una estrategia sólida consiste en enviar un correo electrónico de phishing a una persona de confianza. Esa persona hará clic en
enlaces o proporcionará información según las indicaciones del phishing. Esto permite que la carga útil del phishing se entregue
de una manera políticamente segura mientras se permite que el correo electrónico de phishing toque todas las defensas de seguridad. Este modelo
modelo utiliza la suposición de que un usuario sucumbirá a un ataque de phishing. El reto para el Red
Team es eludir las protecciones de seguridad diseñadas para proteger a los usuarios de sí mismos.

Un phishing que lleve a comprometer un solo sistema puede ser aceptable. Un phishing que lleve a comprometer una organización no es aceptable.
organización no es aceptable, ya que deben producirse múltiples fallos en los controles de la organización (técnicos, políticos, de procedimiento).
controles organizativos (técnicos, de política, de procedimiento, etc.). Los autores son conscientes de que estas
Los autores son conscientes de que estas afirmaciones son controvertidas y proporcionan los siguientes conceptos para la reflexión.  

Considere lo siguiente
```
Un ataque de phishing que lleve a un compromiso organizativo no es
NO es culpa de un usuario final. En su lugar, es la insuficiencia de
controles de seguridad de un entorno objetivo.
```

Como se ha señalado anteriormente, la ingeniería social simplemente funciona. Los usuarios suelen recibir muchos tipos diferentes de
formación sobre ingeniería social, phishing, seguridad de la información, seguridad operativa, etc.; sin embargo, un
Sin embargo, un phishing bien investigado, construido y dirigido tendrá éxito en la mayoría de los escenarios. Esta idea ha sido
Esta idea ha sido probada varias veces por múltiples profesionales con múltiples escritos sobre técnicas y
éxitos. Un phish bien planificado evita los indicadores comunes de phishing, no alerta al usuario de
intención maliciosa, y en última instancia puede proporcionar acceso a la amenaza al sistema del usuario final. Combinado con una
combinado con el uso efectivo de una amenaza de buen oficio, el usuario no tiene "indicadores de maldad". En este punto, la responsabilidad del usuario
responsabilidad del usuario. Todo lo que vaya más allá (y podría decirse que incluye) del compromiso inicial del sistema del usuario final es responsabilidad del usuario.
del sistema del usuario final es responsabilidad de la organización. A todos los efectos, la amenaza se ha
se ha convertido en una persona interna lógica. Si la amenaza tiene la capacidad de moverse lateralmente por la red,
elevar los privilegios, acceder a información sensible, exfiltrar datos o causar un impacto operativo; también lo hacen
otros usuarios (quizás todos) de la organización. Es probable que simplemente no sepan cómo hacerlo.


### Herramientas y ejemplos de herramientas

Un Equipo Rojo puede y debe utilizar cualquier herramienta que apoye sus objetivos finales. Aunque muchos Equipos Rojos utilizan
las mismas herramientas utilizadas por los probadores de penetración, esto no significa que las herramientas se empleen igual o se elijan
sin cuidado. Un equipo debe comprender las capacidades y los límites de una herramienta. El equipo debe tener la
capacidad de controlar o ajustar una herramienta para que se adapte a las necesidades de un compromiso; no sólo en cuanto a la capacidad técnica sino
también la capacidad de ajustar una herramienta para modelar una amenaza específica. La elección de las herramientas puede llevar a un desarrollo
de herramientas comerciales, o el simple uso de los comandos integrados en el sistema operativo.
del sistema operativo. Al final, el conjunto de herramientas se elige en función de los objetivos de un Equipo Rojo.

La forma en que un Equipo Rojo utiliza las herramientas de seguridad comunes puede ser muy diferente a la de otros probadores de seguridad.
seguridad. Un Equipo Rojo a menudo necesita personalizar el código para asegurarse de que funciona de una manera específica o
cambiar los indicadores que puede dejar una herramienta. Como mínimo, un buen operador debe entender cómo funciona una
herramienta y qué impacto o riesgo se introduce en un compromiso. Los buenos operadores del Equipo Rojo
mantienen el control sobre sus acciones. Esto incluye cómo, cuándo y si se utiliza una herramienta.

Esta sección se refiere a muchas herramientas comunes utilizadas en la comunidad de seguridad. Muchas de estas herramientas son
Muchas de estas herramientas son antiguas o no son apropiadas para los compromisos modernos de los equipos rojos. El propósito de la discusión es
proporcionar un contexto en el Red Teaming.

#### Escáneres de vulnerabilidad

Los equipos rojos no suelen utilizar escáneres de vulnerabilidad. Estas herramientas generalmente tienden a ser ruidosas y a
generar una enorme cantidad de tráfico. La identificación de vulnerabilidades por parte de un Red Team se centra en
OSINT, enumeración baja y lenta, adivinación inteligente u otros métodos no intrusivos. Hay
casos en los que los escáneres de vulnerabilidad son útiles. Por ejemplo, un Equipo Rojo ha identificado una aplicación web
aplicación construida en Joomla con rutas hacia los objetivos de un Equipo Rojo. Les gustaría saber si la versión
de Joomla es vulnerable. Se podría emplear un escáner de vulnerabilidad estándar, pero esto podría ser
excesivo para una sola aplicación. En su lugar, el equipo puede ajustar un escáner de vulnerabilidad para comprobar un
pequeño conjunto de defectos basados en Joomla. El uso de un escáner enfocado minimizaría la exposición. También podrían
extraer manualmente la información de la versión de la aplicación web. En cualquier caso, se debe tener precaución
antes de ejecutar un escáner de vulnerabilidades para reducir la exposición. Si se necesita un escaneo más intrusivo
realizar el escaneo desde una fuente quemable que se dedique a actividades más ruidosas protegería más
fuentes sensibles de ser expuestas.

Al final, la elección de cuándo o cómo utilizar un escáner de vulnerabilidad viene dada por el riesgo. Piensa en lo siguiente
siguiente antes de ejecutar un escáner de vulnerabilidad:  
```
● ¿El riesgo de exposición por ejecutar una herramienta generalmente ruidosa supera el potencial conocimiento aprendido?  
● ¿Hay otras formas de identificar una vulnerabilidad sin usar el escáner automatizado?  
● ¿La explotación de una vulnerabilidad proporcionará un camino beneficioso para el objetivo de un Equipo Rojo?
(Recuerde que la identificación de la vulnerabilidad no es típicamente un objetivo de compromiso del Equipo Rojo).  
```

Recuerde esto
```
Sólo porque un objetivo sea vulnerable, no significa que deba ser explotado.
```
#### NMAP y el escaneo de la red

Nmap[14] es una herramienta fundamental para los probadores de penetración y los analistas de seguridad. Fue escrito y es mantenido

por Fyodor[15]. Nmap se utiliza a menudo como un escáner de puertos para determinar el estado de los puertos TCP y UDP en un
en un sistema objetivo. La herramienta no es un simple escáner de puertos, sino una herramienta de enumeración de red muy capaz
que permite una gran variedad de técnicas de enumeración. Se puede ampliar mediante el uso de NSE
(Nmap Scripting Engine). Según la documentación de Nmap, el Nmap Scripting Engine
(NSE) es una de las características más potentes de Nmap. Permite a los usuarios escribir (y compartir) scripts sencillos para
automatizar una amplia variedad de tareas de red. Los scripts de NSE son extremadamente útiles. Pueden utilizarse para
enumerar un sistema para obtener información o para identificar vulnerabilidades.

En resumen, Nmap puede utilizarse para una simple enumeración o para un escaneo de vulnerabilidades en profundidad. Su flexibilidad
y potencia permiten una gran flexibilidad y capacidad para enumerar un objetivo; sin embargo, esta
potencia puede ser un arma de doble filo. Nmap no está diseñado necesariamente para ser sigiloso, sino para ser muy
capaz. Un operador del Equipo Rojo debe entender qué indicadores se están generando al utilizar
las distintas capacidades de Nmap. Este texto no profundizará en la herramienta Nmap, sino que cubrirá
algunos usos básicos para destacar un caso de uso cotidiano para un Equipo Rojo. Estos conceptos se aplican a varias
herramientas. Se habla de Nmap debido a su popularidad y al uso de las pruebas de seguridad en general.

Veamos un comando de Nmap con varias opciones

```
Nmap -sT -T2 -n -Pn -oA <fecha/hora_objetivo> -p 80,443,8080 10.10.10.1-100
```
Aquí está el desglose de los argumentos del comando:

-sT  
```
● Esto obliga a Nmap a realizar un escaneo de conexión completo. El valor por defecto de Nmap es -sS, o un escaneo sigiloso. A
análisis completo completa el handshake TCP (SYN, SYN/ACK, ACK) y envía un (RST) para
para interrumpir la conexión. Un escaneo -sS envía sólo SYN y espera una respuesta
o un tiempo de espera. No se establece una conexión completa. Aunque se utiliza el término "stealth", este
comportamiento puede indicar que se está ejecutando un escaneo contra un objetivo. En general, los escaneos de conexión completa
producen menos disparos a través de los dispositivos de seguridad de la red. Esto es especialmente cierto cuando
se ejecutan muy lentamente.  
```
-T2  
```
● Se trata de una plantilla de temporización de Nmap. Van de 0 a 5. Los nombres de las plantillas son paranoico
(0), sneaky (1), polite (2), normal (3), aggressive (4), y insane (5).  
Según los documentos de Nmap, "aunque -T0 y -T1 pueden ser útiles para evitar las alertas de IDS
tardarán un tiempo extraordinariamente largo en escanear miles de máquinas o puertos.
Para un escaneo tan largo, puede preferir establecer los valores de tiempo exactos que necesita en lugar de confiar en
en los valores enlatados -T0 y -T1".  
● La conclusión: controlar la velocidad de un escaneo para equilibrar la recopilación de información con
el envío de paquetes demasiado rápido.  
● Nmap tiene muchas otras opciones de control de tiempo. Consulte el documento de ayuda para más detalles.  
```
-Pn
```
● Tratar todos los hosts como si estuvieran en línea: omitir el descubrimiento de hosts.  
● Esto desactiva las pruebas por defecto que Nmap utiliza para descubrir si un host está en línea.  
● Si no se dan opciones de descubrimiento de hosts, Nmap envía una solicitud de eco ICMP, un paquete TCP SYN
al puerto 443, un paquete TCP ACK al puerto 80 y una solicitud de marca de tiempo ICMP. (Para
IPv6, la solicitud de sello de tiempo ICMP se omite, porque no es parte de ICMPv6). Estos valores predeterminados de
valores predeterminados son equivalentes a las opciones -PE -PS443 -PA80 -PP.  
● Para las máquinas en una red Ethernet local, se seguirá realizando el escaneo ARP (a menos que --
disable-arp-ping o --send-ip), porque Nmap necesita las direcciones MAC para
escanear los equipos de destino. En versiones anteriores de Nmap, -Pn era -P0 y -PN.  
```
-n
```
● No hacer nunca la resolución de DNS.  
● Esto se recomienda por defecto. Si los servidores DNS son públicos, esto no es tan
problema. Si se utilizan los servidores DNS de un objetivo, el envío de consultas DNS para realizar un escaneo de puertos
puede considerarse innecesario.  
```
-oA
```
● Salida en tres formatos (normal, greppable y xml).  
● La recopilación de datos es extremadamente importante durante un compromiso del Equipo Rojo. El uso de la función incorporada de Nmap 
permite que los resultados sean capturados y potencialmente analizados por otras herramientas.  
```
-p
```
● Los puertos a escanear.  
● Establecer los puertos específicos es una buena práctica. Utilizar el valor predeterminado de Nmap puede ser útil para encontrar
servicios desconocidos, pero una suposición intelectual del objetivo puede ayudar a encontrar servicios específicos.  
● Si está buscando servidores web, elija los puertos que probablemente estén asociados con
su objetivo. La OSINT y el reconocimiento previo a un escaneo ayudarán a determinar los puertos apropiados para enumerar.
```

Tenga en cuenta que incluso con estas sugerencias, hay situaciones en las que el sigilo o la tolerancia al riesgo son menos
importante. Quizás esté utilizando Nmap para activar una respuesta Blue. Un escaneo ruidoso puede ser necesario para obtener
información para acceder a un objetivo. En cualquier caso, un Equipo Rojo debe controlar sus COIs y gestionar su
riesgo de exposición para cumplir con los objetivos de un compromiso. Entender y controlar las herramientas del Equipo Rojo es
la clave de esta sección. Este ejemplo es sólo un pequeño vistazo a Nmap. Nmap ofrece numerosos
métodos para controlar su tráfico. Consulte la documentación en https://nmap.org/docs.html para más detalles.

#### Metasploit

El marco de trabajo Metasploit[16] es un marco de trabajo de explotación gratuito y de código abierto creado inicialmente por HD
Moore en 2003. Esta herramienta se ha convertido en un activo fundamental para los probadores de seguridad de todo tipo debido a su enorme
flexibilidad y capacidad. Metasploit incluye varias colecciones de exploits, cargas útiles, módulos auxiliares
auxiliares y módulos de post-explotación. Metasploit es un gran marco de explotación. El exploit,
enumeración, y las capacidades de post-explotación pueden proporcionar a un equipo una gran cantidad de capacidades.
Aunque Metasploit es un gran recurso, hay que tener cuidado cuando se utiliza el Meterpreter
de Metasploit. Meterpreter no es una mala elección de carga útil para el Comando y Control, pero como cualquier herramienta, debe
ser entendida y ajustada adecuadamente antes de su uso. Esta herramienta ha sido examinada y analizada en gran
profundidad. Esto ha dado lugar a un conjunto de herramientas muy capaz, pero puede ser perfilado e identificado por un competente
equipo de seguridad.

Pros y contras de Meterpreter  
PROS  
```
● Tremenda cantidad de capacidad y flexibilidad  
● Gran base de colaboradores  
● Gran selección de módulos de post-explotación  
● Fácil de usar  
● Estable  
```

CONS
```
● Comunicación sincrónica.  
● COIs bien conocidos. (Es necesario modificar el código fuente para minimizarlos).
```
Msfconsole puede ser ajustado usando archivos de recursos. Los archivos de recursos son simplemente un conjunto de msfconsole
guardados en un script. Si los scripts se guardan en ~/.msf4/msfconsole.rc
Algunas configuraciones recomendadas de msfconsole para tener en cuenta:

```
~/.msf4/msfconsole.rc  
spool /root/.msf4/spool.log  
setg ConsoleLogging true  
setg verbose true  
setg LogLevel 5  
setg SessionLogging true  
setg TimestampOutput true  
setg PromptTimeFormat %Y%m%d.%H%M%S%z  
setg PROMPT %T S:%S J:%J  
setg ExitOnSession false  
setg DisableCourtesyShell true  
cargar sonidos #opcional  
```

Estos ajustes configurarán el registro de la consola, aumentarán la verbosidad del registro, habilitarán el registro de la sesión
estandarizar la marca de tiempo, añadir información al prompt de la consola, establecer exitonsession para evitar que los oyentes
para evitar que los oyentes mueran, desactivar el shell de cortesía y cargar sonidos. Los sonidos son opcionales pero pueden ser útiles
indicadores cuando la consola no está siendo monitoreada en tiempo real. Este es un pequeño conjunto de ajustes de configuración de Metasploit
msfconsole. Hay veces en que el código fuente de Metasploit necesitará ser
modificado para controlar el flujo de ataque o gestionar los IOCs.

En términos de dónde encaja el marco metasploit en el Red Teaming, es útil para proporcionar una biblioteca de
exploits, pero generalmente no es apropiado para el comando y control.

#### Web Shells

Una shell web es un código del lado del servidor que actúa como una "shell", herramienta de administración remota o panel de control
permitiendo a un usuario emitir comandos remotos para ser ejecutados por un servidor web. Quien controla la web
shell tiene la capacidad de ejecutar comandos del sistema operativo en el servidor web de destino. La explotación
explotación de una aplicación web es necesaria para desplegar una shell web. Las web shells pueden ser escritas en cualquier
lenguaje web, como PHP, ASP, ASPX, Perl, Ruby, Python, JSP, Java, etc.

**Ejemplos de Web Shell  
```
● China Chopper - Una pequeña shell web repleta de características. Tiene varias características de Comando y
Control características, incluyendo una capacidad de fuerza bruta de la contraseña  
● WSO - Significa "web shell by orb" y tiene la capacidad de hacerse pasar por una página de error
que contiene un formulario de inicio de sesión oculto  
● C99 - Una versión del shell WSO con funcionalidad adicional. Puede mostrar las medidas de seguridad del servidor
medidas de seguridad del servidor y contiene una función de auto-borrado  
● B374K - Un shell web basado en PHP con funcionalidades comunes como la visualización de procesos
y ejecutar comandos  
```

Por qué una amenaza utilizaría una shell web? Los fallos de ejecución remota de código son limitados y han forzado el
uso intensivo de la explotación del cliente; sin embargo, las aplicaciones web siguen siendo puertas muy valiosas en una
Sin embargo, las aplicaciones web siguen siendo puertas muy valiosas para entrar en una red, y comprometer directamente una red a través de medios remotos proporciona muchas opciones a una amenaza.
Las aplicaciones web suelen pasarse por alto, están mal configuradas y están plagadas de fallos. Ejecutar
comandos del sistema operativo con una herramienta bajo demanda es una solución perfecta de largo recorrido y, por tanto, un
objetivo perfecto para un Equipo Rojo.  

Un Equipo Rojo debe ser consciente de los COIs comunes generados por el despliegue de un shell web:  
```
● La explotación de un defecto de la aplicación web debe ocurrir  
        ○ La superficie de ataque del servidor se limita a fallos de carga de archivos, fallos de RFI o fallos de seguridad de la aplicación    
        ○ Esto puede desencadenar una alerta dependiendo del tipo de explotación o defecto  
● Se añadirán o modificarán los archivos del servidor web  
        ○ Se producirá la modificación del código fuente o la modificación directa del código fuente de una aplicación  
        ○ La supervisión de la integridad puede alertar a las defensas de estos cambios  
```
Aunque las vulnerabilidades requeridas para el despliegue del shell web comprenden un pequeño subconjunto de
seguridad de las aplicaciones, vale la pena perseguir esos caminos como una amenaza.

Las web shells son grandes herramientas, pero tienen límites. Los comandos del sistema operativo ejecutados en el
están en el contexto del usuario del servicio web. Si el objetivo ha seguido las mejores prácticas de seguridad, el
servicio se ejecutará como no privilegiado. Esto puede limitar seriamente la capacidad de una shell web. Un operador de
Un operador puede necesitar credenciales adicionales o más explotación para emitir comandos con los permisos adecuados.
permisos. Incluso en el caso de un uso limitado, las web shells a menudo pueden seguir siendo utilizadas como puntos de giro. Otras
limitaciones dependen de la comunicación del servidor web con otros sistemas de destino. Las web shells pueden
tener acceso limitado a los servidores internos. Los servidores web en una DMZ o en una ubicación externa pueden requerir
pivotar a través de múltiples servidores para comunicarse con los sistemas internos de destino. En cualquier caso, el
mantenimiento de un sólido conjunto de herramientas que incluya shells web permite a un Equipo Rojo ser flexible, lo que
aumenta su capacidad.


### Mando y control (C2)

El Mando y Control (C2) es la piedra angular de la capacidad de un Equipo Rojo para controlar y mantener el control
de un objetivo. El C2 es la influencia que un atacante tiene sobre un sistema informático comprometido. Esta influencia se
Esta influencia se expresa mediante una infraestructura C2 que puede emitir diversas tareas e instrucciones al sistema remoto.

Herramientas como PowerShell Empire o Cobalt Strike proporcionan agentes o balizas que pueden desplegarse en
un objetivo. Estas herramientas utilizan un medio de comunicación asíncrono. Un agente o baliza sondea un servidor C2
para obtener instrucciones en un intervalo controlado. El servidor es consultado por una tarea. Si existe una tarea, el
Si existe una tarea, el agente o la baliza realiza la acción e informa de los resultados. Si no hay tareas, el agente o la baliza
pasa a "dormir" durante el periodo de tiempo predefinido.

Los C2 se dividen en tres categorías.

```
● Sincrónico
● Asíncrono
● A la carta
```
El C2 sincrónico funciona en tiempo real. Se requiere un flujo constante de comunicaciones para mantener
el canal C2. Las comunicaciones C2 asíncronas ofrecen muchas ventajas a un Equipo Rojo sobre
las comunicaciones síncronas por:  
```
● Controlar cuándo y con qué frecuencia se envían las comunicaciones - Un agente C2 puede sondear tan rápido
como casi en tiempo real o puede consultar una vez al día, a la semana o al mes  
● Evitar los cortafuegos a través de la comunicación de salida - Los clientes normalmente no son accesibles
desde fuera de una red, pero pueden llegar a los activos en Internet a través de la comunicación de salida  
● No requieren una conexión constante y establecida  
```

El C2 bajo demanda es único y opera sólo cuando se necesita. Las comunicaciones se producen sólo cuando son activadas
por un operador. Herramientas como el correo electrónico o los shells web pueden proporcionar excelentes canales de C2 a la carta.
La elección de los mecanismos de mando y control (C2) es un paso fundamental en el diseño del plan C2
para un compromiso.

#### Canales C2  

Existen numerosos métodos para establecer el C2. Cada uno de estos métodos utiliza un Canal C2 para las comunicaciones primarias.
comunicaciones primarias. Aunque se puede utilizar cualquier canal, se recomienda utilizar un canal que se integre
con el tráfico de la organización. Los canales C2 más utilizados son:  
```
● HTTP/HTTPS  
● DNS  
● SMB  
● SSH  
```

![Alt Image](./Images/18.png)

#### Establecimiento de una infraestructura C2  

Un plan C2 bien pensado y diseñado puede marcar la diferencia entre un compromiso exitoso o fallido.
compromiso. El entorno C2 es el corazón y la línea de vida de todas las comunicaciones de amenaza.

Como parte de la creación y el mantenimiento de una infraestructura para sus operaciones de Equipo Rojo, necesitará lo siguiente
lo siguiente, como mínimo:

```
● Una variedad de nombres de dominio -preferiblemente sitios .com, .net y .org relacionados con la(s) organización(es) que se están evaluando  
        ○ Asegurarse de que los dominios están correctamente categorizados (BlueCoat, WebPulse, OpenDNS, PhishTank)  
        ○ Utilizar dominios de nivel superior (TLD) comunes a su área o uso objetivo  
● Certificados SSL válidos para esos dominios  
● Servidores con acceso a Internet (VPS o físicos)  
        ○ Separados para la suplantación de identidad, la redirección y los servidores C2  
● Plataformas C2 instaladas y configuradas.  
```

Para más información, la información detallada del diseño C2 es mantenida regularmente por Jeff Dimmock @bluescreenofjeff[17]) se puede encontrar en lo siguiente:  
```
● Designing Effective Covert Red Team Attack Infrastructure - ttps://bluescreenofjeff.com/2017-12-05-designing-effective-covert-red-team-attack-infrastructure/#references  
● Wiki de la infraestructura del equipo rojo - https://github.com/bluscreenofjeff/Red-Team-Infrastructure-Wiki
```

#### Herramientas C2

Aunque los Equipos Rojos utilizan herramientas de seguridad ofensivas similares a las de los probadores de penetración, hay herramientas
más enfatizadas por los Equipos Rojos-específicamente, cuando se trata de Mando y Control. Mientras que otros
de seguridad pueden utilizar herramientas de Mando y Control, los objetivos de un Equipo Rojo son típicamente
dependen en gran medida de una sólida infraestructura y conjunto de herramientas C2.

Algunos de los conjuntos de herramientas C2 más populares han sido Cobalt Strike, PowerShell Empire y Metasploit.
Todas las herramientas comparten un fuerte énfasis en el apoyo a la post-explotación. Aunque las herramientas pueden tener una
Aunque las herramientas pueden tener una capacidad de explotación, un Equipo Rojo se centra en su uso para la post-explotación y el uso de C2 para la
duración necesaria.

```
2019, el año del C2  
En el año 2019 y sus alrededores, se produjo un enorme crecimiento en el número de marcos C2. Docenas de marcos C2
se lanzaron o se actualizaron seriamente. Este aumento proporcionó nuevas opciones a los equipos rojos al ofrecer
nuevos protocolos, más soporte multiplataforma y nuevas interfaces de perador.
```

**CobaltStrike[18]**  
```
● Software comercial de Strategic Cyber, LLC.  
● La carga útil de mando y control se conoce como baliza.  
● Un proyecto anterior, Armitage, es una herramienta gratuita de Raphael Mudge. A menudo se confunde con la versión gratuita de Cobalt Strike, pero tiene una base de código muy diferente  
● Se describe como "Cobalt Strike es un software para simulaciones de adversarios y peraciones del equipo rojo".  
● Soporta la comunicación C2 asíncrona y síncrona.  
```

**Empire[19]**  
```
● Software de código abierto  
● La carga útil de mando y control se conoce como agente  
● Descrito como "Empire es un agente de post-explotación puro de PowerShell construido sobre comunicaciones ryptológicamente seguras y una arquitectura flexible."  
● Admite la comunicación C2 asíncrona y síncrona.  
● Se retira oficialmente como proyecto en 2019  
```

![Alt Image](./Images/19.png)

Tweet anunciando el etirement de Empire

**Metasploit**
```
● El software de código abierto y comercial es mantenido por Rapid7  
● Marco de pruebas de penetración y explotación de gran capacidad con algún soporte de post-explotación de Red Team  
● La carga útil de mando y control se conoce como Meterpreter  
● La comunicación es generalmente sincrónica  
```

**Otros C2**  
Cobalt Strike, Empire y Metasploit son simplemente tres ejemplos de C2 seleccionados por ser comúnmente
conocidos y ampliamente utilizados. En 2018 y 2019 numerosas herramientas y marcos de trabajo para el comando y control
fueron anunciados y lanzados. Es probable que esta tendencia continúe en los próximos años. Si la construcción de un marco C2
no es posible dado el tiempo o el presupuesto del equipo, los autores recomiendan una simple búsqueda de
de marcos potenciales, probar cada uno de ellos y seleccionar el marco o marcos que mejor satisfagan la necesidad del
necesidad del esfuerzo actual.

#### Redirectores C2  
Los redirectores C2 son pivotes diseñados para separar las comunicaciones entre un objetivo y los servidores C2.
Están diseñados para proteger las direcciones IP de los servidores C2 de la identificación. Los redirectores son lo que
el objetivo verá como maliciosos. El objetivo puede observar cualquier dirección IP o nombre de dominio asociado
con un redirector. Si un defensor identifica actividad maliciosa, puede bloquear una dirección IP de redirector.
Los redirectores deben ser tratados como quemables. Si se queman, un operador del equipo rojo puede simplemente cambiar a un
redirector alternativo para pivotar el tráfico C2 desde el objetivo hasta el servidor C2.

Los redirectores y los servidores C2 deben estar protegidos. Los servidores de mando y control deben comunicarse con
el objetivo a través del canal C2, como HTTPS en el puerto 443. Deben realizarse esfuerzos para limitar (o eliminar) las conexiones C2
desde redes inesperadas; sin embargo, ésta no es la única comunicación con un servidor C2
servidor C2. Un operador debe utilizar la interfaz C2 para controlar el servidor y emitir comandos. Esto debe
también estar protegido. Deben establecerse ACLs u otras protecciones sólo para permitir el acceso de los operadores del Equipo Rojo.
Operadores del Equipo Rojo. Un Equipo Rojo responsable no debe permitir el control del C2 fuera de las IPs/Segmentos designados del Equipo Rojo.
IPs/Segmentos designados. Incluso el software "hacker" no es seguro.

Teniendo en cuenta este pensamiento, los controles de seguridad y acceso adecuados limitan efectivamente el riesgo de nuevas
vulnerabilidades o métodos de acceso desconocidos en las herramientas de Red Team. Por ejemplo, en septiembre de 2016 se encontró un
fallo de ejecución remota de código en Cobalt Strike 3.5. Este fallo permitía la ejecución remota de código
en el servidor C2 a través de una baliza maliciosa. Los controles de acceso efectivos, si se emplean, limitan significativamente
la probabilidad de compromiso desde cualquier red que no sea el Equipo Rojo, el redirector o el objetivo.

Los servicios privados virtuales como Amazon EC2, Digital Ocean y Linode son excelentes soluciones para crear
redirectores accesibles desde Internet. Los servidores de redirección pueden desplegarse o desmontarse fácilmente. La mayoría de los proveedores de servicios de
proveedores de servicios ofrecen una API que permite el despliegue y la destrucción de redirectores para ser
automatizados. Los redirectores pueden hacerse muy resistentes a la eliminación o estar aún más
ofuscado. Técnicas como el Domain Fronting[20] se aprovechan de la confianza en las CDNs de alta confianza.
Un proxy HTTP inverso, como el mod_rewrite de Apache, puede utilizarse para ajustar el tráfico HTTP para ofuscar
mejor u ocultar el tráfico malicioso.

Despliegue de redirectores  
Hay varias formas de redirigir el tráfico. Aquí hay un par de ejemplos rápidos para Linux y
redirectores "dumb pipe" de Windows. Un redireccionador dumb pipe es el proceso de redirigir el tráfico de un
puerto TCP a otro.

Linux:  
Cree un trabajo cron para iniciar un script socat que redirija TCP 443 desde el redirector a 10.10.10.10:
```
crontab -e
@reboot /usr/bin/socat TCP-LISTEN:443,fork / TCP:10.10.10.10:443 &
```

Windows:  
Utilice el comando netsh para crear una regla de redirección de puertos persistente que redirija TCP 443 del edirector a 10.10.10.10:  
```
netsh interface portproxy add v4tov4 listenport=443 listenaddress=10.20.20.20
connectport=443 connectaddress=10.10.10.10
```

Hay varios métodos y técnicas para la redirección. Los ejemplos de este libro se centran en
exponer la necesidad de que los redirectores sean críticos para un compromiso. Los operadores del Equipo Rojo deben incluir un
conjunto de procesos y enfoques técnicos en la caja de herramientas del Equipo Rojo.

#### Niveles C2

El diseño de una infraestructura C2 robusta implica la creación de múltiples niveles de Mando y Control.
Estos pueden describirse como niveles. Cada nivel ofrece un nivel de capacidad y cobertura. La idea de
La idea de utilizar varios niveles es la misma que la de no poner todos los huevos en la misma cesta. Si el C2 es detectado y
Si el C2 es detectado y bloqueado, tener una copia de seguridad permitirá que las operaciones continúen. Los niveles de C2 generalmente se dividen en tres
categorías: Interactivo, de corto recorrido y de largo recorrido. A veces se etiquetan como nivel 1, 2 o 3.
No hay nada único en cada nivel, aparte de cómo se utilizan, y el despliegue de redirectores es
independiente del nivel C2.

Las reglas generales para mantener varios niveles son:  
```
● Mantener la disciplina en cada nivel, y utilizarlo sólo para su propósito previsto  
● Sólo pasar o establecer nuevas sesiones hacia abajo.  
        ○ Los trayectos largos sólo pueden pasar a los trayectos cortos o a los interactivos  
        ○ Corto puede pasar a Interactivo  
        ○ Interactivo puede pasar sólo a otras sesiones interactivas  
● Para cada nivel, utilice un perfil diferente: tipo de comunicación, puertos, protocolos, tiempos de devolución de llamadas, etc.
```

Disminuir el tiempo de devolución de llamada cuando no está en uso
Por supuesto, hay excepciones a estas reglas. Un equipo rojo debe ser flexible para lograr sus objetivos. Si una regla
se viola, hay que ser consciente de los riesgos de exposición antes de realizar una acción. Por ejemplo, digamos que un servidor Long
Haul muere después de haberse establecido inicialmente. Es posible que se necesite un nivel corto o interactivo para
restablecer el Long Haul.

Niveles y sus usos:  

**Interactivo (Nivel 3)**  
```
● Se utiliza para comandos generales, enumeración, escaneo, exfiltración de datos, etc.  
● Este nivel tiene la mayor interacción y corre el mayor riesgo de exposición  
● Planea perder el acceso por un fallo de comunicación, un fallo del agente o acciones del Equipo Azul  
● Ejecute suficientes sesiones interactivas para mantener el acceso (Aunque sea interactivo, esto no significa
bombardear al cliente con paquetes). Utilizar el buen juicio para minimizar la interacción a lo justo para
realizar una acción  
```

**Corto recorrido (Nivel 2)**  
```
● Se utiliza como respaldo para restablecer las sesiones interactivas.  
● Utiliza comunicaciones encubiertas que se mezclan con el objetivo.  
● Tiempos de devolución de llamadas lentos. Los tiempos de devolución de llamadas en el rango de 12 a 24 horas son comunes.  
```

**Largo recorrido (Nivel 1)** 
```
● Se utiliza para restablecer el C2 de corta distancia.  
● Tiempos de devolución de llamada lentos. Los tiempos de devolución de llamada de más de 24 horas (a menudo unos días) son comunes.  
```

**Reglas de la infraestructura C2  
```
● Los servidores C2 no se comunican directamente con los objetivos  
● Los objetivos y los servidores C2 se comunican a través de un redirector  
● Los niveles deben utilizarse para los fines previstos  
        ○ Nivel 1 - Bajo y lento, destinado a la persistencia a largo plazo  
        ○ Tier 2 - Comunicaciones de velocidad media, destinadas a restablecer el C2 interactivo  
        ○ Nivel 3 - Un nivel interactivo diseñado para realizar comandos cotidianos casi en tiempo real o según las necesidades operativas  
        ○ El nuevo C2 debe permanecer en el mismo nivel o inferior (nunca superior):  
                ■ Tier 1 - Tier1 o Tier 2  
                ■ Nivel 2 - Nivel 2 o Nivel 3  
                ■ Tier 3 - Tier 3  
```
**¿Cuándo se puede infringir una norma?**  
El único momento en el que se pasa el C2 es cuando se establece inicialmente el C2. Se puede utilizar un nivel interactivo para
establecer niveles de acceso más altos, pero se desaconseja encarecidamente. Existe el riesgo de exponer los niveles superiores.
Hay que tener cuidado al establecer el acceso inicial.

![Alt Image](./Images/20.png)

```
Este diagrama puede ayudar a ilustrar los niveles y las relaciones de cómo compartir información entre cada uno.
```

**Diseño multinivel C2**  
El diseño de una infraestructura C2 es una de las tareas más críticas a la hora de planificar un compromiso del Equipo Rojo.
La planificación de la infraestructura C2 implica elegir el número y el tipo de servidores C2, si se van a utilizar direcciones IP
direcciones IP o nombres de dominio, los protocolos C2, y si se van a utilizar redirectores. La decisión de cada uno
está directamente relacionada con los objetivos de un Equipo Rojo. Si un equipo se enfrenta a un objetivo en una operación a gran escala del Equipo Rojo
Si un equipo se enfrenta a un objetivo en una operación de Equipo Rojo a gran escala, los canales sigilosos y encubiertos serán buenas opciones.

Diseño típico de C2 para una operación de Equipo Rojo a gran escala  
```
● Tres servidores C2 con un nivel interactivo, un servidor de corta distancia y un servidor de larga distancia  
● Múltiples redireccionadores  
● Uno o dos nombres de dominio cuidadosamente elegidos para cada dirección IP (preferiblemente con historial y categorización)  
● No hay comunicación directa entre el objetivo y el C2. Todo el tráfico pivota a través de un servidor de redirección  
● El uso de protocolos comunes en puertos estándar para mezclar (HTTP, HTTPS, SSH, DNS)  
● Las comunicaciones están cifradas  
```

Si un equipo está emulando una amenaza específica o tratando de estimular la respuesta de un equipo azul, el sigilo puede no
ser tan importante.

Diseño típico de C2 para emular una amenaza diseñada para estimular al equipo azul (ejercicios)  
```
● Uno o dos servidores C2. Todos los niveles se utilizan para la interacción con el objetivo  
● No se utilizan redirectores  
● Se utilizan direcciones IP en lugar de nombres de dominio  
● El objetivo y el C2 se comunican directamente  
● Se utilizan protocolos comunes en puertos estándar o no estándar (HTTP, HTTPS)  
● Las comunicaciones pueden estar cifradas o no  
```

#### Domain Fronting  

El Domain Fronting es una técnica desarrollada para evitar la censura mediante el enrutamiento del tráfico
a través de dominios legítimos y de alta confianza. Hay muchos servicios que soportan el Domain Fronting,
incluyendo Google App Engine, Amazon CloudFront y Microsoft Azure. ¿Cómo funciona?
Cuando el tráfico es recibido por el servidor de un proveedor, como gmail.com, se envía a un servidor de origen,
como myapp.appspot.com. Esto se controla en base a una cabecera de host especificada en la solicitud HTTP.
El servidor de origen reenvía directamente el tráfico a un dominio especificado, que apunta a un servidor C2 controlado por la amenaza, o a un servidor personalizado.
controlado por la amenaza, o bien una aplicación personalizada proxyiza la solicitud para completar el reenvío.

Nota: El uso de domain fronting ha sido severamente limitado ya que las organizaciones han estado reduciendo activamente
la capacidad de utilizarlo. En el momento de escribir este libro todavía es una opción, pero como muchas técnicas, cambiará con el tiempo.
cambiarán con el tiempo.

Referencias
```
1. Wiki de Infraestructura del Equipo Rojo, https://github.com/bluscreenofjeff/Red-Team-Infrastructure-Wiki#domain-fronting.  
2. Dominio de fachada a través de dominios alternativos de Cloudfront, https://www.mdsec.co.uk/2017/02/domain-fronting-via-cloudfront-alternate-domains/.  
3. Redirectores de alta reputación y domain fronting, https://blog.cobaltstrike.com/2017/02/06/high-reputation-redirectors-and-domain-fronting/.  
4. Encontrar dominios frontables, https://github.com/rvrsh3ll/FindFrontableDomains  
```

### Key Chapter Takeaways

La ejecución del compromiso implica todos los esfuerzos desde el final de la planificación hasta el inicio de la culminación y
de la culminación y la presentación de informes, incluida la creación de la infraestructura. La fase de ejecución es simplemente la aplicación
aplicación práctica del "por qué" y el "cómo" de la planificación.  

Recuerde también:  
```
Una buena estrategia comercial es más valiosa que cualquier capacidad individual.  
● A veces la mejor manera de explotar un sistema es evitar el uso de exploits  
● Un plan detallado de C2 y una infraestructura definida pueden ser la diferencia entre un compromiso exitoso y uno fallido  
● Las herramientas son facilitadoras, nada más  
        ○ Conozca sus herramientas y cuándo (o cuándo no) ejecutarlas  
        ○ ¡Asegúrate de entender por qué se ejecuta una herramienta, qué hace y qué indicadores (o artefactos) proporciona!  
● ¡Registro, registro, registro!  
```

### ```Tareas para casa
```
1. Ampliar la guía de manejo de datos para incluir las pautas de repositorio y almacenamiento de datos
2. Desarrollar un proceso de recogida de datos y un flujo de trabajo para los operadores. Considerar las opciones de recogida manual y
opciones de recogida automatizada
3. Desarrollar una guía de orientación para los operadores
4. Desarrollar una caja de herramientas estándar. Nota: esto es recomendable pero opcional
5. Desarrollar una arquitectura de mando y control y un plan de despliegue del c2
```

## Culminación del compromiso

![Alt Image](./Images/21.png)

Tras la fase de ejecución, cada compromiso incluye una serie de actividades necesarias para un
para el cierre exitoso, la limpieza y la presentación de informes finales. Esta sección recorre los pasos necesarios para
cerrar con éxito un encargo.


### Saneamiento y limpieza

Todas las pruebas de una intervención deben ser saneadas antes de la salida del Equipo Rojo. Cualquier evidencia
que describa la naturaleza de los ataques, las vulnerabilidades, los resultados u otra información debe ser
eliminarse y destruirse por completo. Esta limpieza incluye herramientas y artefactos, así como la reversión de cualquier
de los controles de seguridad que puedan dejar un entorno menos seguro cuando finalice la intervención.
de un compromiso.

Además de las modificaciones del sistema, los equipos rojos pueden tener la oportunidad de modificar o eludir los controles de seguridad.
controles de seguridad. Si los controles de seguridad del sistema objetivo fueron desactivados o modificados, deben ser restaurados tan pronto como sea posible.
lo antes posible. Estos deben ser rastreados con todos los demás cambios.

```
La ROE es la ley  
El proceso de saneamiento debe documentarse en las ROE antes de la ejecución del compromiso. Esta es la mejor manera de
garantizar que el proceso de saneamiento se documenta y, si se sigue, se ejecuta adecuadamente.
```

Se desea que todos los exploits, kits de herramientas y mecanismos de persistencia tengan un código de autodestrucción
autodestrucción basado en el tiempo, para evitar la ejecución fuera de la ventana de compromiso, y basado en el objetivo para evitar la explotación fuera del entorno de destino.
para evitar la explotación fuera del entorno de destino. Para los elementos que no tienen código de autodestrucción incorporado
incorporado, el Equipo Rojo debe eliminar cada uno individualmente y documentar la eliminación. Cuando la limpieza no es
Cuando la limpieza no sea posible (pérdida de comunicaciones, sistema desconectado, permiso, etc.), el Equipo Rojo alertará a la AT
con el nombre del sistema, la dirección IP, los directorios, los nombres de los archivos, la fecha de modificación, las modificaciones realizadas, las herramientas
o archivos modificados. Un registro de seguimiento de cambios debería formar parte del conjunto de herramientas necesarias para cada compromiso.
(Nota: si se utilizan las recomendaciones de registro hechas anteriormente en el texto, este seguimiento se captura
en el registro). Las modificaciones de los sistemas siempre deben esperarse y planificarse como parte de un compromiso.
Estas modificaciones no son sólo cambios permanentes, como la caída de archivos o las modificaciones del registro de Windows
sino también los procesos en memoria. La siguiente lista de comprobación rápida ayudará a un compromiso
a eliminar todas las modificaciones.

**Lista de comprobación para la eliminación de modificaciones en la contratación**.

```
● Revertir las modificaciones del sistema de archivos.  
● Eliminar los mecanismos de acceso y las puertas traseras.  
● Eliminar los archivos arrojados por un operador o las herramientas del operador.  
● Asegurarse de que se eliminan los artefactos de archivo generados por el mecanismo.  
● Examinar todo el sistema para confirmar que el mecanismo no fue copiado o movido inadvertidamente.  
● Elimine o restaure las claves del Registro si se utilizan.  
● Restaurar los archivos modificados.  
● Eliminar o sustituir los archivos de inicio por los originales.  
● Examinar los scripts de inicio si se utilizan. Tenga en cuenta que el contenido de inicio puede haber cambiado.  
● Elimine los mecanismos de ejecución.  
● Elimine el mecanismo de instalación.  
● Copie los archivos de registro generados por el mecanismo en el repositorio de Red Team y elimínelos del sistema de destino.  
● Elimine los mecanismos de persistencia C2.  
● Terminar los canales C2.  
● Continúe con la supervisión de las conexiones en busca de mecanismos extraviados o perdidos.  
● Repita el proceso para los extraviados.  
● Proporcionar una lista de todos los artefactos, nombres, hashes, ubicaciones y su estado de limpieza a la AT.  
```

Considere lo siguiente
```
A veces, la organización de destino puede querer que determinados artefactos (quizás todos) se queden en la red con fines de formación o de puesta a punto de la herramienta y del procesamiento.

Esto debe ser aprobado y documentado antes del cierre del compromiso. Se debe proporcionar una lista de todos los artefactos y modificaciones a la AT designada por el objetivo.
```

### Verificación del registro del operador

Cada operador debe verificar la finalización de sus registros de operador antes de la finalización de un
compromiso. Cada uno debe comprobar también que todos los registros del operador, los datos recogidos a través de la automatización, los datos del objetivo
y las capturas de pantalla se han nombrado y almacenado adecuadamente en la carpeta de datos de la intervención.

```
Tenga en cuenta lo siguiente
Lo mejor es realizar la cumplimentación de los registros del operador durante todo el
de la operación. Un jefe de proyecto que hace que los operadores
que los operadores se aseguren de completar los registros antes del final de cada día
reducirá significativamente la falta de registros o de capturas de pantalla críticas.
```
Tras la notificación de finalización por parte de los operadores, el jefe del equipo rojo debe revisar la
consolidación. Si el jefe está convencido de que los datos están completos, debe crear un archivo comprimido con hash de todos los datos.
comprimido de todos los datos. Las copias realizadas del archivo deben guardarse en un lugar aprobado.
Este archivo puede ser un dispositivo de medios extraíbles encriptados que mantenga un acceso controlado o cualquier
lugar aprobado para el almacenamiento de estos datos sensibles.
El jefe del equipo rojo es el responsable último de la aceptación, revisión y consolidación de
los registros de los operadores y todos los datos. Se recomienda encarecidamente que el jefe del equipo rojo compruebe periódicamente el
durante la ejecución del proyecto para asegurarse de que los registros se completan, los datos se nombran y almacenan
se nombren y almacenen adecuadamente, y que los registros reflejen el cumplimiento de las ROE.

**Lista de comprobación de la finalización de registros**

```
● Asegurar la finalización de todos los registros de los operadores
● Asegurar la consolidación de todos los registros
● Asegurar la consolidación de los datos recogidos automáticamente
● Asegurar la consolidación de los datos objetivo
● Revisión y aceptación del líder del equipo rojo
● Archivar (Tar/Zip) y hacer un hash de todos los datos
```

### Briefings previos al informe

Se recomienda realizar un briefing de cierre tras el último día del compromiso. Este informe
Este informe probablemente no incluirá muchos de los detalles del informe final; sin embargo, debería permitir al equipo rojo
proporcionar al objetivo una visión general de alto nivel del acceso obtenido en relación con las
observaciones significativas de la intervención, los comentarios generales y las recomendaciones generales.

#### Informe ejecutivo

Al final de la ejecución de una intervención, la organización objetivo normalmente necesita (y a menudo garantiza) un
un resumen del evento. Esperar a un informe final puede mantener al objetivo fuera del circuito durante demasiado tiempo. Si
Si el registro y la recopilación de datos se realizaron correctamente (como debería ser), esto no sería una
tarea difícil.

La primera reunión posterior al compromiso suele ser el informe ejecutivo. La reunión ejecutiva suele realizarse
se suele realizar poco después de que se haya completado la ejecución (en el plazo de uno o dos días tras la ejecución). Esta reunión
está dirigida a la dirección y debe incluir al personal clave de la organización objetivo. Esta reunión
Esta reunión no sólo debe incluir la gestión de la seguridad de la información, sino también la gestión de la organización.
de la organización. El resultado de la intervención de un equipo rojo puede afectar al funcionamiento de la organización en el futuro,
y puede requerir financiación para llevar a cabo mitigaciones o modificaciones de personal. La concienciación de la dirección
La concienciación y el compromiso de la dirección son fundamentales si los resultados de los equipos rojos se van a utilizar para mejorar la posición de seguridad de una organización
para defender y responder a una amenaza.

El informe ejecutivo debe centrarse en el panorama general del evento y se presenta mejor como una
historia cronológica de pasos críticos y observaciones. La historia y las acciones se convertirán en la narrativa del ataque en el informe final.
en la narración del ataque en el informe final. En este momento, el informe final y el análisis no están completos, pero
la dirección busca respuestas rápidas. Si se identifican problemas obvios, podrían destacarse
en el informe. Hay que señalar que el informe final puede contener observaciones que no se
descubran hasta que se haya analizado toda la información.

```
Tenga en cuenta lo siguiente
La mayoría de los ejecutivos y altos cargos no están tan interesados en los detalles técnicos del encargo. Ellos
suelen estar más interesados en los impactos en las funciones empresariales, la producción y la reputación.
Intente correlacionar cada acción o hito importante con los aspectos empresariales afectados. Si es posible, estimar los costes totales
Si es posible, la estimación de los costes totales (incluidos los ingresos perdidos, el tiempo, la reparación, la capacidad, etc.) facilita la comprensión de los ejecutivos de los impactos y refuerza la interacción.
impactos y refuerza la interacción.
```

**Lista de comprobación del informe ejecutivo**
```
● Se realiza inmediatamente después de la ejecución del compromiso  
● Incluye a la dirección de la organización (responsables de la toma de decisiones)  
● Incluir al personal técnico y de seguridad de la información clave  
● Centrarse en el resumen cronológico de las observaciones (historia del evento)  
● Destacar las observaciones críticas  
● Informar a la audiencia de que este informe es simplemente un resumen. El informe final contendrá todos los detalles del evento   
```
Opcional  
```
● Incluir personal adicional de seguridad de la información o técnico  
● Incluir a expertos en sistemas críticos  
● Incluir personal jurídico  
```

#### Informe técnico

Un outbrief técnico (o sesión informativa técnica) es extremadamente valioso para la organización, para el
equipo azul/defensivo y para el propio equipo rojo. Estos intercambios técnicos no siempre ocurren pero
son demasiado valiosos para ignorarlos y deberían ser un paso obligatorio en cada compromiso.

La tecnología sobre tecnología es un intercambio bidireccional de información técnica entre el Equipo Rojo, el
equipo azul y la organización. Durante este intercambio, tanto los elementos rojos como los defensivos
defensivos proporcionan una revisión técnica muy detallada, paso a paso, de las acciones y resultados (incluyendo todos los
detalles asociados) del compromiso. Aquí es donde se unen la formación y la educación y es una de las
oportunidades más valiosas para que todas las partes aprendan. La mayoría de las veces, los defensores descubren que
tenían muy poca información sobre las acciones del Equipo Rojo en la red. El "tech-on-tech" permite a ambas partes
participar en un recorrido detallado junto con una sesión de preguntas y respuestas.

La aparición del tech-on-tech es a menudo más útil para aquellos que van a implementar mitigaciones o
cambios impulsados por la actividad del equipo rojo que el informe final. Aunque el proceso es bastante sencillo, el valor
es insuperable. A continuación se identifican algunas acciones/papeles de tech-on-tech para dar una mejor
para que se entienda mejor lo que debe ocurrir.

**Lista de comprobación de la sesión informativa sobre tecnología y planificación de la agenda**  

El equipo rojo:  
```
● Explica los TTPs rojos y los IOCs previstos.  
● Explica su proceso de pensamiento inicial para cumplir los objetivos del compromiso.  
Explica su proceso de pensamiento inicial para cumplir con los objetivos del compromiso. (Esto ocurre simultáneamente con el recorrido del defensor).  
● Describe por qué se ejecutaron esas acciones. (¿Qué llevó a cada acción específica?)  
● Proporciona los resultados de cada acción y cómo esa acción permitió la siguiente.  
● Proporciona recomendaciones o técnicas que limitarían cada acción de amenaza.  
```

El equipo defensivo:  
```
● Tiene la oportunidad de preguntar el cómo y el porqué.  
● Explica el proceso para asegurar y defender el entorno.  
● Identifica cualquier alerta, desencadenante o anomalía dentro del entorno durante el compromiso.  
● Recorre las acciones azules en respuesta a la actividad del equipo rojo. (Esto ocurre simultáneamente con el recorrido del Equipo Rojo).  
● Identifica cómo se podría haber detectado, prevenido o aprovechado la actividad del Equipo Rojo (la aportación del Equipo Rojo suele ser clave durante este periodo de discusión).  
● Proporciona información sobre las acciones y recomendaciones del Equipo Rojo.  
● Utiliza la información de tecnología sobre tecnología para realizar un análisis posterior al compromiso antes de recibir el informe oficial.  
```

#### Responder a los comentarios negativos de la organización durante las sesiones informativas.

Inevitablemente, un Equipo Rojo será cuestionado en sus observaciones. Un Equipo Rojo debe estar preparado para
responder a preguntas o comentarios negativos, tales como "Nosotros les dimos acceso", "Un tipo malo nunca
hacer eso", o "¿Cómo es eso justo?". Estos comentarios son demasiado comunes y suelen provenir de
organizaciones inmaduras o desinformadas sobre las amenazas y la seguridad.

Para responder adecuadamente, un equipo rojo debe ser profesional y llevar a cabo un compromiso de alta calidad.
calidad. El Red Teaming puede generar estrés y hacer que la gente se ponga a la defensiva, tanto personal
como profesionalmente. Un Equipo Rojo no debe presumir o menospreciar al personal del objetivo durante una sesión informativa o en un
informe. Un Equipo Rojo que cuenta la historia de un compromiso con hechos simples puede transmitir un mensaje fuerte
un mensaje contundente, sin culpar a nadie. Incluso si una organización lo hizo mal, los hechos serían más que suficientes para
para transmitir el mensaje. Recuerde, el trabajo de un Equipo Rojo no es demostrar cuán elitistas son sus habilidades de hacking
sino ejercitar un escenario de amenaza que permita a una organización aprender y mejorar su seguridad. A
La historia del Equipo Rojo debe transmitir los fallos significativos que condujeron a un compromiso exitoso.

Una buena regla de práctica es la no atribución, o no atribuir los fallos a personas concretas. Muchas organizaciones de
organizaciones culpan de los fallos de seguridad a ciertos individuos en lugar de reconocer las brechas o fallos de la organización.
o fallos de la organización. Culpar a los individuos parece ser una solución fácil, pero rara vez mejora la seguridad.
Culpar a Bob en contabilidad por hacer clic en un correo electrónico de phishing no es la razón por la que toda la propiedad intelectual fue
intelectual fue robada.

En ocasiones, un Equipo Rojo puede encontrarse con una persona inusualmente hostil o posiblemente con un equipo técnico hostil.
equipo técnico hostil. En estos escenarios, difundir las hostilidades se vuelve tan importante como la información
que se transmite; de lo contrario, la información puede no ser ingerida como se pretende. El equipo rojo puede utilizar
tres sencillas preguntas para empezar a calmar la situación.

**Preguntas para disipar la respuesta hostil a la actividad del equipo rojo**

1. ¿La acción se desarrolló dentro del ámbito de aplicación?  
```
Un compromiso bien planificado tendrá un alcance bien definido. Si todas las actividades se desarrollan dentro del
Si todas las actividades se desarrollan dentro del ámbito de aplicación, todas las actividades son aceptables.  

En los casos en los que se proporcione información al Equipo Rojo, indíquelo por adelantado al describir
el escenario.  

Enumerar los supuestos para ayudar a garantizar que la audiencia esté de acuerdo con los supuestos o, como mínimo, que entienda por qué se tomaron acciones específicas.
como mínimo, entienda por qué se han tomado acciones específicas.
```

2. 2. ¿La acción se ajustó a las normas de intervención?
```
Las Reglas de Enfrentamiento dictan todo sobre cómo se realizará o no una acción
acción. Las Reglas de Enfrentamiento deben ser respetadas. La violación de las reglas es una forma rápida de que un Equipo Rojo
perder la confianza de la organización. Al igual que con la operación en el ámbito, si las Reglas de
Si no se violan las Reglas de Compromiso, la acción es aceptable.
```

3. ¿Se ha realizado la acción en un ataque del mundo real?
```
Si una acción o técnica se ha utilizado en el mundo real, tiene validez. Las organizaciones pueden
rápidamente a los ataques teóricos. Poder relacionar una acción con una técnica o amenaza
técnica o amenaza conocida ayudará a validar su autenticidad.
```

### Conclusiones clave del capítulo

La fase de culminación es un hito importante en un compromiso del Equipo Rojo. Toda la actividad se ha completado, y
los datos o registros se han finalizado. Si la validación de los datos no se ha completado, existe un grave riesgo para elaborar un
informe de calidad. Esta es la última oportunidad para garantizar que los registros estén completos, que existan capturas de pantalla y que se pueda contar la historia de la intervención.
y que se pueda contar la historia del compromiso.

La culminación es el primer momento oficial en que la organización destinataria recibe información sobre el resultado de una
resultado de la intervención. El éxito o el fracaso de una intervención suele depender de la calidad del briefing realizado
en esta fase.

Si se realiza correctamente, el jefe del equipo rojo debería tener todo lo necesario para empezar a desarrollar un informe profesional de calidad.
informe de calidad y profesional.


### Tarea
```
● Desarrollar un documento de seguimiento de la modificación del sistema de compromiso
● Desarrollar un documento de seguimiento de saneamiento y limpieza
● Asegurar que la verificación del registro del operador se incluya en la metodología o flujo de trabajo del compromiso
● Desarrollar una plantilla de agenda para los outbriefs ejecutivos
● Desarrollar una plantilla de agenda para los outbriefs de tecnología sobre tecnología
```

## Engagement Reporting

![Alt Image](./Images/22.png)

Los informes son el producto final y la única prueba de un compromiso. La fase de elaboración de informes es un
La fase de elaboración de informes es un aspecto crítico de la intervención del Equipo Rojo. Los informes deben permitir a la organización reproducir las
y resultados del Equipo Rojo y son la última forma de evidencia que puede ser analizada y utilizada para
proporcionar una base para mejorar la seguridad. Deben incluirse como entrega final de un compromiso.
Algunos equipos (especialmente los internos) no suelen elaborar informes formales. Algunos sólo proporcionan una lista
de hallazgos y lo etiquetan como un informe. Si bien esto es aceptable (suponiendo que se produzca alguna entrega detallada
Si bien esto es aceptable (siempre que se produzca algún producto detallado), se recomienda encarecidamente desarrollar un proceso formal de elaboración de informes utilizando una plantilla estándar.
Este proceso garantiza la coherencia y la exhaustividad en la entrega de un producto final tras un
compromiso.

```
Normas relativas a la recopilación de datos y la elaboración de informes
1. Si una acción no se registra, no se ha producido.
2. Si no hay informe, no hubo compromiso
```
Los informes no sólo documentan la actividad que tuvo lugar durante un compromiso específico, sino que también proporcionan una
una excelente referencia que puede utilizarse como hoja de ruta fiable para planificar y diseñar otras o futuras
de otros o futuros compromisos. Muchos proyectos comparten enfoques y objetivos similares. A medida que el número de informes
de informes, pueden analizarse juntos para comprender los patrones y riesgos comunes que comparten varios
entornos. Éstos pueden utilizarse para comprender cómo las amenazas tienen éxito o fracasan cuando se enfrentan a diferentes niveles de defensa.
niveles de defensa.


### Diagramas de flujo de ataques

![Alt Image](./Images/23.png)

Todo el mundo ha oído decir que una imagen vale más que mil palabras. Lo mismo se aplica cuando se generan
informes. Esto es especialmente cierto en aquellos que contienen hilos y actividades complejas. El Red Teaming consiste en
sobre la comprensión del impacto de las acciones de una amenaza contra un objetivo. Aunque esto se documenta en los registros
y eventualmente escrito como observaciones, un diagrama visual es extremadamente valioso y una de las formas más
de las formas más efectivas de describir y resaltar las actividades y observaciones clave.

El diagrama de arriba es un ejemplo de un compromiso real del Equipo Rojo que aprovecha un modelo simple de
modelo simple de infracción. Este compromiso se utilizó para entrenar a un nuevo equipo rojo utilizando un compromiso pequeño y simplificado.
simplificado. Los objetivos de la intervención eran los siguientes

```
Entrenar y exponer a un nuevo equipo rojo a los procesos del equipo rojo  
Medir la capacidad de una amenaza para moverse lateralmente  
Medir la capacidad del defensor para detectar tráfico C2 y binarios  
● Medir la capacidad de realizar y posteriormente detectar la exfiltración de datos críticos  
```
Este compromiso del Equipo Rojo fue diseñado como entrenamiento C2 para un nuevo Equipo Rojo y para educar a un Equipo Azul en las técnicas de amenaza.
Azul sobre las técnicas de amenaza. El Equipo Rojo diseñó y puso en escena el Mando y Control con
El Equipo Rojo diseñó y puso en escena el Mando y Control con objetivos de amenaza y COI específicos, utilizando un perfil de amenaza para documentar el diseño de la misma. El diagrama destaca
El diagrama destaca las acciones, los éxitos y los fracasos del Equipo Rojo y se creó utilizando el software comercial de
comercial de mapeo mental XMind (http://www.xmind.net/), pero podría haberse creado fácilmente en una serie de
otras herramientas de diagramación.

Un diagrama bien diseñado puede utilizarse únicamente para presentar un compromiso del Equipo Rojo. El poder de una
El poder de una imagen es realmente inmenso. Los diagramas no son obligatorios, pero son muy recomendables.

```
Considere esto
Los autores de este libro a menudo sólo utilizan diagramas para dirigir las sesiones informativas ejecutivas o técnicas, en lugar de utilizar un largo documento de texto o una presentación de PowerPoint.
de texto o una presentación de PowerPoint. Las presentaciones gráficas son una gran manera de transmitir las complejas
acciones complejas de un compromiso del Equipo Rojo.
```

### Observaciones vs. Conclusiones

El informe del compromiso de Red Team puede ser muy diferente a los informes generados en las pruebas de penetración o
evaluaciones de vulnerabilidad. Los objetivos del compromiso y los impactos asociados son los puntos de datos fundamentales
que alimentan directamente un informe de Red Team. Como se ha comentado anteriormente, las intervenciones de los equipos rojos están muy
centrados en el escenario. Esto conduce a un informe impulsado por la historia que contiene la historia (o el flujo) del Equipo Rojo y
su capacidad para ejecutar o cumplir sus objetivos.

Los informes de pruebas de penetración o de evaluación de vulnerabilidades se centran en los hallazgos. Por ejemplo, una prueba de penetración
Por ejemplo, una prueba de penetración puede descubrir una política de contraseñas débil que deja a una organización susceptible a un ataque de fuerza bruta.
o parches faltantes que permiten la explotación de las estaciones de trabajo de los usuarios finales. Estos hallazgos
Estos hallazgos suelen estar relacionados con algún control o política de seguridad. Tal vez estos hallazgos conduzcan a las
de modificar la política de contraseñas para requerir contraseñas más largas, implementar la autenticación de dos factores y asegurar que el
autenticación de dos factores, y asegurarse de que se sigue la política de parches. Estos son hallazgos importantes
importantes, pero están más en la línea de la limpieza de la seguridad y la reducción de la superficie de ataque.
de ataque.

Los compromisos de los equipos rojos tienen objetivos muy diferentes a los de otras pruebas de seguridad. Los métodos para describir
Los métodos para describir los objetivos en un informe de Red Team se representan mejor como observaciones que como hallazgos discretos. Para
ejemplo, un sistema obsoleto puede tener fallos que permitan a un operador comprometer una estación de trabajo.
Esto proporciona mando y control y se utiliza para realizar el conocimiento de la situación de los
los activos de la organización objetivo. Un operador continúa explorando y moviéndose por la red del objetivo y
finalmente roba datos de propiedad como objetivo planificado. El fallo técnico es importante y debe ser
documentado, pero es sólo uno de una serie de pasos. Esta serie de pasos puede utilizarse para detallar la
observación que tiene una amenaza con respecto a la libertad de movimiento.

Ejemplo de observación
```
El equipo rojo pudo moverse libremente por la red del objetivo sin apenas resistencia. El host inicial
El anfitrión inicial comprometido proporcionó el escalón inicial, pero pronto fue abandonado una vez que se estableció la libertad de movimiento.
libertad de movimiento. El equipo rojo no observó ningún control preventivo o de detección que indicara que la organización
era consciente de la actividad de la amenaza. Esta libertad de movimiento fue clave para proporcionar la capacidad de exfiltrar
datos sensibles del objetivo.
```

El Equipo Rojo se rige por objetivos que pretenden estimular o medir no sólo los fallos técnicos sino
las operaciones de seguridad en su conjunto. Esto incluye a las personas, los procesos y la tecnología. Un informe del Equipo Rojo
utiliza un formato basado en historias en el que se enumeran las observaciones en lugar de los hallazgos.

### Calificación del riesgo y métricas

La mayoría de las pruebas de seguridad incluyen una calificación de riesgo con un hallazgo. Una escala común utiliza el diagrama de la matriz de riesgo
compuesto por Impacto vs. Probabilidad en asignaciones Alta, Media o Baja. Lo más frecuente es que se represente
en un diagrama cuadrado de 3x3. Aunque esto puede dar una idea general del riesgo, suele ser demasiado arbitrario y
subjetivo. Los valores elegidos quedan a la discreción de los redactores del informe. A menos que la organización objetivo
se incluya en la decisión de calificación, estas calificaciones incluyen sólo la perspectiva del evaluador de seguridad. Estos
tipos de calificaciones funcionan bien para las evaluaciones de vulnerabilidad, donde las vulnerabilidades individuales son el
objetivo principal y se pueden asignar puntuaciones CVE asociadas. También puede funcionar para las pruebas de penetración cuando
medir y validar los niveles de explotabilidad es el objetivo principal.

Este tipo de puntuaciones pueden utilizarse en los informes del Equipo Rojo; sin embargo, no son apropiadas para la
metodología de observación. Consideremos este ejemplo. Si un Equipo Rojo tuviera como objetivo el robo de
datos de propiedad de la organización, el informe de observación describiría cómo y dónde se tomaron los datos
y el volumen de datos adquiridos. Esto es difícil de resumir en un solo punto en una
matriz de riesgo de impacto vs. probabilidad. Considere otra opción, utilizando las métricas de los objetivos del Equipo Rojo. Rojo
Los objetivos del Equipo Rojo se han discutido anteriormente en el libro. Estos objetivos tienen métricas asociadas en forma de
preguntas. En lugar de calificar el riesgo utilizando una escala subjetiva, una narración que responda a las preguntas puede
describir el riesgo. Esto no asigna un valor alto o bajo, pero proporciona a la organización
información que puede utilizarse para determinar el nivel de acción necesario.

Si se requiere un diagrama de matriz de riesgo de Impacto vs. Probabilidad, incluya tanto la narrativa del objetivo del Equipo Rojo
y la matriz de riesgos de vulnerabilidad. Recuerde que el Red Teaming se centra en los objetivos y no en las vulnerabilidades.
Las vulnerabilidades se descubrirán durante un compromiso del equipo rojo y pueden documentarse utilizando la
matriz de riesgo tradicional en una sección de conclusiones secundarias del informe.


### Comparación de matrices de riesgo

Las matrices de riesgo son una gran manera de añadir un elemento visual a un informe para proporcionar un contexto adicional y
comprensión. Esta matriz se suele utilizar para estimar el grado de gravedad y la probabilidad o
nivel de algún impacto a una vulnerabilidad discreta específica o hallazgo

#### Ejemplo de matriz de riesgo 3 × 3

La matriz de riesgo 3x3 es posiblemente la más común en los informes de seguridad. Es relativamente sencilla y
proporciona nueve niveles posibles para asignar el riesgo. Este tipo de clasificación es muy subjetiva. Es un reto
Es un reto para un probador de seguridad (vulnerabilidad, penetración o equipo rojo) calificar con precisión el impacto o la probabilidad en
en términos de riesgo para las operaciones. Esto lleva a calificaciones centradas en el nivel técnico. Aunque esto es útil, no siempre
Si bien esto es útil, no siempre proporciona al liderazgo la visión necesaria para tomar una decisión informada sobre la aplicación de
mitigación con sus limitados recursos.

![Alt Image](./Images/24.png)

Probabilidad: La probabilidad de que un evento ocurra:

```
● Baja - No es probable que ocurra
● Media - Puede ocurrir
● Alta - Probablemente ocurra
```
Impacto: El resultado esperado de un evento (grado de lesiones, daños a la propiedad u otros factores que perjudican la misión), medido como
que perjudican la misión) medido como:


```
● Bajo - Impacto limitado en las operaciones
● Medio - Impacto notable en las operaciones
Alto - Impacto significativo en las operaciones
```
#### Ejemplo de matriz de riesgo 5 × 5

La matriz de riesgo 5x5 es una versión ampliada de la 3x3. El uso es el mismo pero proporciona un poco más de
granularidad. Esto puede ayudar a afinar la calificación, pero sufre de limitaciones similares. Ofrece un método
método para ver el riesgo en términos de operaciones en lugar de vulnerabilidades discretas. La versión presentada
ha sido adoptada y modificada por el Ejército de Estados Unidos[21] y el NIST[22] para centrarse en el impacto de las operaciones
en lugar del impacto en la misión.

![Alt Image](./Images/25.png)

Probabilidad: La probabilidad de que un evento ocurra:

```
● Frecuente - Ocurre a menudo
● Probable - Ocurre varias veces en un periodo x
● Ocasional - Ocurre esporádicamente
● Rara vez - Poco probable pero podría ocurrir
● Improbable - Probablemente no ocurra
```
Gravedad: El resultado esperado de un evento (grado de lesiones, daños a la propiedad u otros factores que perjudican la misión).
que perjudican la misión) medida como:

```
● Catastrófico - Impacto directo, generalmente de larga duración si no es permanente
● Crítico - Impacto significativo: detiene o paraliza el funcionamiento
● Moderado - Pérdida notable: reduce/retrasa el funcionamiento/la producción
● Marginal - Pérdida limitada: se nota pero no detiene el funcionamiento
● Insignificante - Alguna pérdida: pasa desapercibida si no se vigila de cerca
```
La clave en la construcción de estas matrices es la vulnerabilidad. Como se ha dicho varias veces a lo largo de este libro, el Red Teaming no se centra en la vulnerabilidad.
Como se ha dicho varias veces a lo largo de este libro, el Red Teaming no se centra en la vulnerabilidad. Teniendo en cuenta este proceso de pensamiento, el compromiso de un Equipo Rojo debe ser
construido como una narrativa de acciones de amenaza. A continuación se presentan algunas preguntas que pueden ayudar a determinar el
impacto y dar forma a los objetivos del Equipo Rojo. Consulte la sección Objetivos del Equipo Rojo de este libro para obtener más
detalles. Estas preguntas deben reflejar directamente los objetivos creados durante la planificación del compromiso.

Preguntas a tener en cuenta al desarrollar los objetivos del equipo rojo:

```
● ¿Qué capacidad tiene el adversario para acceder a las zonas comunes?
● ¿Qué capacidad tiene un adversario para acceder a las zonas restringidas?
● ¿Puede un adversario utilizar el acceso obtenido para habilitar capacidades electrónicas?
● ¿Qué impactos puede tener un adversario con el acceso ganado?
● ¿Puede un adversario acceder a sistemas clave/críticos?
● ¿Qué impactos puede tener un adversario en un sistema clave/crítico?
● ¿Qué capacidad tiene un adversario para moverse libremente por una red?
● ¿Cuánto tiempo puede vivir un adversario en el objetivo sin ser descubierto?
● ¿Qué acciones son necesarias para activar una detección/respuesta?
```
Estas preguntas se centran en medir o comprender la capacidad que tiene una amenaza para realizar alguna
acción o la capacidad que tiene la defensa para impactar en la amenaza. Esto lleva a la necesidad de un medio alternativo
medio de proporcionar métricas de riesgo.

#### Categorización de tres niveles

Chris Crowley[23] ha propuesto un concepto simple pero muy efectivo para la categorización utilizando sólo
tres niveles. Aunque esta estructura escalonada está pensada para ser aplicada a las operaciones de seguridad, puede ser
puede aplicarse a prácticamente cualquier concepto.

Una de las ventajas de este modelo es que las categorías se centran en la capacidad de mitigación y no en el riesgo. Por naturaleza, esto
proporciona un plan de acción para implementar mejoras. Revisemos y entendamos este concepto
empezando por las categorías de niveles. Cada nivel se define en función de la facilidad relativa de aplicar una
mitigación a la observación o al hallazgo.

**Matriz de niveles**

```
| Categoría de la observación o del hallazgo
|---------- |------------------------------------------------- |
| 1. La corrección está disponible en el entorno.
| | pero no ha sido implementada o | | aplicada.
| | aplicada.                                        	
| | |
| 2. La corrección o mitigación está disponible en el entorno, pero no se ha aplicado.
| | disponible en el entorno o en el público, pero | | | | algo como la política o la
| | algo como la política, el procedimiento, la política, | | | los contratos, la formación, etc.
| | contratos, formación, etc. impiden | | | la implementación o aplicación.
| | la implementación o la aplicación | | | de la misma.

| 3. La corrección o mitigación no está disponible en ninguna industria.
| | disponible en cualquier industria o sector. La investigación
| | o se requiere un esfuerzo adicional para investigar | | | | para determinar una corrección o mitigación.
| | para determinar un plan de corrección o mitigación.   	
```
![Alt Image](./Images/26.png)

Ejemplo de diagrama que resume las categorías

![Alt Image](./Images/27.png)

Ejemplo de fragmento de un informe que muestra cómo utilizar la clasificación por categorías

```
Pensamientos del autor  
Muy pocas cosas deberían ser etiquetadas como 3. Casi siempre hay una mitigación/resolución aceptable.  

Muchos serán probablemente etiquetados como 2. Esto debería ser motivo de cambio de política o proceso y podría utilizarse para justificar la formación adicional.  

Cualquier cosa etiquetada como 1 debería ser motivo de gran preocupación para la organización, la división o la dirección. A menudo indica una falta de esfuerzo.
```

Es importante señalar que este método de categorización requiere una comunicación abierta y eficaz
entre el Equipo Rojo y la organización. Los equipos rojos internos pueden tener el conocimiento y la experiencia
conocimiento de la organización y la experiencia necesaria para categorizar sus observaciones. Sin embargo, como la mayoría de los Equipos Rojos
(internos o externos) no suelen formar parte de la función empresarial que se está evaluando, requieren una
revisión y discusión en colaboración de cada observación.

Durante la elaboración de los informes de los equipos rojos, este método puede utilizarse junto con la Pirámide del Dolor para
ilustrar cómo una corrección específica afecta a la capacidad de una amenaza para realizar acciones nefastas. Este conocimiento de
Este conocimiento puede, a su vez, ser aprovechado para crear una priorización de correcciones o modificaciones organizativas.
modificaciones organizativas.

#### Pirámide del dolor

Las operaciones de seguridad no necesitan una lista de parches o fallos de configuración como el punto culminante de
mitigaciones o recomendaciones. Sí, deben incluirse en el informe. Sin embargo, es mucho
Sin embargo, es mucho más beneficioso proporcionar a las operaciones de seguridad una lista de acciones, procesos, procedimientos, etc. que
dificultarían la capacidad de una amenaza para operar (moverse, recopilar datos y causar impacto). A
gran manera de describir e ilustrar este concepto es la Pirámide del Dolor.

![Alt Image](./Images/28.png)

La Pirámide del Dolor[24] fue creada y descrita por David Bianco en 2013 y revisada posteriormente en
2014. La pirámide describe los tipos de indicadores que pueden utilizarse para detectar actividades de amenaza y cuánto
dolor se causará (a la amenaza) si un Equipo Azul es capaz de negar a una amenaza la capacidad de realizar
acciones que generan esos IOC. ¿Qué significa esto en términos de un compromiso del Equipo Rojo? Rojo
Los equipos rojos generan artefactos durante un enfrentamiento. Un Equipo Rojo puede utilizar el concepto de la Pirámide del
El Equipo Rojo puede utilizar el concepto de la Pirámide del Dolor para medir su posición en este gráfico durante una evaluación. En otras palabras, ¿cuánto dolor está causando el
Azul causa al Rojo.

Cuando un equipo azul se mide por las acciones de una amenaza en lugar de por lo bien que detecta
malware, configuran sus cortafuegos o implementan una política de contraseñas, se les mide contra
las técnicas de las amenazas. Esto incluye ataques conocidos, desconocidos e incluso de día cero. Descomponer las amenazas
en sus acciones proporciona a los defensores una forma manejable de entender la eficacia de su
estrategia defensiva. Los equipos azules pueden ser más eficaces y protegerse mejor contra cualquier amenaza
en lugar de defenderse contra una sola pieza de malware.

La perspectiva de un equipo azul
```
Detección en profundidad  
La ingeniería de detección (el proceso de creación de una lógica de detección para la actividad de los atacantes) es una disciplina a menudo mal entendida.
disciplina. Es común ver estas "detecciones" etiquetadas como buenas o malas, pero la lógica de detección no es inherentemente ninguna de las dos.
El malentendido tiende a ocurrir cuando las expectativas de alguien sobre una lógica específica no se alinean con la realidad. Para
tener éxito en la detección, es importante construir una malla de detección que combine indicadores precisos con bajas
falsos positivos (firmas) con indicadores amplios con bajas expectativas de falsos negativos
(detecciones de comportamiento). Me refiero a este concepto como Detección en Profundidad. Este enfoque garantiza que los analistas puedan confiar en
detección de alta señal de actividad mala conocida, mientras que también esperan que la malla resista los intentos de evasión.  
- Jared Atkinson, Microsoft MVP, @jaredcatkinson  
    Presentación del embudo de fidelidad - https://posts.specterops.io/introducing-the-funnel-of-fidelity-b1bb59b04036
```

¿Cuáles son algunos ejemplos de acciones defendibles que dificultarían la capacidad de actuación de una amenaza?

```
|-----------------------------------------------------------------------------------------------|
| Acción Defensiva | Descripción |
|-----------------------------------------------|-----------------------------------------------|
| Impedir la comunicación entre clientes | Impedir estas comunicaciones |
| | limita la capacidad de una amenaza de moverse libremente |
| | a través de la red, reduce la | | probabilidad de
| | | probabilidad de descubrimiento de cuentas privilegiadas
| | | descubrimiento, obliga a aumentar el tiempo | | | y el esfuerzo (más
| | y esfuerzo (más actividades y | | artefactos).
| | artefactos), y, por lo tanto, puede aumentar
| | | la capacidad de detección del defensor.         	
|-----------------------------------------------------------------------------------------------|
| Impedir la comunicación de servidor a cliente | Suponiendo que la red haya impedido | | la comunicación de cliente a cliente.
| | comunicaciones de cliente a cliente, la | | | | única opción que tiene una amenaza.
| | única opción que tiene una amenaza es intentar | | | acceder a un servidor.
| | acceder a un servidor, pero no puede | |
| | comunicar el servidor al cliente.         	
|-----------------------------------------------------------------------------------------------|
| Bloquear las comunicaciones salientes del servidor | Hay muy pocos casos en los que un |
| | servidor necesita comunicarse con un | | | sistema externo.
| | sistema externo a la red. Estos casos son excepciones.
| | son excepciones y deben ser gestionados | | | para permitir sólo las conexiones
| | para permitir sólo las conexiones con el | | | activo externo requerido.
| | requerido o a la IP externa y | | | | a la red.
| | permitir sólo el uso de los puertos | | requeridos
| | y protocolos requeridos.                            	
|-----------------------------------------------------------------------------------------------|
| Borrar credenciales administrativas en caché | Descubrimiento de credenciales en caché es un |
| | método común y principal en el que | | | las amenazas escalan privilegios.
| | las amenazas escalan privilegios.              	|
|-----------------------------------------------------------------------------------------------|
| Restablecer la cuenta KRBTGT: Restablecer la cuenta KRBTGT dos veces.
| | dentro de un marco de tiempo limitado seguido | | por el cambio de la cuenta KRBTGT.
| | por el cambio de todas las credenciales | | administrativas.
| | credenciales administrativas. Estos restablecimientos limitan la capacidad de una
| | de una amenaza para mantener el acceso después de | | |
| | cambios de credenciales | |
|-----------------------------------------------------------------------------------------------|
| Realiza una revisión de elementos sensibles | Realiza búsquedas frecuentes y |
| | actividades de descubrimiento de elementos críticos | | | almacenados en los activos de la organización.
| | almacenados en los activos de la organización | | | | (contraseñas, etc.)
| | (contraseñas, configuraciones, privacidad de | | | información).
| (contraseñas, configuraciones, datos de la Ley de Privacidad de la Información (PIA), propiedad intelectual, etc.)
| (Contraseñas, configuraciones, datos de la Ley de Privacidad de la Información (PIA), propiedad intelectual, etc.)              	|
|-----------------------------------------------------------------------------------------------|
| Bloquear y desactivar los puertos no necesarios, | Tanto los sistemas internos como los externos y |
| protocolos, y servicios (PPS) | dispositivos de red deben desactivar y |
| | bloquear los PPS que no sean necesarios para la |
| | red. Limitar los PPS sólo a lo que es | | necesario para cada
| | requerido para cada sistema específico | | | | |.
|-----------------------------------------------------------------------------------------------|
| Implementar la separación de cuentas | Los usuarios deben estar limitados sólo a lo que |
| y privilegios | es necesario para realizar las tareas diarias.       	|
| | Los usuarios estándar a menudo no necesitan | | privilegios elevados.
| | privilegios elevados en el día a día.     	
| En los raros escenarios en los que un usuario necesita privilegios elevados a menudo, se puede utilizar el sistema de privilegios elevados.
| | elevación a menudo, requiere el uso de una | | cuenta secundaria
| | cuenta secundaria con sólo el | | acceso requerido y sin
| | acceso requerido y sin capacidad de | | comunicación externa.
| | capacidad de comunicación externa | |
|-----------------------------------------------------------------------------------------------|
| Asegúrese de que los permisos de grupo son | | Esta recomendación tiene múltiples | | ud.
| identificados y mapeados apropiadamente | aplicaciones; sin embargo, el foco principal |
| | es en los grupos y permisos anidados.         	|
|-----------------------------------------------------------------------------------------------|
| Implementar el Administrador Local de Microsoft | No hay dos cuentas locales que tengan la misma | Solución de Contraseñas (LAPS).
| Solución de contraseñas (LAPS) | Contraseña. Un componente del lado del cliente |
| | genera una contraseña aleatoria, actualiza |
| | la contraseña LAPS en la cuenta de ordenador de Active |
| Directory, y establece la contraseña localmente.
| | la contraseña localmente | |
|-----------------------------------------------------------------------------------------------|
| Autenticación de múltiples factores | | Control de seguridad adicional y |
| | protección que requiere más de un | | autenticador o autenticación.
| | autenticador o factor de autenticación | |

|-----------------------------------------------------------------------------------------------|
| Implementar listas blancas de aplicaciones.
| | sólo después de que todas las | | recomendaciones anteriores
| | recomendaciones previas hayan sido | | | implementadas.
| | implementadas.                              	|
|-----------------------------------------------------------------------------------------------|
```
Esta lista está compuesta por una lista de controles prevenibles (Estrategias de mitigación Parte 1[25] y Parte 2[26])
y es una gran lista de técnicas de inicio que un Equipo Rojo puede utilizar para aplicar técnicas de Equipo Rojo que directamente
mide la capacidad de las operaciones de seguridad para detectar y responder a las técnicas de amenaza.


### Narrativa del ataque

La sección Narrativa de Ataque del informe contiene las observaciones hechas durante un compromiso del Equipo Rojo
de los equipos rojos. Es la versión escrita del diagrama de ataque. Normalmente se escribe en
Se suele escribir en orden cronológico y sigue el flujo de ejecución de un compromiso. Las observaciones clave que un Equipo Rojo
El equipo rojo debe documentar las observaciones clave que utiliza para alcanzar sus objetivos. Esto incluye todos los pasos importantes, exitosos y
pasos que se han dado mientras se trabaja para alcanzar un objetivo. Deben incluirse los perfiles de las amenazas u otros indicadores que el equipo azul pueda utilizar durante el
Durante el análisis posterior, deben incluirse los perfiles de amenaza u otros indicadores que el equipo azul pueda utilizar. El final de un compromiso del Equipo Rojo puede ser el comienzo de un análisis
análisis forense o el compromiso del equipo de caza. Los equipos azules que aprovechan los COIs listados en el
informe después de un compromiso a través del post-análisis pueden utilizarlo para encontrar puntos ciegos o para afinar las herramientas de seguridad para protegerse mejor contra las amenazas mediante la comparación de las herramientas de seguridad.
de seguridad para protegerse mejor contra las amenazas, comparando lo que se descubrió con lo que no se descubrió.

**Tipos de observaciones que deben documentarse

```
|---------------------------------------------------------------------------------------|
| Observación a documentar Descripción
|---------------------------------------|-----------------------------------------------|
| Acciones clave que condujeron desde | Acciones que describen cómo el acceso |
| acceso inicial al objetivo final | se obtuvo como varias fases del |
| | compromiso.                             	

| Acceso inicial
| Movimiento lateral.
| | ● Escalada de privilegios | |
|---------------------------------------------------------------------------------------|
| Mando y Control | Visión general del diseño y arquitectura del C2. 	
| | Incluir | | | Información de la red.
| | Información de la red (direcciones IP | |
| | Direcciones, nombre de dominio, puertos, | | | Protocolos, etc.
| | protocolos, etc.)                   	|
| | ● Incluir información del agente | | | | | (binarios y

| | Cambios en el registro) | | ● Incluir información del agente

|---------------------------------------------------------------------------------------|
| Acciones de reconocimiento | Pasos dados para realizar el reconocimiento | |
| | o conocimiento de la situación.               	|
| | Incluir | | Técnicas de reconocimiento.
| | Técnicas utilizadas que ayudan | | a identificar indicadores potenciales | |.
| | identificar indicadores potenciales | | | | ● Incluir técnicas utilizadas que ayuden a
| Incluir elementos clave de la información recogida.
| | Información recopilada | |
|---------------------------------------------------------------------------------------|
| Observaciones interesantes que | Los operadores suelen aprovechar |
| asistidos por el equipo rojo durante las | situaciones únicas para apoyar un |
| compromiso. Esto es a menudo no técnica |
| | en la naturaleza. Observaciones relacionadas con |
| | personas, procesos y tecnología | |
| | deben ser documentadas.                   	|
| Incluya...
| | ● Defectos lógicos encontrados en el | |

| | ● Respuesta (o falta de) de los | | | defensores.
| | defensores | |
|---------------------------------------------------------------------------------------|
| Observaciones interesantes que | Compromiso ofrecen una visión única a un |
| puede ser preocupante pero que son | gama de sistemas. Los operadores a menudo |
| no relacionados directamente con el | encuentran caminos interesantes u otras |
| compromiso | observaciones que pueden o no |
| | haber sido exploradas. Éstas deberían |
| | estar documentados.                          	
|---------------------------------------------------------------------------------------|
```
Una sola observación debe incluir los siguientes elementos (un ejemplo completo está disponible en el
sitio web complementario)

```
● El título de la observación
● Una descripción narrativa
● Detalles técnicos
        ○ Direcciones IP de origen/destino
        ○ Herramientas o técnicas
        ○ Resultados (incluidos los impactos)
● Capturas de pantalla
```
![Alt Image](./Images/29.png)

Ejemplo de observación


#### Dónde incluir las conclusiones y recomendaciones

Aunque un informe se centra en el diagrama y la narrativa del ataque, se identificarán fallos que deberían
en la sección de conclusiones del informe. Los hallazgos deben ser una lista de cuestiones críticas que ayudaron
al Equipo Rojo en el logro de sus objetivos. Entre ellos deben figurar los hallazgos tradicionales, como
falta de parches, contraseñas débiles u otros fallos comunes.

Las recomendaciones de mitigación suelen ser genéricas en esta fase. Con el fin de mejorar
recomendaciones y proporcionar consejos de mitigación que se centren directamente en la organización objetivo, debe haber
debe haber una colaboración con el Equipo Rojo y la organización objetivo para determinar la causa raíz de
los fallos de seguridad. Por desgracia, esto no siempre ocurre. Muchos Equipos Rojos proporcionan una lista de
recomendaciones, y éstas se toman como verdades básicas. Los equipos rojos deberían fomentar la realización de una
de riesgo adecuada con respecto a las mitigaciones recomendadas. Los equipos rojos sólo proporcionan una parte
de la ecuación del riesgo. Las organizaciones que utilizan un informe para llevar a cabo su propio análisis de la causa raíz a menudo están
mejor y aplican una mejora más sólida a sus operaciones de seguridad.

```
Punto de enfoque
Aunque las conclusiones y recomendaciones no son el punto central de un compromiso del Equipo Rojo ni se solicitan siempre, deberían incluirse siempre en un apéndice.
deberían incluirse siempre en un apéndice.
```
Una vez analizadas y comprendidas las observaciones, el Equipo Rojo tiene una idea de cómo le fue a la
defensa contra el ataque, pero esta comprensión es a menudo unilateral. Puede ser difícil proporcionar
recomendaciones o remedios exactos. Puede ser beneficioso proporcionar una relación en lugar de una
recomendación directa. Una relación que ofrezca una imagen global de un compromiso ayudará a
describir cómo las mejoras aumentarán la seguridad.

![Alt Image](./Images/30.png)

Los detalles de este ejemplo no son importantes. El mapeo de la observación a la recomendación en
en relación con la pirámide del dolor es el objetivo. La izquierda de la imagen muestra las observaciones del equipo rojo
observaciones del equipo rojo en relación con la capacidad de la defensa para impactar en las acciones de la amenaza. En este momento se encuentra en Easy.
La derecha de la imagen describe el problema y proporciona una recomendación. Si la organización objetivo
implementa la recomendación, el equipo rojo estima la postura defensiva y el impacto a la
amenaza. En este caso, a desafiante o molesto.
Los informes no necesitan mostrar explícitamente este diagrama, pero el concepto debe entenderse en
el contexto del informe. Tenga en cuenta que, al igual que con el diagrama de ataque, las imágenes ayudan a la comprensión. Incluir elementos visuales
junto con el texto, aumenta drásticamente las posibilidades de ingestión y aplicación.


### Conclusiones clave del capítulo

Un informe de compromiso del equipo rojo es la última y única prueba de un compromiso del equipo rojo.
Estos informes pueden ser muy diferentes de otros informes de seguridad. Los informes deben centrarse en la narrativa del ataque
Los informes deben centrarse en la narrativa del ataque y destacar las observaciones clave realizadas por los operadores durante la ejecución de la intervención.

Aplicar una calificación de riesgo puede ser difícil, ya que las observaciones del equipo rojo suelen ser unilaterales. Considere la posibilidad de
considerar la posibilidad de aplicar las calificaciones trabajando directamente con un equipo de riesgo o con individuos del equipo de operaciones de seguridad.
de seguridad. Utilice estos consejos para aplicar una calificación en los casos en que el equipo rojo proporcione una calificación.  
```
● Utilice una sección de observaciones para apoyar la narración del ataque
● Utilice una sección de hallazgos para rastrear y definir las fallas técnicas
● Aplicar la técnica de calificación de tres niveles para las observaciones
● Aplicar una técnica de calificación de 5x5 para los hallazgos técnicos
```

### Tarea para casa
```
1. Elaborar una plantilla de informe personalizada  
2. Crear una colección de observaciones para permitir una redacción coherente al informar sobre observaciones repetidas en la narración del ataque.  
3. Crear una sección de hallazgos para rastrear los hallazgos técnicos (similar a un informe de prueba de penetración).  
4. Desarrollar una plantilla de diagrama de flujo de ataque.  
5. Desarrollar una plantilla de narración del flujo de ataque.  
```

## Resumen

El Red Teaming es el proceso de utilizar Tácticas, Técnicas y Procedimientos (TTPs) bien definidos para
emular una amenaza del mundo real con el objetivo de entrenar y medir la eficacia de las personas
procesos y tecnología utilizados para defender un entorno.

Se debe hacer hincapié en los impactos de las operaciones de la amenaza frente a las vulnerabilidades que la posibilitan.
Las vulnerabilidades serán descubiertas y aprovechadas; sin embargo, las debilidades encontradas son un subproducto de
de un equipo rojo, no el objetivo. Los resultados de los equipos rojos deben ser mucho más que una simple lista de
defectos identificados. Proporcionan una comprensión más profunda de cómo actuaría una organización contra
una amenaza real. El valor real de un Red Team es ayudar a un objetivo a identificar controles administrativos, técnicos y
y procedimentales que limitan directamente la capacidad de una amenaza para causar impactos negativos. Incluso cuando
vulnerable a la última "vulnerabilidad de día cero". En consecuencia, los impactos operativos proporcionan una verdadera
de la capacidad de las operaciones de seguridad para proteger, detectar, responder o recuperarse de una variedad de
amenazas.

¿Se ha dado cuenta de que la planificación del compromiso es bastante más larga que la ejecución, la culminación y la elaboración de informes?
Hay un método para esa locura. La planificación del compromiso es crucial para gestionar los riesgos potenciales del compromiso
de compromiso, ejecutar con éxito las metas y objetivos deseados y proporcionar la información necesaria para mejorar la organización y la defensa.
necesaria para mejorar las capacidades organizativas y defensivas. En resumen, es casi imposible
llevar a cabo un compromiso profesional y exitoso sin comprender plenamente los objetivos y el alcance,
comprender los recursos necesarios para la ejecución y crear un plan sólido. Asimismo, una planificación
planificación eficaz aumenta considerablemente la velocidad y la precisión de la culminación del compromiso y de los informes.
de los informes. Nunca se insistirá lo suficiente en la importancia de la planificación del encargo.

Los entregables (informes) permiten a la organización reproducir las acciones y los resultados del equipo rojo.
Son la última forma de evidencia que puede ser analizada y utilizada para proporcionar una base para mejorar
seguridad. Deben incluirse como entrega final de un compromiso.

Por último, nos gustaría destacar nuestro mantra común. "Si no hay registro, no hubo acción. Si no hay
Si no hay informe, no hay compromiso". Los operadores y jefes de los equipos rojos deberían tomarse esto a pecho y
animarse mutuamente a documentar sus acciones adecuadamente.

```
http://redteam.guide
No olvides visitar el sitio web complementario, http://redteam.guide, para obtener información adicional, plantillas de equipos rojos y otras guías.
```

## Conclusión

Queremos agradecerle que se haya tomado el tiempo de leer este contenido. Por supuesto, la lectura es sólo un paso en
sus esfuerzos. También es esencial absorber, procesar y comprender las lecciones y los conceptos que se presentan.
presentados. Si no lo ha hecho mientras leía, le recomendamos que trabaje con los deberes.
La mejor manera de aprender y mejorar estos conceptos es ponerlos en práctica.

Se han necesitado años de investigación, experimentación (también conocida como prueba y error) y ejecución para discernir qué
elementos deben y no deben formar parte de este texto. Nuestro objetivo era ofrecer una orientación práctica para
para ayudarle a usted, o a su equipo, en el desarrollo, la gestión y la ejecución de un equipo rojo profesional.
Se podrían escribir volúmenes y volúmenes sobre cada tema individual; sin embargo, hemos intentado
escribir según la regla del 80/20. El ochenta (80) por ciento de lo que ve, oye y experimenta es la información menos valiosa.
información menos valiosa. Este texto cubre lo que creemos que es el veinte (20) por ciento del desarrollo y las operaciones de los equipos rojos que tiene más valor.
Desarrollo y Operaciones de Equipos Rojos que tiene el mayor valor. No sólo le hará un mejor Red Teamer,
sino que también debería proporcionar un medio para racionalizar sus esfuerzos y aliviar su carga de trabajo. En definitiva,
mejorar (hacer las cosas mejor) y disfrutar en el proceso es lo que más cuenta. De nuevo,
¡gracias!


## Apéndice A: Ejemplos de plantillas

Las plantillas y los ejemplos se pueden encontrar en el sitio web complementario, [http://redteam.guide.](http://redteam.guide.)


## Apéndice B: Ejercicios de reflexión

### Desafío de la mentalidad adversaria

**Descripción**  
En este ejercicio, completará rápidamente una serie de desafíos de rompecabezas diseñados para fomentar el pensamiento crítico en un corto período de tiempo.
pensamiento crítico en poco tiempo. Está diseñado para ser una forma divertida de empezar a comprender las habilidades
necesarias para planificar y ejecutar un plan de equipo rojo.

**Instrucciones  
Siga las instrucciones de cada rompecabezas  
Establezca un tiempo y complete los rompecabezas en 5 minutos.

**Para aquí y prepárate para empezar cuando estés listo**


#### Puzzle de 9 puntos

Instrucciones:
Colocando el bolígrafo en la página una sola vez, dibuja cuatro líneas rectas que pasen por los nueve puntos
sin levantar el bolígrafo de la página.

![Alt Image](./Images/31.png)

#### Desafío del laberinto

Instrucciones:
Dibuja una línea desde el portátil hasta el centro de datos.

![Alt Image](./Images/32.png)

#### Puzzle de triángulos

Instrucciones:
Cuenta los triángulos. ¿Cuántos se muestran?

![Alt Image](./Images/33.png)

#### Rompecabezas de palabras

Instrucciones:
Escribe tu explicación a la siguiente historia.

Un hombre entra en un bar y le pide al camarero un vaso de agua. El camarero saca una pistola y
apunta al hombre. El hombre dice "gracias" y se va.


#### Procesamiento del pensamiento alternativo

Instrucciones:
Contempla lo siguiente y piensa en las áreas en las que los conceptos erróneos o los prejuicios comunes influyen en la forma en que se implementa o aborda la seguridad en tu organización.
seguridad se implementa o se aborda en tu organización.

Dado que los puntos rojos son zonas en las que los aviones de combate suelen ser alcanzados durante el combate, ¿qué indica el
siguiente diagrama? ¿Cuáles serían sus recomendaciones para el blindaje adicional de la
de la aeronave?

![Alt Image](./Images/34.png)


### Comentarios y Respuestas del Desafío de la Mente

#### Desafío de 9 puntos

Posibles respuestas.

![Alt Image](./Images/35.png)

¿Se te ocurrió algo diferente? El objetivo de este ejercicio es apoyar la frase "pensar
fuera de la caja". No te limites a lo que se presenta y céntrate en medir lo que "Es" frente a lo que
"Debería ser".

#### Desafío del laberinto

Posibles respuestas

![Alt Image](./Images/36.png)

¿Cómo se compara su solución? El objetivo de este ejercicio es similar al anterior. No dejes que
suposiciones y limitaciones impidan las posibles soluciones. Un buen Red Teamer es capaz de entender y
de entender y modificar las reglas de formas que no siempre se tienen en cuenta.


#### Rompecabezas triangular

Respuesta: Total de triángulos = 27

Cuando te enfrentas a un problema para el que no conoces la "fórmula", puede ser necesario un enfoque de fuerza bruta
necesario un enfoque de fuerza bruta. Se pueden aprender lecciones, y las "fórmulas" se pueden añadir a tu base de conocimientos para mejorar
eficiencia cuando te enfrentes a problemas similares en el futuro.

Fórmula:
T(n) = floor(n*(n + 2)*(2n + 1) / 8)

Ejemplo:
f(4) = 4*(4 + 2)*(2*4 + 1) / 8 = 27.000

```
Referencia:
http://www.billthelizard.com/2009/08/how-many-triangles.html
```
#### Rompecabezas de palabras

Este es un rompecabezas de pensamiento lateral común. Este tipo de rompecabezas suele dar al público un conjunto de circunstancias aparentemente
circunstancias inusuales en las que deben intentar averiguar qué ha pasado o qué ocurre en
una historia corta e inusual. Esto ayuda a mostrar cómo los retos difíciles a menudo pueden ser resueltos con soluciones fáciles.
soluciones fáciles.

Solución clásica:
El hombre tenía hipo y quería un vaso de agua para quitárselo. El camarero pudo
El camarero oía el hipo cuando el hombre hablaba, así que sacó la pistola para espantar el hipo. Funcionó,
y el hombre le dio las gracias y se fue, sin necesitar más el vaso de agua.

¿Cómo se comparó su respuesta con la solución clásica?

#### Procesamiento del pensamiento alternativo

Durante la Segunda Guerra Mundial, la Armada de los Estados Unidos realizó una revisión de los aviones con encuentros de combate. Esta
revisión pretendía determinar en qué casos los aviones necesitaban un blindaje adicional para garantizar la supervivencia y el
retorno. Tras el análisis, la Marina decidió que todos los lugares en los que se encontraron agujeros de bala debían ser
mejor blindaje ya que son más propensos a ser golpeados. Estos incluyeron las puntas de las alas, el cuerpo central,
y los elevadores.

Un estadístico de la Marina, Abraham Wald[27] tenía otra teoría. Las áreas con agujeros de bala identificaban
donde la aeronave ya era sobrevivible. Recomendó blindar el morro, el motor y el cuerpo central
aunque pocos de los aviones tenían daños en esas áreas. ¿Por qué?

Wald reconoció que esas zonas también recibían disparos; sin embargo, no eran capaces de regresar con seguridad. Él
conjeturó correctamente que los aviones con disparos en las alas, el cuerpo central y los elevadores pudieron


mientras que los que tenían disparos en el morro, el motor y la parte central del cuerpo estaban catastróficamente dañados y
y no pudieron regresar.

Considere cómo se traduce este escenario al Red Teaming o a la seguridad en general. Considere también lo que se sabe
También hay que tener en cuenta lo que se sabe (y lo que se desconoce) a partir de la información de inteligencia sobre amenazas, los acontecimientos actuales y los indicadores.


## Apéndice C: Ejercicio de descomposición de una amenaza

### Descripción

Este ejercicio recorre el proceso de descomponer una amenaza y un escenario de amenaza para construir un perfil de amenaza.
perfil de la amenaza. Se examinará el actor de la amenaza Oso Energético para desarrollar un perfil de amenaza que pueda ser utilizado
durante un compromiso del Equipo Rojo.
**Objetivos
1. Revisar las TTPs del actor de la amenaza Energetic Bear.
2. 2. Utilizar la información para crear una amenaza que sea similar y que pueda ser utilizada para apoyar futuros
compromisos del Equipo Rojo.
3. Completar una plantilla de perfil de amenaza


### Escenario del ejercicio

Un cliente ha pedido a su Red Team que emule una amenaza específica. En concreto, están interesados en los
ataques de Energetic Bear.


### Objetivo

El objetivo de este ejercicio es crear un documento de perfil de amenaza utilizando a Energetic Bear como inspiración.
Como equipo rojo profesional, entiendes que emular a un actor de amenaza específico no es fácil o
factible, y que centrarse en las TTPs de la amenaza es más relevante. Utilizarás la investigación sobre las TTP de Energetic Bear
TTP de Energetic Bear para construir un perfil de amenaza personalizado que sea técnicamente factible y que pueda ser utilizado para comprometer al cliente
con una amenaza realista.


### Recursos

```
● MITRE ATT&CK Framework (https://attack.mitre.org/wiki/Main_Page)
● MITRE ATT&CK Navigator (https://attack.mitre.org/wiki/ATT%26CK_Navigator)
● Dragonfly: Ataques de ciberespionaje contra proveedores de energía
(http://www.symantec.com/content/en/us/enterprise/media/security_response/whitepapers/Dragonfly_Threat_Against_Western_Energy_Suppliers.pdf)
● Energetic Bear - Crouching Yeti (https://media.kasperskycontenthub.com/wp-
content/uploads/sites/58/2018/03/09092926/EB-YetiJuly2014-Public.pdf)
● El callejón del compromiso (https://www.crowdstrike.com/blog/cve-2014-1761-alley-
compromiso)
```

### Comenzar el Ejercicio

Comienza investigando la amenaza y el ataque del Oso Energético. Después de completar la suya, compare
tus observaciones con los puntos destacados que aparecen a continuación.

Los puntos destacados se han proporcionado para ayudar en este proceso.

#### Aspectos destacados del actor de la amenaza del oso energético
```
● Desde 2010 y hasta 2014, el malware Energetic Bear / Dragonfly / Crouching Yeti
atacó numerosos ordenadores para recopilar información sobre los sistemas de control industrial en los
Estados Unidos y Europa
● Se extendió en el tiempo y, por lo tanto, es difícil de detectar
● El objetivo principal era recopilar información que afectara a las industrias energética y farmacéutica
● Posiblemente apoyado por un estado-nación
● Ataques de suplantación de identidad, watering hole.
Se utilizaron exploits conocidos (PDF, Java, IE, Word)
● Servidores web de ICS comprometidos
● C2 basado en HTTP
Actividades y capacidades específicas
```
IOCs del actor Energetic Bear y del malware HAVEX

![Alt Image](./Images/37.png)

**Actor**
```
● Asociado a la Federación Rusa
Activo durante varios años
● Activo principalmente durante el horario comercial de Moscú
● Dirigido a organizaciones basadas en el sector de los sistemas de control industrial vObjetivo de reunir información de inteligencia sobre organizaciones basadas en ICS
● Uso de malware personalizado
```

**Ataque y entrega de TTPs**
```
● Phishing
● Watering hole
● Servidores web comprometidos
```

**TTPs de Explotación
```
● Explotaciones de PDF
● Explotaciones de Java e IE
● Explotaciones de Word2
● Binarios personalizados
```

**TTPs post-explotación**
```
● Enumeración del sistema local para el sistema operativo, nombre de usuario, procesos, historial de Internet, etc.
● Escaneo de puertos conocidos relacionados con ICS
● Inyección de DLL para migrar a explorer.exe
● Recoger información de la libreta de direcciones de Outlook
● Recoger contraseñas de los navegadores
● Guardar los datos exfiltrados en un archivo encriptado en el disco antes de entregarlos al C2 en una petición HTTP POST
```

**TTPs de persistencia**  
Ejecutar modificaciones en el registro de claves:  
```
HKEY_CURRENT_USER\NSoftware\NMicrosoft\Windows\NCurrentVersion\NRun\N "TmProvider"
HKEY_LOCAL_MACHINE\NSOFTWARE\NMicrosoft\NWindows\NCurrentVersion\Nejecutar "TmProvider"
HKEY_LOCAL_MACHINESOFTWARE\Microsoft\NInternet Explorer\NInternetRegistry\N "fertger"
HKEY_LOCAL_MACHINE\NSOFTWARE\NMicrosoft\NInternet Explorer\NInternetRegistry
```

**Entrega de la carga de pago de SHAVEX**

![Alt Image](./Images/38.png)

```
Energetic Bear utilizó tres métodos principales para entregar el malware.
1) PDF malicioso a través de spear-phishing El spear-phishing se utilizó para infectar a los individuos objetivo
para la recopilación inicial de información mediante la entrega de documentos PDF maliciosos, en este caso,
PDF/SWF dirigidos a CVE-2011-0611 para lanzar el malware3 .
hasta 2014, los exploits más antiguos seguían siendo valiosos.  
2) JAR y HTML maliciosos a través de un ataque de agujero de riegoLos ataques de agujero de riego se utilizaron para
para distribuir Backdoor.Oldrea de Symantec. Estos ataques explotaron CVE-2013-2465, CVE-
2013-1347 y CVE-2012-1723 en Java 6, Java 7, IE 7 e IE 8 para lanzar el malware HAVEX
. El malware HAVEX. Los exploits parecían ser exploits Metasploit Java modificados construidos para entregar
el cargador HAVEX.  
3) Cargadores de software legítimos Energetic Bear comprometió varios sitios web legítimos de proveedores de ICS
legítimos de ICS. Los binarios, como los controladores de cámaras y el software de gestión de PLC, fueron modificados
y se hicieron para entregar el malware HAVEX.
```

Para completar el tercer tipo de ataque, el actor de la amenaza tuvo que comprometer los sitios web de varios proveedores de ICS.
proveedores de ICS. Estos ataques, a veces denominados ataques de compromiso estratégico de la web (SWC), se han convertido en uno de los métodos de ataque favoritos de rusos y chinos.
método de ataque favorito de las amenazas rusas y chinas. En este caso, los ataques SWC se utilizaron
para comprometer un sitio que probablemente sea visitado por clientes o usuarios de sistemas ICS. Este
Esto hizo que el agujero de riego o los compromisos binarios fueran mucho más útiles contra la víctima objetivo. A través de
Estos tres tipos de ataque demostraron la existencia de un actor de amenazas organizado y posiblemente sofisticado. El equipo
detrás de esto planificó y organizó un escenario para tener éxito contra su público objetivo.

Una vez entregado el malware, se observaron tres tareas principales:
```
Las herramientas de enumeración del sistema recopilaban información, como la versión del sistema operativo, el nombre de la máquina y el nombre de usuario, y los listados de archivos y directorios.  
Una herramienta de recolección de credenciales extraía las contraseñas almacenadas en varios navegadores web.
● Los implantes secundarios6 se comunicaban con diferentes infraestructuras C2 mediante protocolos personalizados y cargas útiles ejecutadas en memoria.
```

**Ejemplo de solicitud HTTP deHAVEX  
Solicitud POST**
```
POST /wp08/wp-includes/dtcla.php?id=285745296322896178920098FD80-20&v1=038&v2=170393861&q=5265882854508EFCF958F979E4 HTTP/1.1
Usuario-Agente: Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US)
AppleWebKit/525.19(KHTML, como Gecko) Chrome/1.0.154.36 Safari/525.19
Alojamiento: toons.freesexycomics.com
Contenido-Longitud: 0
Cache-Control: no-cache
```

**Respuesta de los correos**
```
HTTP/1.1 200 OK
Fecha: Wed, 22 Jan 2014 13:40:48 GMT
Content-Type: text/html
Transfer-Encoding: chunked
Conexión: keep-alive
Servidor: Apache/1.3.37 (Unix)
Cache-Control: no-cache

9f65
<html><head><mega http-equiv='CACHE-CONTROL' content='NO-CACHE'></head><body>¡Sin datos!
havexQlpoOTFBWSZTWYvDI0BOsD/////////////////////////////////////////////4oB+93VXu69DuN7XYzds9yt49Ques
[...TRUNCADO ...]
+yUW3zfTxWAOstsCwCckdW5 AH5Q6vbbCu7GputPt5CSfgPCAKXcAOOICMsqliACGYEhAQT3v9eD
M92D/8XckU4UJBmLwyNA==havex--></body></head>
```

En este ejemplo de Symantec, se pueden identificar varios indicadores.

La solicitud POST muestra varios indicadores que pueden incorporarse a una amenaza emulada:
```
● Un archivo PHP de destino (dtcla.php)
● Parámetros de URL interesantes (id, v1, v2, q)
● Un User-Agent potencialmente interesante
Un host de destino
```

Al igual que la petición, la respuesta tiene varios indicadores:
```
● Una cabecera del servidor
● Un ID potencialmente único (9f65)
● Datos codificados en base64 almacenados entre texto (havex < base64 > havex)
```

Nota: MALWAREMUSTDIE2 publicó un gran artículo sobre el malware HAVEX. Esto proporciona
ejemplos adicionales de código fuente C2 y pares de solicitud/respuesta HTTP. Referencia:
[http://pastebin.com/qCdMwtZ6](http://pastebin.com/qCdMwtZ6)


### Crear un perfil de amenaza

1) Utiliza la investigación que has realizado y esta información para crear un perfil de amenaza. No hay una respuesta correcta o
respuesta incorrecta. Los componentes importantes de un perfil de amenaza son la viabilidad técnica, la capacidad de cumplir
objetivos de compromiso, y la capacidad de implementación utilizando las herramientas y la capacidad de su Equipo Rojo.

Consejos
```
Los perfiles deben ser técnicamente viables. Si su perfil requiere el uso de días cero, asegúrese de que puede cumplirlo. (el uso de tarjetas blancas y los modelos de infracción asumidos pueden ayudar)  
● Los perfiles de amenazas se implementan como parte del plan C2. Influyen directamente en la selección y configuración del C2. Tenga siempre en cuenta las capacidades y limitaciones técnicas de sus plataformas C2 al diseñar un perfil  
```

2) Desarrolle su perfil utilizando la siguiente plantilla y compárela con la posible solución.

![Alt Image](./Images/39.png)

### Posible solución

![Alt Image](./Images/40.png)

**Piensa en las siguientes preguntas:**

¿Cómo se compara su solución?  

¿Tienes la capacidad técnica para ejecutar este perfil?  

¿Copiaste las técnicas exactas del ejemplo de referencia o rellenaste los huecos con otras técnicas?  

¿Está preparado para explorar técnicas desconocidas para imitar mejor el ejemplo de referencia?  


## Glosario de términos

**Supuesto incumplimiento**  
El modelo de presunta violación supone que una amenaza tiene cierto nivel de acceso a un objetivo al inicio del
el compromiso.

Este modelo es posiblemente el más beneficioso de todos los modelos. Se supone que la amenaza tiene cierto nivel de acceso al objetivo antes de comenzar el combate.
nivel de acceso a un objetivo antes de comenzar. Esto hace que el escenario comience mucho más adelante en la línea de tiempo del ataque.
línea de tiempo. Asumir que alguien puede vulnerar una red es algo que a menudo argumentan las organizaciones menos maduras.
A los que dicen "pruébalo" no les suele gustar este escenario. Las organizaciones menos maduras asumen que
las amenazas deben demostrar que pueden entrar antes de empezar. ¿Cuándo es importante la prueba? Sólo es importante
si es importante medir la capacidad que tiene una amenaza para "entrar". Si este no es un objetivo clave, utilizar el modelo de presunta
Breach Model ahorrará tiempo y dinero. Liberará al Equipo Rojo para explorar objetivos de mayor impacto.

**Célula azul**  
La celda azul es el lado opuesto a la roja. Son todos los componentes que defienden una red objetivo. La célula azul
La célula azul suele estar compuesta por miembros del equipo azul, defensores, personal interno y la
gestión.

**Equipo azul**  
Es el equipo de seguridad que defiende contra las amenazas.

**Mando y control (C2)**  
El mando y control (C2) es la influencia que un atacante tiene sobre un sistema informático comprometido que
que controla.

**Niveles de C2  
El diseño de una infraestructura C2 robusta implica la creación de múltiples capas de Mando y Control.
Éstas pueden describirse como niveles. Cada nivel ofrece un nivel de capacidad y cobertura. La idea de
La idea de utilizar varios niveles es la misma que la de no poner todos los huevos en la misma cesta. Si el C2 es detectado y
Si el C2 es detectado y bloqueado, tener una copia de seguridad permitirá que las operaciones continúen.

Los niveles de C2 se dividen generalmente en tres categorías: Interactivo, de corto recorrido y de largo recorrido. Estos son
a veces etiquetados como Nivel 1, 2 o 3. No hay nada único en cada nivel, aparte de cómo deben utilizarse.
utilizar.

Nivel interactivo
```
Utilizado para comandos generales, enumeración, escaneo, exfiltración de datos, etc.
● Este nivel tiene la mayor interacción y corre el mayor riesgo de exposición.
● Planifique la pérdida de acceso por fallo de comunicación, fallo del agente o acciones del Equipo Azul.
● Ejecute suficientes sesiones interactivas para mantener el acceso. Aunque sea interactivo, esto no significa
significa bombardear al cliente con paquetes. Utilice el buen criterio para minimizar la interacción lo suficiente
suficiente para realizar una acción.
```

Niveles de corto alcance
```
● Se utiliza como respaldo para restablecer las sesiones interactivas.
● Utiliza comunicaciones encubiertas que se mezclan con el objetivo.
● Tiempos de devolución de llamadas lentos. Los tiempos de devolución de llamadas en el rango de 1 a 24 horas son comunes.
```

Nivel de larga distancia
```
- Lo mismo que en Short Haul pero aún más bajo y lento.
- Tiempos de devolución de llamadas lentos. Los tiempos de devolución de llamadas de más de 24 horas son comunes.
```

**Deconflicción**  
La desconflicción es la capacidad de identificar qué actividad es generada por un Equipo Rojo y cuál no. En
En general, la desconflicción proporciona una forma de separar la actividad del Equipo Rojo de la actividad del mundo real
a través de un proceso controlado.

**Grupo de Control de Compromiso/Ejercicio (ECG)**  
El Grupo de Control del Compromiso (o del Ejercicio) es el responsable último de todas las actividades realizadas
durante el compromiso. La mayoría de las veces, el Grupo de Control del Compromiso está compuesto por uno o dos altos
de alto nivel del entorno de destino (por ejemplo, un director de información o un director de operaciones), un miembro del departamento de información y un director de operaciones.
de Operaciones), un miembro del departamento de Tecnología de la Información del entorno, un enlace de la Célula Blanca
y un enlace del Equipo Rojo. Se pueden añadir más si es necesario. Todos deben ser agentes de confianza.

**Exfiltración**  
La exfiltración es la extracción de información de un objetivo. Esto es típicamente a través de un canal encubierto.

**Entrar, permanecer, actuar  
Las tres fases principales de un compromiso del Equipo Rojo.

```
Entrar  
Obtener acceso a una red. El Equipo Rojo debe tener acceso a su objetivo. El acceso puede ser
a través de un compromiso legítimo o el acceso se concede directamente como parte de un supuesto escenario de violación
como un escenario de amenaza interna.
```
```
Permanecer  
Establecer una persistencia o una presencia permanente. Los compromisos de los equipos rojos suelen ser más largos
que otros tipos de pruebas. Un equipo rojo suele establecer una persistencia o una presencia permanente
presencia permanente para sobrevivir a la duración del compromiso.
```
```
Actuar  
Fase en la que un Equipo Rojo realiza impactos operativos contra un objetivo.
```
**Indicadores de Compromiso (IOC)  
Los indicadores de compromiso (IOC) son artefactos que identifican o describen las acciones de la amenaza.


**OPFOR**  
Una fuerza opositora, o fuerza enemiga, que suele ser utilizada por los militares en los escenarios de juegos de guerra.
Los Equipos Rojos están comúnmente asociados o apoyan a una OPFOR en escenarios de juegos de guerra.

**OPLOG (Registro del Operador)**  
Los registros del operador son los registros generados por los operadores del Equipo Rojo durante un compromiso. Estos registros
Estos registros tienen campos específicos y obligatorios que deben ser capturados.

**Impacto operativo**  
Un impacto operacional es el efecto de una acción orientada a un objetivo dentro de un entorno objetivo.

**OPSEC  
OPSEC o Seguridad Operacional es un proceso que identifica la información crítica para determinar si
acciones amigas pueden ser observadas por la inteligencia enemiga, determina si la información obtenida por
adversarios podría ser interpretada como útil para ellos, y luego ejecuta medidas seleccionadas que
eliminar o reducir la explotación de la información crítica amiga por parte del adversario. En términos de Red Teaming
es entender qué acciones puede observar el Azul y minimizar la exposición.

**Informe, Ejecutivo**  
La primera reunión posterior al compromiso suele ser el informe ejecutivo. El briefing ejecutivo se realiza normalmente
Una reunión ejecutiva suele realizarse poco después de la ejecución (en uno o dos días después de la ejecución). Esta reunión
Esta reunión está dirigida a la dirección y debe incluir al personal clave de la organización objetivo. El
El resultado de una intervención del equipo rojo puede afectar al funcionamiento de la organización en el futuro,
y puede requerir financiación para llevar a cabo mitigaciones o modificaciones de personal. La concienciación de la dirección
La concienciación y el compromiso de la dirección son fundamentales si los resultados del equipo rojo se utilizan para mejorar la posición de seguridad de la organización
para defender y responder a una amenaza.

**Informe técnico  
El outbrief técnico (también conocido como tech-on-tech) es un intercambio bidireccional de información técnica
entre el Equipo Rojo, el Equipo Azul y la organización. Durante este intercambio, tanto el Equipo Rojo como
los elementos defensivos proporcionan una revisión técnica muy detallada, paso a paso, de las acciones y
resultados (incluyendo todos los detalles asociados) del compromiso. Aquí es donde se unen la formación y la educación
y es una de las oportunidades más valiosas para que todas las partes aprendan.

**Persistencia**  
La persistencia es la capacidad o las técnicas utilizadas para establecer una presencia permanente con el fin de sobrevivir a la
duración del compromiso.

**Preposicionamiento**  
El preposicionamiento es el proceso de utilizar el acceso y las capacidades adquiridas durante un compromiso para
de un compromiso para posicionar mejor a un operador para la ejecución de un impacto.

**Célula roja  
El término "célula roja" procede del ámbito militar. Se asocia comúnmente a un grupo que desempeña
OPFOR (fuerza opositora) durante los ejercicios de rojo contra azul. Una célula roja son los componentes que conforman la
parte ofensiva de un compromiso del equipo rojo que simula las respuestas estratégicas y tácticas de un
objetivo determinado. La célula roja se compone normalmente de los líderes y operadores del equipo rojo y se denomina comúnmente
se denomina Equipo Rojo en lugar de Célula Roja.

**Equipo Rojo**  
Un equipo rojo es un grupo independiente que, desde la perspectiva de una amenaza o adversario, explora
planes y operaciones alternativas para desafiar a una organización y mejorar su eficacia.

**Jefe del Equipo Rojo  
Sirve como líder operativo y administrativo del Equipo Rojo. Dirige el compromiso, el presupuesto
y gestión de recursos para el Equipo Rojo.
Supervisa y orienta los compromisos, las capacidades y las tecnologías. Garantiza que
Garantiza el cumplimiento de todas las leyes, reglamentos, políticas y normas de intervención.

**Operador del Equipo Rojo  
Cumple con todos los requisitos del Equipo Rojo bajo la dirección del Jefe del Equipo Rojo. Operativo
Ejecuta el compromiso. Aplica las TTPs del Equipo Rojo al compromiso. Proporciona investigación técnica
y capacidad al Equipo Rojo. Lleva un registro detallado durante cada fase de la intervención. Proporciona
soporte de registro e información para la creación del informe final

**Reglas de actuación (ROE)**  
Las Reglas de Compromiso establecen las responsabilidades, relaciones y directrices entre el Red Team, el cliente, el propietario del sistema y la empresa.
El equipo rojo, el cliente, el propietario del sistema y las partes interesadas necesarias para la ejecución de la intervención.

**Conciencia de la situación**  
El conocimiento de la situación es un paso en el compromiso del Equipo Rojo que se utiliza para reunir toda la información necesaria
sobre los objetivos y el entorno objetivo. La información recopilada se utiliza para determinar las siguientes acciones
hacia la escalada de privilegios, el movimiento lateral u otros pasos. Es un componente clave del Red Teaming
Es un componente clave del Red Teaming y debe realizarse en algún nivel en todos los objetivos de acceso.

**Amenaza**  
Una amenaza es una expresión de intención de infligir un mal, una lesión o un daño.

**Emulación de amenazas  
Emulación de amenazas La emulación de amenazas es el proceso de imitar las TTPs de una amenaza específica.

**Inteligencia sobre amenazas  
La inteligencia sobre amenazas es la información que ha sido agregada, transformada, analizada, interpretada o
La inteligencia sobre amenazas es la información que ha sido agregada, transformada, analizada, interpretada o enriquecida para proporcionar el contexto para los procesos de toma de decisiones sobre las amenazas.

**Modelo de amenaza  
Un modelo de amenaza es el proceso mediante el cual se pueden identificar, enumerar y mitigar las amenazas potenciales o la ausencia de salvaguardias apropiadas.
de las amenazas potenciales o de la ausencia de salvaguardias apropiadas, y en el que se pueden priorizar las mitigaciones.


**Perspectiva de la amenaza  
La perspectiva de una amenaza es el punto de vista inicial de la misma. Esta perspectiva se utiliza para construir y dar forma a
un perfil o escenario de amenaza. La perspectiva de una amenaza puede ser la de una persona ajena, cercana o interna.

**Perfil de la amenaza  
El perfil de la amenaza se utiliza para establecer las reglas de actuación del Equipo Rojo. Estas reglas
Estas reglas sirven como hoja de ruta para un Equipo Rojo al guiar cómo y qué tipo de acciones deben realizarse.
Los perfiles de amenaza son una parte clave del desarrollo y diseño del C2 al principio de la planificación del Equipo Rojo.

**Escenario de amenaza**  
Los escenarios proporcionan una visión de cómo una solución defensiva actuará y se ajustará a los procesos,
procedimientos, políticas, actividades, personal, organizaciones, entorno, amenazas, limitaciones,
supuestos, y el apoyo involucrado en la misión de seguridad. Los escenarios suelen describir el papel de
la amenaza, cómo interactuará con los sistemas y redes dentro del entorno objetivo, y
suscita la verdad del mundo real sobre cómo se emplean las prácticas internas esenciales. En resumen, responde a cómo las
operaciones de seguridad del objetivo realizarían dinámicamente una acción para obtener resultados, productos o demostrar
capacidad.

**Tradecraft**  
El oficio del espionaje son las técnicas y procedimientos del espionaje. El arte del oficio se asocia normalmente con la
comunidad de inteligencia. TTPs y Tradecraft se utilizan indistintamente en este curso.

**Agente de confianza (AT)   
El papel principal del Agente de Confianza es limitar el daño irreversible y el riesgo para la vida, las extremidades, la vista y el equipo.
equipo; sin embargo, se utilizan más a menudo para evitar que los defensores causen un daño autoinfligido inesperado.
daños inesperados.
Un Agente de Confianza (AT) tiene un conocimiento privilegiado y detallado de las actividades del compromiso, los hitos
condiciones, y el estado del compromiso que podría sesgar o influenciar indebidamente las acciones del
personal del entorno y los defensores. Un Agente de Confianza debe proteger toda la información para que no sea proporcionada a
cualquier parte sin la aprobación expresa del Grupo de Control de la Intervención.

**TTPs**  
Los TTPs son Tácticas, Técnicas y Procedimientos (a veces llamados Herramientas, Técnicas y Procedimientos).

**Integridad de dos personas (TPI)**  
La integridad de dos personas se utiliza para verificar las actividades realizadas durante el compromiso y debe ser
mantenerse en todo momento. Un miembro del equipo debe revisar, comprender y proporcionar una "comprobación de cordura" para
cada acción/comando realizado. Las TPI reducen los riesgos personales y del compromiso.

**Shell de la web**  
Un shell web es una pieza de código web que se coloca en un servidor web para permitir a un adversario utilizar el
servidor web como una puerta de entrada a la red. Las web shells se despliegan comúnmente como parte de un ataque de seguridad a una aplicación.
ataque de seguridad.

**Célula blanca  
Sirve de árbitro entre las actividades del Equipo Rojo y las respuestas del defensor durante un compromiso.


Controla el entorno/red de la intervención. Supervisa el cumplimiento de las normas de conducta. Coordina
actividades necesarias para alcanzar los objetivos del enfrentamiento. Correlaciona las actividades del Equipo Rojo con las acciones
defensivas. Garantiza que el compromiso se lleve a cabo sin prejuicios hacia ninguno de los bandos.

[1] "Office Space (1999) - IMDb". https://www.imdb.com/title/tt0151804/.  
[2] "Threat | Definition of Threat at Dictionary.com". https://www.dictionary.com/browse/threat.  
[3] "ISO IEC 27000 2014 Information Security Definitions - Praxiom." https://www.praxiom.com/iso-27000-definitions.htm.  
[4] "Amenaza - Glosario | CSRC - NIST Computer Security Resource ...." https://csrc.nist.gov/glossary/term/threat.  
[5] "Revivir el DDE: usar OneNote y Excel para la ejecución de código ...." 29 de enero de 2018, https://enigma0x3.net/2018/01/29/reviving-dde-using-onenote-and-excel-for-code-execution/.  
[6] "Hashdump sin el DC usando DCSync (porque todos ...." 2 oct. 2015, https://silentbreaksecurity.com/invoke-dcsync-because-we-all-wanted-it/.  
[7] "CVE-2017-0144 - The MITRE Corporation". https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-0144  
[8] "NIST SP 800-53 - Página del NIST". 4 abr. 2013, https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf.  
[9] "PCI Security Standards Council". https://www.pcisecuritystandards.org/.  
[10] "Health Information Privacy | HHS.gov." https://www.hhs.gov/hipaa/index.html.  
[11] "Cybersecurity Framework | NIST." https://www.nist.gov/cyberframework.  
**[12]** "Cómo hackearon a Hacking Team | Ars Technica". 19 abr. 2016, https://arstechnica.com/information-technology/2016/04/how-hacking-team-got-hacked-phineas-phisher/.  
[13] "PsExec - Windows Sysinternals | Microsoft Docs". 28 jun. 2016, https://docs.microsoft.com/en-us/sysinternals/downloads/psexec  
[14] "Nmap: the Network Mapper - Free Security ...." https://nmap.org/  
[15] "Nmap Network Scanning-The Official Nmap Project Guide to ...." https://nmap.org/book/.  
[16] "Metasploit | Penetration Testing Software, Pen Testing ...." https://www.metasploit.com/.  
[17] "Jeff Dimmock (@bluscreenofjeff) | Twitter" https://twitter.com/bluscreenofjeff.  
**[18]** "Cobalt Strike." https://www.cobaltstrike.com/..  
**[19]** "PowerShell Empire | Building an Empire with PowerShell." https://www.powershellempire.com/.  
[20]** "Dominio Frontal - Empresa | MITRE ATT&CK™". 16 ene. 2018, https://attack.mitre.org/techniques/T1172/.  
[21] "Gestión de riesgos - Dirección de Publicaciones del Ejército - Army.mil." 14 abr. 2014, https://armypubs.army.mil/epubs/DR_pubs/DR_a/pdf/web/atp5_19.pdf.  
[22] "NIST Special Publication 800-30 Revision 1, Guide for ...." https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-30r1.pdf.  
[23] "Chris Crowley (@CCrowMontance) | autor de SANS MGT535, MGT517, y SOC-Class" https://twitter.com/ccrowmontance?lang=en.  
[24] "Enterprise Detection & Response: The ...." [http://detect-respond.blogspot.com/2013/03/the-pyramid-of-pain.html.](http://detect-respond.blogspot.com/2013/03/the-pyramid-of-pain.html.)  
25] "Threat Mitigation Strategies - Threatexpress" [https://threatexpress.com/blogs/2018/threat-mitigation-strategies-observations-recommendations/.]  
[26] "Estrategias de mitigación de amenazas Parte 2 - Threatexpress". 15 May. 2018, https://threatexpress.com/blogs/2018/threat-mitigation-strategies-technical-recommendations-and-info-part-2/.  
[27] "Wald, Abraham. (1943). A Method of Estimating Plane Vulnerability Based on Damage of Survivors. Statistical Research Group,Columbia University. CRC 432" - reimpresión de julio de 1980, [http://www.dtic.mil/get-tr-doc/pdf?](http://www.dtic.mil/get-tr-doc/pdf?) AD=ADA091073&Location=U2&doc=GetTRDoc.pdf.

