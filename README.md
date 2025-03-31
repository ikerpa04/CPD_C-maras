# CPD para sistemas de cámaras con reconocimiento automático de matriculas
## Definición del Proyecto
El objetivo es crear un CPD para toda la policía de la comarca la Safor, en la cual mediante las cámaras de control de vehículos de cada municipio, vayan leyendo las matrículas de cada coche, para después, se envíe al CPD con el día, la hora, la calle y el número de cámara, para que cualquier policía de la Safor desde su comisaría pueda buscar la matrícula y le aparezca por donde va o ha ido x vehiculo.

Las cámaras estarán equipadas con una tarjeta SIM que permitirá su conexión con el CPD. Una vez establecida la conexión, el sistema podrá recibir y procesar los datos capturados por cada cámara, incluyendo el número de matrícula, fecha, hora, localidad y calle.

En el CPD, los servidores operan con Windows Server, encargado de gestionar los datos y facilitar el acceso a la plataforma web. Desde cualquier comisaría policial de la comarca de La Safor, los agentes, mediante una clave de acceso proporcionada por nosotros, podrán consultar el historial de circulación de un vehículo introduciendo su número de matrícula.

Es importante destacar que el sistema no almacena imágenes captadas por las cámaras , sino únicamente los datos derivados, como la matrícula, fecha, hora y localización. Esto garantiza que el CPD se enfoque en la gestión de datos y no en la vigilancia policial.
