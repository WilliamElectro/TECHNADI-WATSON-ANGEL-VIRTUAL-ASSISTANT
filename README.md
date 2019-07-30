# TECHNADI: WATSON ANGEL-VIRTUAL ASSISTANT

<img src="https://raw.githubusercontent.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/proyecto.png"/>
https://www.facebook.com/watsonAngelAssistant/

# DESCRIPCIÓN 
Durante las catástrofes naturales el número de personas heridas superan por mucho al de personas capacitadas en primeros auxilios y soporte vital básico. Muchas de las muertes son por causa de la inasistencia, la falta de alguien capacitado que pueda brindar la atención necesaria en el menor tiempo posible. Las hemorragias, amputaciones y otras lesiones requieren una acción inmediata, muchas por la gravedad no pueden esperar la llegada de brigadas o incluso el traslado a un hospital.   Watson Angel es un asistente virtual en entrenamiento que implementa la tecnología de Watson Assistant junto node RED y otras más, proporcionando conexión a servicios más tangibles y accesibles como por ejemplo un chat de Messenger, Telegram o WhatsApp. Logrando que todo aquel con acceso a internet pueda ayudar en poco tiempo a quien lo necesite. Cuente o no con un botiquín. En caso de falta de internet se tienen en cuenta dos soluciones futuras: la primera es la implementación de datos móviles que pueden ser brindados por el gobierno tras la catástrofe y la segunda es una vinculación entre nuestra propuesta y la propuesta ganadora del año pasado, Proyect Owl. Aunque son prioridad no solo las personas heridas se verían beneficiadas con la implementación de Watson Angel, las instituciones de salud gozarían de una menor congestión y podrían concentrarse en los casos de mayor gravedad.  Watson Angel es superior a aplicaciones de primeros auxilios. Primero, por ser un asistente virtual que guía paso a paso al usuario. Segundo, identifica el estado del lesionado lo cual podría ser conectado a una base de datos. Tercero, no se encuentra ligado a la descarga de una aplicación extra en el celular o computadora que por motivos de espacio podría ser eliminada por el usuario. Cuarto, no requiere de una búsqueda o lectura extensa para obtener el procedimiento a seguir. Quinto, cuenta con el modo respuesta tanto en versión de texto como de audio. En este momento Watson Angel cuenta con asistencia para hemorragias, hematomas, aplastamientos, amputaciones simples, amputaciones compuestas y convulsiones, de igual manera puede instruir para tomar el pulso, realizar RCP y brindar los números de entidades de emergencia como la policía, bomberos y ambulancias.

# CODIGOS DEL SKILL Y EL FLUJO NODE-RED

SKILL: https://github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/blob/master/skill-P_Aux.json
NODE-RED: https://github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/blob/master/flows.json

