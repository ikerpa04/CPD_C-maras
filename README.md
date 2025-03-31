# CPD para sistemas de cámaras con reconocimiento automático de matriculas
## Definición del Proyecto
El objetivo es crear un CPD para toda la policía de la comarca la Safor, en la cual mediante las cámaras de control de vehículos de cada municipio, vayan leyendo las matrículas de cada coche, para después, se envíe al CPD con el día, la hora, la calle y el número de cámara, para que cualquier policía de la Safor desde su comisaría pueda buscar la matrícula y le aparezca por donde va o ha ido x vehiculo.

Las cámaras estarán equipadas con una tarjeta SIM que permitirá su conexión con el CPD. Una vez establecida la conexión, el sistema podrá recibir y procesar los datos capturados por cada cámara, incluyendo el número de matrícula, fecha, hora, localidad y calle.

En el CPD, los servidores operan con Windows Server, encargado de gestionar los datos y facilitar el acceso a la plataforma web. Desde cualquier comisaría policial de la comarca de La Safor, los agentes, mediante una clave de acceso proporcionada por nosotros, podrán consultar el historial de circulación de un vehículo introduciendo su número de matrícula.

Es importante destacar que el sistema no almacena imágenes captadas por las cámaras , sino únicamente los datos derivados, como la matrícula, fecha, hora y localización. Esto garantiza que el CPD se enfoque en la gestión de datos y no en la vigilancia policial.

##Datos generales del proyecto

**Ubicación del CPD:** Polígono industrial Benieto, Gandia.

**¿Quién realizará las instalaciones?¿Nosotros o una empresa externa?** 

La instalación del CPD y de las cámaras será realizada por el personal contratado para el mantenimiento y gestión del centro.

Ahorramos en gastos extra al contratar terceras personas y contaremos con personal cualificado para realizar dicha tarea.

El personal que buscaremos serán profesionales graduados en CFGS de Administración de Sistemas Informáticos y Redes.

##Esquema técnico
El Centro de Procesamiento de Datos (CPD) está diseñado para garantizar seguridad, eficiencia y continuidad operativa.
El CPD contará con servidores de alto rendimiento, almacenamiento NAS/SAN, switches avanzados y generadores de autonomía de 12 horas. 

A nivel de software, incluirá una plataforma de monitoreo e integración con cámaras municipales.
Finalmente, se implementarán respaldo diario fuera del sitio, mobiliario ergonómico en la sala de monitoreo y armarios de seguridad, garantizando una operación eficiente y protegida. Este diseño asegura un CPD escalable, confiable y preparado para futuras necesidades.
**1. Planta**
***Distribución de espacios con sus respectivas funciones:***
  Sala de servidores principal: Alojará el hardware crítico del CPD, como los servidores, los racks, switches, .
Sala de comunicaciones: Gestión de redes y telecomunicaciones.
Sala de control y monitoreo: Centro de operaciones con pantallas para visualización de datos y cámaras.
Almacenamiento y archivo: Espacio dedicado a copias de seguridad físicas y digitales.
Área de soporte técnico: Espacio para técnicos y herramientas.
Sala de energía y climatización: Ubicación de UPS, generadores y sistemas de aire acondicionado.
Zonas de acceso restringido y seguridad.
