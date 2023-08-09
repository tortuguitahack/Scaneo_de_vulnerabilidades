Las **vulnerabilidades en el software** son una de las principales puertas de entrada para los cibercriminales, pero también es un vector de ataque una mala configuración de nuestros servicios, e incluso la exposición de puerto TCP/UDP a Internet sin ningún tipo de filtrado. Los piratas informáticos están buscando constantemente nuevas formas de atacar cualquier ordenador, servidor o red a través de estos fallos de seguridad, por este motivo, los propios ingenieros de las compañías, los investigadores de seguridad y los hackers éticos están constantemente analizando los diferentes programas en busca de fallos de seguridad y reportarlo para que se solucione. La herramienta imprescindible para esta tarea con los escáneres de vulnerabilidades.

## Qué es un escáner de vulnerabilidades

Un **escáner de vulnerabilidades** es un software diseñado para realizar análisis automáticos de cualquier aplicación, sistema o red en busca de cualquier posible vulnerabilidad que exista. Aunque estas aplicaciones no son capaces de detectar la vulnerabilidad con total precisión, sí son capaces de detectar ciertos elementos que podrían desencadenar en una vulnerabilidad, facilitando enormemente el trabajo a los investigadores e ingenieros. Hay **varios tipos de escáneres de vulnerabilidades**, autenticados, en los que se realizan pruebas y ataques potenciales desde la propia red, y no autenticados, en los que el investigador o hacker ético se intenta hacer pasar por un pirata informático simulando un ataque desde fuera para ver hasta dónde es capaz de llegar analizando (y explotando) posibles vulnerabilidades.

En la red podemos encontrar una gran cantidad de escáneres de vulnerabilidades, la mayoría muy similares, pero con algunos aspectos que claramente les diferencian y les hacen mejores, o simplemente diferentes, que otros. Hoy en RedesZone vamos a ver cuáles son los más importantes y conocidos para realizar un primer pentesting.

### Qué características debe cumplir

Estas herramientas, son ampliamente utilizadas por empresas y organizaciones. Esto es algo que utilizan para poder detectar posibles brechas de seguridad en los sistemas y redes. Pero para que estos sean efectivos, hay algunas características que deben poder cumplir. Estas son:

- **Cobertura exhaustiva:** Los escáneres de vulnerabilidades deben ser capaces de detectar una gran variedad de vulnerabilidades. Esto incluye los problemas de configuración, vulnerabilidades de software, de red y de aplicaciones. Por otro lado, debe poder reconocer las vulnerabilidades conocidas, como las no conocidas o nuevas.
- **Precisión:** El analizador debe disponer de una alta precisión a la hora de identificar las vulnerabilidades. Esto quiere decir, que debe minimizar al máximo los falsos positivos, y falsos negativos.
- **Escaneos programados y automáticos:** Una de las funciones más solicitadas, es la capacidad para realizar escaneos programados o de forma automática. Esto nos ayuda a mantener una visión al completo y de forma continua de la seguridad de los sistemas y redes. Así, se pueden detectar los problemas y ponerles solución antes de que sean explotados.
- **Análisis de informes y resultados:** La herramienta debe tener la capacidad de crear informes detallados, los cuales muestran los resultados de los escaneos. Incluyen información sobre las vulnerabilidades identificadas, así como de sugerencias que nos permita ponerles solución.
- **Facilidad de uso:** Un buen sistema de escaneo de vulnerabilidades, debe ser sencillo de utilizar y comprender. De forma que los resultados con son claros. Los administradores, no se deben encontrar con dificultades a la hora de entender los informes o resultados. Así se pueden aplicar soluciones más efectivas. 
- **Integración:** Esta herramienta debe ser capaz de realizar una integración con las demás herramientas de seguridad. Sea el firewall o el antivirus. Esto ayudará a detectar intrusiones, y proporcionar una visión más completa de la seguridad de toda la red.

## Nmap