# VIDEO 
[![ScreenShot](https://raw.github.com/GabLeRoux/WebMole/master/ressources/WebMole_Youtube_Video.png)](https://www.youtube.com/watch?v=6NnPdMgFqPc)

https://www.youtube.com/watch?v=6NnPdMgFqPc

# SERVICIOS
* Watson Assistant
* Text to Speech
* Speech to Text
* Node-RED

# I. INTRODUCCIÓN
Descripción de la problemática: 
Tras cualquier catástrofe natural (terremoto, tsunami, incendio forestal, derrumbe, etc.) la cantidad de personas lesionadas supera de forma significativa el número de personas que tienen conocimiento y/o son capacitadas en el servicio de primeros auxilios, ante lo cual surge la necesidad de crear una herramienta que permita a aquellos que no tienen los conocimientos, pero sí la posibilidad física de ayudar, brindar las atenciones médicas básicas, con lo cual sería posible salvar más vidas en estas circunstancias. 
Antecedentes: 
Actualmente ante un acontecimiento de desastre natural es común que brigadas de socorro desde distintas partes del mundo lleguen a asistir la emergencia, sin embargo, su llegada es demorada; lo más pronto serían los servicios de socorro locales. Instituciones como la Cruz Roja han desarrollado aplicaciones para ayudar a personas a enfrentar emergencias cotidianas, pero al ser de carácter informativo requiere una interacción constante del usuario y una manipulación continua del equipo móvil.
Contexto y enfoque de la solución: La idea de Watson Angel, trata de poder brindar un asistente virtual completo para que sea implementada mediante cualquier dispositivo con acceso a la red, implementando el speed to text y viceversa para que el usuario mantenga una constante conversación, sin la necesidad de ocupar sus manos en otra cosa diferente a prestar el servicio de primero auxilios o soporte vital básico.

# II. METODOLOGÍA 
Watson Angel hace uso de la plataforma de IBM Cloud para su entrenamiento y encadenamiento con el mundo real. Se realizó un análisis de los puntos críticos que se generan tras un desastre natural, enfocándonos en la salubridad y asistencia de personas tras los incidentes. Durante el desarrollo del proyecto se implementó un blockchain explicado en la siguiente imagen. 

<img src="https://raw.github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/7.png"/>
   
Donde la capa superior y la única a la que tiene acceso el usuario “Messenger”, las conexiones se realizan entre Chatfuel y Node-Red hasta la capa más profunda la cual contiene a Watson Assistant y conversores de texto a voz y viceversa.

# III. PROBLEMAS DURANTE EL DESARROLLO DE PROTOTIPO 
Idealmente se pensó la implementación de una conversación mediante un canal de voz y audio continuo y abierto, pero el prototipo requiere la interacción constante con el usuario ya sea por textos o mensajes de voz, adicionalmente en la conexión entre Facebook Messenger y Node-Red, en un principio conectando directamente con Facebook Developers no funcionó con usuarios distintos al administrador por lo que se optó por alguna otra alternativa en nuestro caso Chatfuel. 

# IV. RESULTADOS 
Se obtuvo un muy buen primer prototipo, que reconoce e identifica lesiones comunes durante desastres naturales, tiene un pequeño catálogo de soluciones y métodos de respuesta que pueden ayudar aún sin un botiquín, a futuro este catálogo puede ser ampliado e implementado para cualquier otra situación que lo requiera incluyendo servicio con botiquín personalizado o heridas mucho más simples o complejas.

# V. CONCLUSIONES 
La combinación de herramientas existentes y de gran uso como Messenger permite abarcar un mayor publico que gracias a la integración en Node-Red de los servicios de IBM Cloud pueden realizar una conversación fluida con el objetivo de aumentar las manos que ayudan en algún tipo de eventualidad como son los desastres naturales.

# REFERENCIAS
1.	https://cloud.ibm.com/docs/services/assistant?topic=assistant-getting-started#getting-started-tutorial
2.	https://www.efe.com/efe/espana/sociedad/la-onu-destaca-baja-mortalidad-por-desastres-en-2018-pero-alerta-sobre-el-nino/10004-3876923
3.	https://www.efeverde.com/noticias/desastres-naturales-muertos-onu/
4.	https://cadenaser.com/emisora/2016/10/16/radio_valladolid/1476616274_571625.html
5.	https://www.efesalud.com/primer-minuto-salva-vidas-importancia-primeros-auxilios/
6.	http://www.cruzrojacolombiana.org/noticias-y-prensa/aplicaci%C3%B3n-m%C3%B3vil-de-primeros-auxilios-la-nueva-apuesta-de-la-cruz-roja-colombiana
7.	https://cloud.ibm.com/docs/tutorials?topic=solution-tutorials-android-watson-chatbot
8.	https://cloud.ibm.com/apidocs/assistant
9.	https://cloud.ibm.com/apidocs/speech-to-text
10.	https://cloud.ibm.com/apidocs/text-to-speech
11.	https://nodered.org/
12.	https://dashboard.chatfuel.com/#/bots


# CÓMO SE HIZO
Se crea un flujo que permita integrar servicios provenientes de diversas fuentes, este blockchain conecta nuestro flujo de Node-RED que integra los sirvicios de Watson Assistant, TTS y STT con el ChatBot en Facebook Messenger a través de ChatFuel.

<img src="https://raw.github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/flujo.PNG"/>

El flujo recibe un enlace de messenger, se convierte a WAV, se envía a STT para su transcripción y se envía a Watson Assistant. Con la respuesta de Watson Assistant, use TTS para convertirlo a audio, convertir a MP3, almacenar en una sesión variable global y enviar un enlace a Facebook Messenger. Este flujo utiliza el nodo ffmpeg para convertir audio. Este flujo recibe el nombre y el apellido de Facebook y se envía al contexto dentro de WA.

Luego, se deben crear y sincronizar los servicios de IBM CLOUD (Watson Assistant, TTS y SST)(Link del skill utilizado: https://github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/blob/master/skill-P_Aux.json) con el flujo creado (Link para cargar el flujo en NODE-RED: https://github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/blob/master/flows.json), esto se hace a través de las credenciales de cada API 

<img src="https://raw.github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/Credenciales.PNG"/>

Una vez tengamos nuestro Flujo conectado a los servcios de IBM CLOUD, hacemos la debida conexion a ChatFuel  quien conectará nuestro Chatbot en Facebook Messenger con nuestra integración de servicios, pero para ello, debemos haber creado(y personalizado) una página en Facebook

<img src="https://raw.github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/Facebook.PNG"/>

Esta página en Facebook, será sincronizada con ChatFuel la que a su vez llamará los flujos

<img src="https://raw.github.com/WilliamElectro/TECHNADI-WATSON-ANGEL-VIRTUAL-ASSISTANT/master/Chatfuel.PNG"/>











