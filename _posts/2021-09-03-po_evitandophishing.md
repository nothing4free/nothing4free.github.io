---
layout: post
title: "Protección online: evitando el phishing."
permalink: "/legacy/2021-09-03_po-evitandophishing"
---

# Protección online: evitando el phishing.

Los ataques de suplantación de identidad suponen un gran riesgo para nuestra seguridad online. Si bien suelen ser relativamente simples, sus consecuencias pueden ser catastróficas, tanto para nosotros como para los administradores de los sistemas e infraestructuras que se vean afectados. De hecho, recientemente viví una situación en la que un grupo de personas del cual formo parte sufrió un ataque de este tipo: esta situación es la razón por la cual redacto este artículo. En este post, encontraréis formas de identificar este tipo de estafas para evitarlas, así como los pasos a seguir si habéis sido víctimas de un ataque de este tipo.

### _Phishing:_ ¿Qué es exactamente?

Si recurrimos a Wikipedia, la definición de _phishing_ es la siguiente:

> Phishing: conjunto de técnicas que persiguen el engaño a una víctima ganándose su confianza haciéndose pasar por una persona, empresa o servicio de confianza para manipularla y hacer que realice acciones que no debería realizar, como revelar información confidencial o hacer click en un enlace.

Es decir, mediante el phishing un atacante busca robar nuestra identidad para poder utilizarla con fines varios (extorsión, venta en el mercado negro…). Los ataques de este tipo son muy variados: en el caso que viví, el ataque consistía en un correo electrónico que simulaba enviar un archivo adjunto alojado en la nube. Cuando se hacía click sobre el enlace para acceder a dicho archivo, se mostraba una página de inicio de sesión falsa montada por los atacantes, con la finalidad de conseguir las credenciales de acceso de aquellos interesados en ver el archivo. 

Esta es una de las formas más comunes de phishing que existen, ya que clonar páginas web es relativamente fácil para los atacantes, pero también se pueden dar ataques más complejos que hacen uso de llamadas telefónicas con suplantación de identidad, mensajes de texto… En este post, me centraré en dos de las herramientas más utilizadas por los ciberdelincuentes que realizan phishing: los enlaces que podemos encontrar en mensajes estafa y los correos electrónicos o SMS falsos.

### Identificando enlaces y sitios web sospechosos.

Si sospechamos de una página web, su enlace es un elemento que hay que tener muy en cuenta. Las páginas web falsas suelen estar mal hechas, con multitud de errores de formato e imágenes de baja calidad, enlaces que no funcionan, traducciones erróneas, mal funcionamiento… Lo importante que debemos saber es que, aunque estemos ante un clon exacto de la web original, los atacantes no lo pueden publicar en en una web con el mismo enlace que la web legítima. Por ejemplo, si un atacante clona apple.com, no puede publicar su clon en apple.com, sino que tiene que buscar otro nombre. Por ello, publican su página falsa usando dominios (enlaces) muy parecidos a la web original, cambiando algún caracter o realizando modificaciones al nombre original. Para determinar si una web es falsa o no, pues, debemos examinar su enlace.

Supongamos el enlace de este blog:

![](assets/../../assets/legacy_post4_1.png)


Las partes que hay que examinar son el protocolo y el dominio:

- Protocolo: Indica si el servidor es no encriptado (http) o encriptado (https). Las estafas suelen estar montadas en páginas web http, pero es muy posible encontrarse con una estafa en un sitio https. Si una web sospechosa es http, podemos afirmar casi con certeza absoluta que es una estafa, pero antes debemos examinar el dominio.

- Dominio: esta es la parte del enlace que nos permitirá saber si una web es falsa o no. Si no cambia respecto a la página web oficial, entonces estamos ante una web legítima; de cambiar lo más mínimo, estamos ante una estafa. 

Algunos trucos que utilizan los atacantes para encubrir dominios falson son los siguientes:

- Añadir letras al nombre: faceboook.com en vez de facebook.com.
- Añadir elementos al dominio: twitter-support.com en vez de twitter.com.
- Separar palabras: pay–pal.com en vez de paypal.com.
- Usar caracteres similares: gmaii.com en vez de gmail.com. Esta técnica es usada en numerosas ocasiones.
- Mantener el nombre pero cambiar la extensión: apple.org en vez de apple.com o apple.es.

En algunos enlaces se incluye una parte adicional que se sitúa entre el protocolo y el dominio: el subdominio. Se suele utilizar en páginas de soporte técnico como la siguiente:

![](assets/../../assets/legacy_post4_2.png)

Si nos encontramos con un enlace que contiene un subdominio, simplemente nos tenemos que fijar en su dominio: como he mencionado anteriormente, si el dominio sospechoso cambia lo más mínimo respecto al dominio oficial, entonces estamos ante una estafa. En nuestro ejemplo, el dominio superior es legítimo, pero una estafa del mismo podría ser la siguiente:

![](assets/../../assets/legacy_post4_3.png)

Podemos observar que, en vez de apple.com, el dominio ahora es app1e.com: a pesar de que el subdominio coincide, es una estafa, pues lo que debe coincidir al 100% es el dominio.

Es también común ver estafas por SMS o correo electrónico con enlaces acortados (como aquellos de bit.ly o servicios similares). Para saber a dónde llevan sin tener que meternos en el enlace, recomiendo encarecidamente utilizar páginas web como wheregoes.com, que se encargarán de rastrear el enlace acortado para ver dónde lleva en realidad.

### Identificando correos electrónicos y SMS sospechosos.

Una gran cantidad de estafas de phishing se reciben mediante correo electrónico y SMS. A día de hoy, la gran mayoría de servicios de correo electrónico hacen una gran labor a la hora de filtrar este tipo de mensajes, pero no son perfectos. Si sospechamos de un correo u SMS que hemos recibido, es esencial fijarnos en varios aspectos del mismo.

![](assets/../../assets/legacy_post4_4.png)

La dirección de correo electrónico es lo primero que debemo examinar, y posiblemente lo más importante. Si comprobamos su dominio y cambia lo más mínimo respecto a la web legítima, entonces estamos ante una estafa. En la imagen superior, vemos una dirección real que nos envía notificaciones de YouTube (nuevos subscriptores, comentarios, etc.): su dominio coincide con el de YouTube, por lo que es una dirección legítima. Aún así, un atacante puede llegar a suplantar una dirección de correo real, pero la mayoría de clientes de correo lo detectan como correo inseguro; no obstante, conviene examinar más aspectos del mismo, como su contenido y finalidad.

En el caso de los SMS, si sospechamos de un número de teléfono, lo mejor que se puede hacer es una búsqueda en Google del mismo, para ver si obtenemos algún resultado relevante sobre posibles estafas. No obstante, es difícil determinar si un mensaje SMS es una estafa o no a partir del número; si sospechamos, conviene examinar su contenido. 

En las estafas, el contenido de los correos y SMS suele caracterizarse por tener imágenes de baja calidad, gráficos que no cargan, errores de formato, ortográficos y sintácticos… Si el correo se ve «roto», entonces es probablemente una estafa.

La finalidad de los correos y/o SMS también es un aspecto a examinar: las estafas suelen tener asuntos llamativos, con alertas desorbitadas u ofertas demasiado buenas para ser verdad. También hay estafadores que suelen contactar sobre servicios que ni siquiera tenemos contratados o pagos que no hemos realizado. Es importante recordar que ningún banco o empresa nos solicitará enviar datos confidenciales por correo electrónico, llamada telefónica o SMS. En caso de que dudemos de un correo o SMS, lo mejor es contactar por otra vía a la entidad responsable para verificar su legitimidad.