No podemos empezar un recopilatorio con los mejores escáneres de vulnerabilidades sin hablar de uno de los más potentes, completos y veteranos que podemos encontrar en la red: [**Nmap**](https://nmap.org/). Este software es uno de los más usados para buscar hosts dentro de una red local, pero también permite el descubrimiendo de hosts en Internet para comprobar si están conectados a la red, además, podremos realizar amplios y avanzados escaneos de puertos para comprobar si tenemos algún servicio funcionando que no esté protegido por el firewall, e incluso podremos ver si tenemos un firewall en un determinado host. Otras opciones que podremos realizar con este programa es saber qué sistema operativo utiliza un host en concreto, si escaneamos un ordenador con Windows nos indicará que estamos, efectivamente, escaneando un sistema operativo Windows, y lo mismo con Linux o Unix.

Este programa es de código abierto y multiplataforma, aunque lo más normal es utilizarlo en sistemas operativos Linux para realizar la tarea de pentesting, es el primer paso para realizar una intrusión en los sistemas e intentar hackear el equipo correctamente, siempre con fines éticos para descubrir posibles vulnerabilidades. Este software tiene una gran cantidad de opciones avanzadas, y, además, dispone de una interfaz gráfica de manera opcional llamada Zenmap que podremos utilizar de manera rápida y fácil.

![](https://www.redeszone.net/app/uploads-redeszone.net/2015/02/NSEarch_Nmap_foto_3.png)

Aunque esta herramienta nació como un escáner de puertos, gracias a los **scripts NSE** que incluye por defecto (y que podemos bajar de multitud de páginas web) es posible utilizarla como una completa herramienta para buscar vulnerabilidades en redes y sistemas. Los scripts NSE utilizan la potencia del propio Nmap, pero, además, es capaz de explotar vulnerabilidades conocidas a determinados programas, por lo que es muy útil actualizarla frecuentemente con los últimos scripts. Tanto NSE como Nmap hacen un equipo realmente potente para ayudar al hacker a realizar el pentesting. Algunas de las funciones que podremos realizar son atacar los servidores Samba probando cientos de usuarios y contraseñas, lo mismo con los servidores de FTP e incluso servidores SSH, y es que podremos atacar una gran cantidad de servicios para explotar vulnerabilidades. Cuando sale una vulnerabilidad pública, los desarrolladores incorporan este exploit en Nmap NSE para explotarla de forma fácil y rápida, con el objetivo de ayudar a los pentesters la tarea de explotación del sistema comprometido.

En el siguiente **manual de Nmap** os explicamos cómo descargarlo y cómo utilizarlo para buscar posibles vulnerabilidades en una red o un software.

### Motivos para utilizar Nmap

- Cuenta con capacidad para reconocer de forma rápida todos los dispositivos, incluso servidores, routers, móviles, entre otros. Y lo puede hacer tanto en redes únicas como múltiples. Por lo cual es muy buena opción para el sector empresarial donde se utilizan diferentes redes.
- Nos ayuda a realizar una identificación de los servicios que se ejecutan en el sistema. Los servidores web, DNS y otras aplicaciones serán escaneadas también. Esto hace que se puedan detectar diferentes versiones de las aplicaciones con mucha precisión. Esto ayuda a detectar vulnerabilidades existentes.
- Puede localizar información sobre los sistemas operativos que ejecutan los dispositivos. A su vez proporciona información muy detallada como las versiones de los mismos, lo cual nos ayuda mucho a realizar una planificación de diferentes enfoques durante la penetración de los paquetes.
- En las auditorías de seguridad y el escaneo de vulnerabilidades, Nmap puede atacar sistemas mediante la utilización de scripts existentes en el motor scripting de Nmap.
- Cuenta ccon una interfaz gráfica llamada Zenmap, que nos ayuda a llevar a cabo mapeos visuales de las redes. Esto es bueno para darle una usabilidad mayor a la herramienta y facilita que los informes se generen de una forma más detallada, intuitiva y accesible.

## Suite Aircrack-ng

Las redes Wi-Fi son uno de los puntos más débiles de las empresas, y por ello es uno de los aspectos que más debemos cuidar. En este punto, [**Aircrack-ng**](https://www.aircrack-ng.org/) es sin duda la mejor herramienta para poner a prueba la seguridad de cualquier red Wi-Fi en busca de cualquier posible vulnerabilidad que pueda permitir a cualquier usuario no autorizado hacerse con la contraseña de nuestra red. Este programa es uno de los más utilizados en todo el mundo para crackear redes WiFi, ya sea con cifrado WEP, WPA e incluso WPA2, no obstante, normalmente se utiliza junto con otros programas para acelerar la tarea de crackeo de las diferentes contraseñas.

Aircrack-ng realmente no es una única herramienta, sino que está formado por varias herramientas que se dedican específicamente a diferentes tareas, cuando instalamos Aircrack-ng se instalarán todas las herramientas adicionales que están específicamente diseñadas a ciertas tareas. A continuación, podéis ver en detalle todas las herramientas:

- Airmon-ng: se encarga de poner las tarjetas de red Wi-Fi en modo monitor, para permitir la captura de toda la información por parte de Airodump-ng.
- Airodump-ng: es capaz de realizar captura de datos y exportar toda la información, para posteriormente tratara con herramientas de terceros e incluso con otras herramientas de la suite Aircrack-ng.
- Aireplay-ng: esta herramienta se utiliza para realizar ataques replay, desautenticación de clientes, crear APs falsos y otro tipo de inyección de paquetes. Un detalle importante es que la tarjeta Wi-Fi que utilicemos, debe ser compatible con inyección de paquetes, ya que muchas no lo son.
- Aircrack-ng: este programa es el que se encarga de crackear las claves WEP, WPA y WPA2 de las redes Wi-Fi, obteniendo toda la información conseguida por el resto de programas de la suite.

Si tienes que realizar pentesting a las redes inalámbricas Wi-Fi, esta suite es una de las fundamentales para ti. Si estás interesado en el pentesting de redes inalámbricas, podéis ver esta master class.

Tal y como podéis ver, dura más de 3 horas y se explica una gran cantidad de ataques que se pueden realizar, e incluso cómo crear nuestras propias herramientas.

## Hashcat

[**Hashcat**](https://hashcat.net/hashcat/) es un programa que nos sirve para crackear todo tipo de hashes de contraseñas, es el mejor programa para realizar ataques de diccionario o fuerza bruta contra el hash de una clave para intentar crackearla. Hashcat utiliza la potencia de la CPU y GPU para acelerar lo máximo posible el proceso de obtención de la clave. Aunque no es un programa que escanea vulnerabilidades, será muy utilizado por ti en caso de obtener los diferentes hashes de contraseñas, por lo que consideramos que debe estar en este listado de programas fundamentales.

Este programa es la navaja suiza de los crackeadores de contraseñas, normalmente las contraseñas no se almacenan en texto plano sino que se almacena el hash de la contraseña en el sistema. Hashcat lo que hace es atacar este hash de la contraseña, intentando crackearla por diferentes métodos, ya sea por diccionario o por fuerza bruta. Una característica muy importante de Hashcat es que soporta todos los hash que tenemos actualmente, y que usan los principales servidores y servicios que almacenan contraseñas.

## Wireshark

Continuando con las auditorías de redes, [**Wireshark**](https://www.wireshark.org/) es el analizador de paquetes y protocolos por excelencia. Esta aplicación es capaz de registrar absolutamente todos los paquetes que pasan por una red, recogerlos y poder filtrarlos y ordenarlos de multitud e formas para poder analizar cómodamente todo el tráfico. Esta herramienta además es capaz de descifrar los paquetes enviados a través de los principales protocolos de conexión segura para poder analizar sin problema su contenido.

![Wireshark 2.0](https://www.redeszone.net/app/uploads-redeszone.net/2015/11/Wireshark-2.0.png)

Sin duda, la mejor aplicación que podemos encontrar para analizar cualquier red y poder detectar cualquier posible fuga de tráfico o conexiones que intenten explotar un fallo de seguridad. Es compatible con sistemas operativos Windows y Linux, además, soporta una gran cantidad de extensiones que utilizan otros programas a la hora de capturar el tráfico, de esta forma, podremos analizar todo el tráfico más tarde.

## OpenVAS

Entrando ya en la búsqueda de vulnerabilidades en aplicaciones y equipos, una de las aplicaciones más completas que podemos encontrar en la red es **[OpenVAS](https://www.openvas.org/).** OpenVAS es un escáner de vulnerabilidades al que podemos introducir una dirección IP y encargarle el análisis de dicho equipo, recogiendo información sobre los servicios en funcionamiento, los puertos abiertos, fallos de configuración, posibles vulnerabilidades conocidas en el software del equipo o servidor, etc.

Este programa se puede ejecutar tanto desde dentro de una red como desde un servidor externo, simulando así un ataque real. Cuando finaliza nos genera un completo informe con todas las posibles debilidades que pueden suponer un peligro para nuestra seguridad. Además, podemos configurarlo en modo monitorización continua, estableciendo alertas que saltarán cuando se detecte el más mínimo fallo.

![openvas](https://www.redeszone.net/app/uploads-redeszone.net/2019/05/openvas.png)

OpenVAS es una herramienta completamente gratuita que nos permitirá realizar una gran cantidad de pruebas de vulnerabilidad contra servidores web, además, tiene una gran comunidad detrás de ella para darle soporte e incorporar nuevas funcionalidades para exprimir al máximo todo su potencial.

## OWASP Zen Attack Proxy ZAP

El proyecto OWASP (Open Web Application Security Project) es un proyecto abierto y sin ánimo de lucro pensado para mejorar la seguridad de las redes, los servidores, equipos y las aplicaciones y servicios con el fin de convertir Internet en un lugar más seguro. [**Zed Attack Proxy**](https://www.zaproxy.org/), ZAP, es una de las herramientas libres de este proyecto cuya principal finalidad es monitorizar la seguridad de redes y aplicaciones web en busca de cualquier posible fallo de seguridad, mala configuración e incluso vulnerabilidad aún desconocida que pueda suponer un problema para la red.

![](https://www.redeszone.net/app/uploads-redeszone.net/2020/05/ZAP-logo.jpg)

ZAP es una herramienta realmente completa, y si eres nuevo en las auditorías, te será bastante compleja de hacer funcionar, pero una vez que sabes cómo funciona, es una de las mejores que puedes tener en tu arsenal de herramientas. En la web oficial de ZAP nos invitan a ver todos los vídeos de su herramienta donde nos enseñarán cómo funciona y de todo lo que es capaz de hacer.

Por último, ZAP tiene una tienda de addons para aumentar las funcionalidades por defecto de la herramienta, estos add-ons han sido desarrollados por la comunidad que hay detrás de este proyecto.

## Nessus

[**Nessus**](https://es-la.tenable.com/products/nessus) es un programa de escaneo de vulnerabilidades para todos los sistemas operativos, consiste en un demonio nessusd que realiza el escaneo del sistema operativo objetivo, y nessus el cliente que muestra el avance e informa de todo lo que va encontrando en los diferentes escaneos. Nessus se puede ejecutar tanto a nivel de consola por comandos, o también con interfaz gráfica de usuario. Nessus primero empieza realizando un escaneo de puertos, ya que es lo primero que se suele hacer en un pentesting, Nessus hace uso de la potencia de Nmap para ello, aunque también tiene su propio escáner de puertos abiertos.

Esta herramienta permite exportar los resultados del escaneo en diferentes formatos, como texto plano, XML, HTML y LaTeX, además, toda la información se gaurda en una base de datos de «conocimiento» para posteriores revisiones. Actualmente Nessus tiene una versión gratuita muy limitada, y posteriormente una versión de pago mucho más completa y con soporte de la empresa que tiene detrás.

Algunas características muy importantes de Nessus son que tiene muy pocos falsos positivos, tiene una gran cobertura de vulnerabilidades y es utilizada ampliamente por toda la industria de la seguridad, por lo que se actualiza casi continuamente para incorporar las últimas tecnologías y fallos de seguridad de las aplicaciones.

## Seccubus

[**Seccubus**](https://www.seccubus.com/) es una herramienta que utiliza otros escáneres de vulnerabilidades y automatiza la tarea lo máximo posible. Aunque este no es un escáner propiamente dicho como los anteriores, esta aplicación une varios de los escáneres más populares del mercado, como Nessus, OpenVAS, NMap, SSLyze, Medusa, SkipFish, OWASP ZAP y SSLlabs y nos permite automatizar todos los análisis de manera que desde esta única aplicación podamos realizar un análisis lo más profundo posible, además de poder programas análisis a intervalos regulares para asegurarnos de que todos los equipos y las redes están siempre correctamente protegidas y, en caso de que algo vaya mal, recibir avisos en tiempo real.

## Uniscan

Una de las aplicaciones más conocidas dentro de este tipo de aplicaciones para buscar vulnerabilidades es [**Uniscan**](https://tools.kali.org/web-applications/uniscan). Las principales características de esta herramienta son que es una de las más sencillas para la búsqueda de vulnerabilidades, pero también una de las más potentes, siendo capaz de buscar fallos de seguridad críticos en los sistemas. Es capaz de localizar fallos desde el acceso a los archivos locales, hasta la ejecución de código remoto, e incluso es capaz de cargar archivos de forma remota a los sistemas vulnerables. También permite realizar un seguimiento de huella digital y listar los servicios, archivos y directorios de cualquier servidor.

![Uniscan](https://www.redeszone.net/app/uploads-redeszone.net/2020/02/Uniscan.jpg)

Esta es una de las aplicaciones base de muchas distribuciones Linux de hacking ético, como **Kali Linux**, por lo que si usamos esta distro de hacking ético no tendremos que descargar ni instalar nada para poder usarla.

## Metasploit

[**Metasploit**](https://www.metasploit.com/) es una de las mejores herramientas de código abierto que nos permite localizar y explotar vulnerabilidades de seguridad en sistemas y servicios, esta herramienta es fundamental para realizar pentesting. El proyecto más popular es Metasploit Framework, el cual se encuentra instalado de manera predeterminada en distribuciones Linux como Kali Linux. Gracias a la potencia de Metasploit, podremos realizar pruebas de penetración a servicios, aplicaciones y demás ataques.

Es una de las herramientas que debes tener en tu arsenal de herramientas para realizar pentesting, se complementa con el resto de herramientas que hemos hablado anteriormente. Metasploit tiene una gran comunidad detrás, y se han diseñado herramientas basadas en esta para facilitar enormemente todas las tareas automatizándolas.

## WMAP

**WMAP** es un escáner de vulnerabilidades que ha sido diseñado como un módulo para Metasploit. Este escáner de vulnerabilidades es prácticamente igual a Uniscan, ya que tiene los mismos tests y proporciona una información más o menos similar.

![WMAP Metasploit](https://www.redeszone.net/app/uploads-redeszone.net/2020/02/WMAP-Metasploit.jpg)

Un detalle importante es que su uso es más complicado ya que debe ser lanzado directamente desde Metasploit, por lo que si utilizamos habitualmente esta herramienta, entonces esta extensión nos vendrá genial para complementar su funcionamiento.

## Burp Suite

Otra alternativa más para auditar la seguridad de sistemas, webs y redes en busca de vulnerabilidades es [**Burp Suite**](https://portswigger.net/burp). Esta es una de las herramientas más completas que podemos encontrar dentro de este tipo de software, aunque está diseñada con el fin de convertirse en una herramienta comercial.

![BurpSuite](https://www.redeszone.net/app/uploads-redeszone.net/2020/02/BurpSuite.png)

Tenemos una versión gratuita que está muy limitada, y luego tenemos versiones de pago que desbloquea el resto de opciones de configuración avanzadas. Aunque exista esta versión de «Community Edition» que es gratis, la verdad es que esta versión gratuita carece de funciones y características interesantes, como la posibilidad de lanzar escáneres manuales.

## Vega

**Vega** es la alternativa perfecta a Burp Suite, pero desarrollado de forma totalmente gratuita y de código abierto. Esta herramienta puede utilizarse como un proxy gratis y, además, cuenta con un motor para buscar vulnerabilidades en cualquier sistema o red, además de otras brechas de seguridad.

El principal punto fuerte de Vega es que se trata de una herramienta muy flexible, pudiendo encontrar una versión para Linux, macOS y Windows, aunque para este último sistema solo lo encontraremos con interfaz gráfica, GUI. Esta herramienta es una de las fundamentales para realizar tareas de pentesting y escáner de vulnerabilidades web.

![Vega](https://www.redeszone.net/app/uploads-redeszone.net/2020/02/Vega.png)

## Nikto

Los usuarios avanzados que quieren una herramienta potente, y que devuelva unos resultados muy exhaustivos para ver en detalle todo lo que tiene la red y/o el sistema objetivo, recurren a Nikto.

![Nikto](https://www.redeszone.net/app/uploads-redeszone.net/2020/02/nikto-windows-version.png)

Esta herramienta es totalmente gratuita y está escrita en Perl, su funcionamiento es muy similar al de otras herramientas vistas anteriormente, pero la principal diferencia es que devuelve unos resultados mucho más detallados, lo que es de agradecer tanto para los usuarios más avanzados como para los iniciados, ya que te permitirá aprender rápidamente sobre todo lo que reporta, y aprender más sobre vulnerabilidades.

## Acunetix

Esta es una herramienta que se caracteriza por escanear aplicaciones basadas en web, pero eso no quiere decir que esté limitada, ya que tiene un escáner de subprocesos múltiple que tiene la capacidad de analizar cientos de miles de páginas de manera muy rápida e identificar al mismo tiempo los problemas más comunes de configuración de servidores web, podemos destacar que es bastante buena para escanear en WordPress y además incluye integraciones bastante interesantes como Jenkins, GitHub y Jira.

Puedes descargarla en este **[enlace](https://www.acunetix.com/plp/web-vulnerability-scanner/?utm_term=acunetix&utm_campaign=1077471751&utm_content=55423374169&utm_source=Adwords&utm_medium=cpc&gclid=Cj0KCQjwntCVBhDdARIsAMEwACk_zsiBoED7kCRC_bl2IHgoVnldMe7yXvUC_ClTnQFWaQp2tib6bAEaAmkYEALw_wcB)**.

![](https://www.redeszone.net/app/uploads-redeszone.net/2020/05/Acunetix.png)

## Intruder

**[Intruder](https://www.intruder.io/)** se trata de un scanner proactivo de vulnerabilidades basado en la nube y concentra su actividad en el escaneo perimetral, es bastante bueno para descubrir nuevas vulnerabilidades, pero a nivel empresarial necesita complementarse en la mayoría de casos con otras herramientas, es una buena opción para quienes buscar tener una barrera más a nivel perimetral.

![](https://www.redeszone.net/app/uploads-redeszone.net/2020/05/intruder.png)

## IBM Security QRadar

Que podemos decir de IBM que no se sepa, es uno de los proveedores de seguridad más reconocidos a nivel mundial, y esta herramienta está a la altura de la reputación de la empresa, ya que permite escanear la red, correlacionar la información con su topología y los datos de las conexiones de la misma.

![](https://www.redeszone.net/app/uploads-redeszone.net/2020/05/IBM-Security-QRadar.png)

Tiene la capacidad de administrar el factor de riesgo mediante un motor de políticas basadas en verificaciones de cumplimiento automatizadas y nos presta un análisis avanzado bastante poderoso que nos permitirá prevenir violaciones de ciberseguridad además de priorizar y realizar las acciones necesarias para regular y remediar cualquier inconveniente que surja. Puedes descargarla **[aquí](https://www.ibm.com/es-es/qradar?utm_content=SRCWW&p1=Search&p4=43700068026951379&p5=e&gclid=Cj0KCQjwntCVBhDdARIsAMEwACkfrpMP4sD3euZdn68dBYY0G5OwMzcG8T5ZTMG8nahrkvkjGpr1SNEaAo00EALw_wcB&gclsrc=aw.ds)**.

## Amazon Inspector

Si eres usuario de AWS, **[Amazon Inspector](https://aws.amazon.com/es/inspector/?tag=redeszone-21)** es una herramienta es excelente para ti, ya que se trata de un servicio automatizado para la evaluación de seguridad que se encarga de escanear todas las aplicaciones implementadas en AWS y además puede ser utilizado en las instancias de Amazon EC2.

![](https://www.redeszone.net/app/uploads-redeszone.net/2020/05/Amazon-Inspector.png)

Además de la evaluación de vulnerabilidades también nos proporciona una lista bastante detallada de posibles vulnerabilidades y las prioriza al mismo tiempo según el nivel de riesgo que tenga.

### Características de Amazon Inspector

- **Entorno:** Amazon Inspector tiene la capacidad de administrar varias cuentas de forma centralizada. Esto es mediante una cuenta ASWOrganizations, y asignando una como administrador delegado de Inspector. Dejando así la opción de activar toda la organización de forma rápida y sencilla.  Este administrador puede gestionar los datos de los hallazgos y muchos otros ajustes de todos los miembros.
- **Exploración:** Con esta herramienta no es necesario realizar una programación de forma manual para los análisis. Esta descubre e inicia los escaneos de forma automática. Incluso durante este proceso sigue realizando una evaluación de todos los recursos, siempre y cuando se realice algún cambio en estos. Si detecta alguna vulnerabilidad o una ruta abierta, nos permite investigar el descubrimiento. Nos dará información como el recurso afectado, y recomendaciones para solucionarlo lo antes posible.
- **Evaluación de vulnerabilidades:** Según va recibiendo información de los análisis, nos proporciona una puntuación sobre la gravedad específica adaptadas al entorno que tenemos montado.
- **Identificar problemas:** En el panel de control se pueden ver los detalles de los problemas de alto impacto. Recientemente, Amazon rediseñó esta función para tener la información más simplificada sobre el escaneo del entorno. Donde podemos ver cuántos errores críticos hay, y qué recursos tienen más hallazgos. Todo esto tiene cierto grado de personalización. En cada pantalla podemos cambiar algunos parámetros para modificar el resultado que vamos a tener visible. Así como dar uso de filtros para crear reglas para ocultar o mostrar hallazgos.

Por otro lado, Amazon Inspector cuenta con herramientas añadidas para poder mejorar la supervisión. Estas son:

- Consola de administración.
- Herramientas de líneas de comandos.
- SDKs de Amazon Web Services.
- APIs de REST de Amazon Inspector.

En definitiva, estamos ante una herramienta muy útil para detectar vulnerabilidades que nos permite un buen grado de personalización. Esto nos permite realizar búsquedas muy precisas, para que puedan ser solucionadas lo antes posible.

## Precauciones

Siempre y cuando vamos a utilizar este tipo de programas o herramientas como puede ser Wireshark, debemos tener claro que esto puede ser peligroso para los usuarios. Al escanear los paquetes que se transportan por la red, podemos tener gran cantidad de información en nuestra mano. Esto hace que sea más sencillo que se produzca alguna filtración de datos. Por lo cual siempre se deben utilizar de forma adecuada, y con fines legales. Si bien el uso de este tipo de aplicaciones no es ilegal, todo lo contrario, debemos tener cuidado con su uso.

Tal y como habéis visto, tenemos una grandísima cantidad de programas para realizar escaneos de vulnerabilidades a nuestras redes, equipos, servicios web y otros servicios que incorporan los servidores. Dependiendo de lo que estemos realizando, tendremos que utilizar un escáner u otro.