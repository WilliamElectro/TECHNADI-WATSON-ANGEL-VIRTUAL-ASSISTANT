# TECHNADI: WATSON ANGEL-VIRTUAL ASSISTANT
<img src="https://raw.githubusercontent.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/proyecto.png"/>
https://www.facebook.com/watsonAngelAssistant/

# I. INTRODUCCIÓN
Descripción de la problemática: 
Tras cualquier catástrofe natural (terremoto, tsunami, incendio forestal, derrumbe, etc.) la cantidad de personas lesionadas supera de forma significativa el número de personas que tienen conocimiento y/o son capacitadas en el servicio de primeros auxilios, ante lo cual surge la necesidad de crear una herramienta que permita a aquellos que no tienen los conocimientos, pero sí la posibilidad física de ayudar, brindar las atenciones médicas básicas, con lo cual sería posible salvar más vidas en estas circunstancias. 
Antecedentes: 
Actualmente ante un acontecimiento de desastre natural es común que brigadas de socorro desde distintas partes del mundo lleguen a asistir la emergencia, sin embargo, su llegada es demorada; lo más pronto serían los servicios de socorro locales. Instituciones como la Cruz Roja han desarrollado aplicaciones para ayudar a personas a enfrentar emergencias cotidianas, pero al ser de carácter informativo requiere una interacción constante del usuario y una manipulación continua del equipo móvil.
Contexto y enfoque de la solución: La idea de Watson Angel, trata de poder brindar un asistente virtual completo para que sea implementada mediante cualquier dispositivo con acceso a la red, implementando el speed to text y viceversa para que el usuario mantenga una constante conversación, sin la necesidad de ocupar sus manos en otra cosa diferente a prestar el servicio de primero auxilios o soporte vital básico.

# II. METODOLOGÍA 
Watson Angel hace uso de la plataforma de IBM Cloud para su entrenamiento y encadenamiento con el mundo real. Se realizó un análisis de los puntos críticos que se generan tras un desastre natural, enfocándonos en la salubridad y asistencia de personas tras los incidentes. Durante el desarrollo del proyecto se implementó un blockchain explicado en la siguiente imagen. 

<img src="https://github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/7.png"/>
   
Donde la capa superior y la única a la que tiene acceso el usuario “Messenger”, las conexiones se realizan entre Chatfuel y Node-Red hasta la capa más profunda la cual contiene a Watson Assistant y conversores de texto a voz y viceversa.

# III. PROBLEMAS DURANTE EL DESARROLLO DE PROTOTIPO 
Idealmente se pensó la implementación de una conversación mediante un canal de voz y audio continuo y abierto, pero el prototipo requiere la interacción constante con el usuario ya sea por textos o mensajes de voz, adicionalmente en la conexión entre Facebook Messenger y Node-Red, en un principio conectando directamente con Facebook Developers no funcionó con usuarios distintos al administrador por lo que se optó por alguna otra alternativa en nuestro caso Chatfuel. 

# IV. RESULTADOS 
Se obtuvo un muy buen primer prototipo, que reconoce e identifica lesiones comunes durante desastres naturales, tiene un pequeño catálogo de soluciones y métodos de respuesta que pueden ayudar aún sin un botiquín, a futuro este catálogo puede ser ampliado e implementado para cualquier otra situación que lo requiera incluyendo servicio con botiquín personalizado o heridas mucho más simples o complejas.

# V. CONCLUSIONES 
La combinación de herramientas existentes y de gran uso como Messenger permite abarcar un mayor publico que gracias a la integración en Node-Red de los servicios de IBM Cloud pueden realizar una conversación fluida con el objetivo de aumentar las manos que ayudan en algún tipo de eventualidad como son los desastres naturales.