Otro punto clave a la hora de no caer en phishing son los archivos adjuntos. Si el archivo adjunto es un .exe, entonces estamos ante un claro indicador de que se trata de una estafa: bajo ningún concepto debemos abrir dicho archivo. Incluso un simple PDF puede infectar nuestro ordenador, así que lo mejor que podemos hacer si un correo sospechoso tiene archivos es no abrirlos.

Por último, pero no menos importante, es esencial fijarse en el estilo de redacción del correo o SMS. Ya lo he mencionado anteriormente: el phishing es internacional, lo que implica que la mayoría de atacantes utilizan servicios de traducción que cometen errores que son fácilmente identificables, como frases sin sentido o sintaxis extraña. Además, en ocasiones caracteres únicos del español como la ñ o las tildes no aparecen representados correctamente; esto se debe a las diferentes distribuciones digitales de caracteres, utilizadas globalmente. 

¿Es posible que un hacker suplante completamente la identidad de una entidad real? Sí, pero en estos casos la mayoría de servicios de correo electrónico marcan el mensaje como inseguro; no obstante, si se trata de una estafa, suele haber indicios claros de ello en el correo electrónico o en los enlaces del mismo.

### He sido víctima: ¿Qué hago ahora?

Dependiendo del ataque y de la información que los delincuentes hayan conseguido, la respuesta a este tipo de incidentes varía.

Si diste tu usuario y contraseña en un login falso, entonces debes cambiar la contraseña de la cuenta comprometida. Si utilizabas la misma contraseña en otros sitios, la debes cambiar también. Una buena práctica para reducir el impacto de un ataque como este es no reutilizar contraseñas y utilizar un [gestor de contraseñas](https://nothing4free.org/legacy/2021-04-21_po-gestoresdecontrasenas). Si la cuenta comprometida forma parte de una empresa o entidad educativa, es esencial trasladar este problema a los encargados relevantes, para que realizen un chequeo de su infraestructura y puedan minimizar el daño en caso de ataque.

En caso de haber introducido otro tipo de información, como la relativa a cuentas bancarias o similares, es preciso contactar con la entidad relevante, comentándoles el problema y restableciendo claves de acceso y contraseñas.

### Conclusión y guía rápida

En resumen, los aspectos en los que nos tenemos que fijar si sospechamos que estamos siendo estafados son:

- Enlace: comprobar el dominio (examinarlo detenidamente: si cambia, es estafa).
- Enlace: comprobar el protocolo (si es http, muy probablemente es estafa, aunque también hay estafas https).
- Correo electrónico: comprobar el dominio de la dirección (examinarlo detenidamente: si cambia, es estafa).
- Correo electrónico: comprobar el contenido (si está «roto», hay faltas de ortografía, frases sin sentido o caracteres extraños, es estafa).
- Correo electrónico: comprobar la finalidad (las ofertas demasiado buenas para ser verdad probablemente lo son, ojo a los correos con asuntos desorbitados o sobre servicios que no tenemos contratados).
- Correo electrónico: mucho cuidado con los archivos adjuntos (no abrirlos si dudamos del remitente o del correo, y mucho menos si son .exe)

Si recibimos un correo o SMS de una empresa y sospechamos de su legitimidad, conviene contactar con dicha empresa por otras vías para comprobar si estamos ante una estafa o no. Una vez más, conviene recordar que ningún banco o empresa nos solicitará enviar datos confidenciales como contraseñas o códigos privados por correo electrónico, llamada telefónica o SMS.

Si hemos sido víctimas de un ataque de este tipo, debemos restablecer la contraseña o los datos confidenciales que se pedían en la estafa, contactando con las entidades relevantes en los casos que así lo precisen.

¡Espero que esta pequeña guía sirva de ayuda! Estos son los pasos que suelo seguir a la hora de examinar posibles estafas, pero si tenéis más consejos no dudéis en dejarlos en los comentarios o enviádmelos en la sección de contacto.

¡Muchas gracias por el apoyo! Esto es todo por hoy :)