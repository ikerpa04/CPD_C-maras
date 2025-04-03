# CPD para sistemas de cámaras con reconocimiento automático de matriculas
## Definición del Proyecto
El objetivo es crear un CPD para toda la policía de la comarca la Safor, en la cual mediante las cámaras de control de vehículos de cada municipio, vayan leyendo las matrículas de cada coche, para después, se envíe al CPD con el día, la hora, la calle y el número de cámara, para que cualquier policía de la Safor desde su comisaría pueda buscar la matrícula y le aparezca por donde va o ha ido x vehiculo.

Las cámaras estarán equipadas con una tarjeta SIM que permitirá su conexión con el CPD. Una vez establecida la conexión, el sistema podrá recibir y procesar los datos capturados por cada cámara, incluyendo el número de matrícula, fecha, hora, localidad y calle.

En el CPD, los servidores operan con Windows Server, encargado de gestionar los datos y facilitar el acceso a la plataforma web. Desde cualquier comisaría policial de la comarca de La Safor, los agentes, mediante una clave de acceso proporcionada por nosotros, podrán consultar el historial de circulación de un vehículo introduciendo su número de matrícula.

Es importante destacar que el sistema no almacena imágenes captadas por las cámaras , sino únicamente los datos derivados, como la matrícula, fecha, hora y localización. Esto garantiza que el CPD se enfoque en la gestión de datos y no en la vigilancia policial.

## Datos generales del proyecto

**Ubicación del CPD:** Polígono industrial Benieto, Gandia.

**¿Quién realizará las instalaciones?¿Nosotros o una empresa externa?** 

La instalación del CPD y de las cámaras será realizada por el personal contratado para el mantenimiento y gestión del centro.

Ahorramos en gastos extra al contratar terceras personas y contaremos con personal cualificado para realizar dicha tarea.

El personal que buscaremos serán profesionales graduados en CFGS de Administración de Sistemas Informáticos y Redes.

## Esquema técnico
El Centro de Procesamiento de Datos (CPD) está diseñado para garantizar seguridad, eficiencia y continuidad operativa.
El CPD contará con servidores de alto rendimiento, almacenamiento NAS/SAN, switches avanzados y generadores de autonomía de 12 horas. 

A nivel de software, incluirá una plataforma de monitoreo e integración con cámaras municipales.
Finalmente, se implementarán respaldo diario fuera del sitio, mobiliario ergonómico en la sala de monitoreo y armarios de seguridad, garantizando una operación eficiente y protegida. Este diseño asegura un CPD escalable, confiable y preparado para futuras necesidades.

**1. Planta**

### Distribución de espacios con sus respectivas funciones:

> Sala de servidores principal: Alojará el hardware crítico del CPD, como los servidores, los racks, switches, .

> Sala de comunicaciones: Gestión de redes y telecomunicaciones.

> Sala de control y monitoreo: Centro de operaciones con pantallas para visualización de datos y cámaras.

> Almacenamiento y archivo: Espacio dedicado a copias de seguridad físicas y digitales.

> Área de soporte técnico: Espacio para técnicos y herramientas.

> Sala de energía y climatización: Ubicación de UPS, generadores y sistemas de aire acondicionado.

> Zonas de acceso restringido y seguridad.

### Dimensiones (medidas)

> Sala de servidores: 50 m².
 
> Sala de comunicaciones: 25 m².

> Sala de control: 40 m².

> Espacio técnico: 30 m².

> Sala de energía y climatización: 20 m²

### Mobiliario sugerido

***Hardware***

> Servidores de alta capacidad con redundancia.

> Almacenamiento escalable en red (NAS o SAN).

> Switches y routers de última generación con soporte para VLAN.

> UPS y generadores con autonomía de 12 horas mínimo.

***Software***

> Sistema de gestión de bases de datos para registro de matrículas.

> Plataforma centralizada de monitoreo.

> Sistema de gestión de accesos y registros.

***Otros Requisitos***

> Enlaces de red redundantes con alto ancho de banda.

> Integración con cámaras de vigilancia municipales.

> Seguridad física: Control de acceso biométrico y videovigilancia.

> Sistema de respaldo diario con almacenamiento fuera del sitio.

> Escritorios y sillas ergonómicas en sala de monitoreo.

> Armarios para almacenamiento seguro de equipos.

## Material a utilizar

### Equipos necesarios:

Servidores de procesamiento de imágenes (ALPR), servidores de almacenamiento y de base de datos: Aproximadamente 3-6 servidores dependiendo del volumen de datos.
Almacenamiento en red (NAS/SAN): 2-4 unidades para garantizar redundancia.
Equipos de red (switches, routers, firewalls): 2-3 unidades.
Espacio para crecimiento futuro: Se recomienda al menos un 20-30% adicional.

### Capacidad de un rack estándar:

> Un rack típico mide 42U (1U = 1.75 pulgadas de altura).

> Servidores estándar ocupan entre 1U y 2U cada uno.

> Equipos de almacenamiento suelen ocupar entre 4U y 8U por unidad.

> Switches y routers: 1U-2U cada uno.

## Estimación total de espacio necesario:

> Servidores: Unos 6 servidores x 2U = 12U.

> Almacenamiento: 4 unidades x 6U (promedio) = 24U.

> Equipos de red: 3 equipos x 2U = 6U.

> Espacio adicional para PDUs (distribución de energía) y mantenimiento: 5U.

> Espacio reservado para crecimiento futuro: 20U.

> Total: 75U de espacio necesario.

## Distribución en racks:

> Cada rack tiene 42U, pero por ventilación y cableado no se debe llenar al 100%.

> Usando un 70-80% de capacidad por rack, cada uno puede albergar 30U-34U útiles.

## Racks necesarios:

> 3 racks serán suficientes (2 llenos + 1 para redundancia y expansión).

## Distribución sugerida de los racks

>> Rack 1: Servidores y switches principales.

>> Rack 2: Almacenamiento y equipos secundarios.

>> Rack 3: Redundancia, espacio para futuros equipos y crecimiento.

Para garantizar un diseño eficiente del Centro de Procesamiento de Datos (CPD) y cumplir con los requerimientos del proyecto, se ha realizado una estimación detallada de los equipos necesarios y su distribución en racks. A continuación, se justifica por qué se requieren tres racks.

*Un rack típico tiene 42U, pero en la práctica no se puede ocupar al 100% debido a varios factores:*

· Ventilación y flujo de aire: Se recomienda dejar un margen de al menos un 20-30% libre para evitar sobrecalentamiento y permitir un flujo de aire adecuado.

· Gestión de cableado: Un espacio adicional permite una mejor organización del cableado de red y energía, reduciendo interferencias y mejorando la accesibilidad para mantenimiento.

· Expansión futura: Contar con espacio libre dentro de los racks facilita la incorporación de nuevos equipos sin necesidad de reorganizar o trasladar equipos ya instalados.

Por estos motivos, se considera que cada rack puede utilizar entre 30U y 34U de manera eficiente.

## Tarjetas SIM

Hemos cambiado la opción de instalar antenas P2P, por las tarjetas SIM, ya que en verdad hay una gran distancia, montañas, etc… Es muy difícil tener una buena conexión y no tener pérdidas de conexión y datos.

Por eso hemos buscado otra opción y es la de implementar una tarjeta SIM a cada cámara, ya que así, aparte de tener una buena conexión y utilizar los servicios ya instalados de telefonía, reducimos los costes y tiempo de instalación.

Nos harán falta 478 tarjetas SIM (una por cada cámara), para conectar las cámaras por vía telefónica al CPD. 
El resultado total del número de cámaras a las que le tenemos que poner tarjetas SIM, se encuentran aquí, donde cada número al lado de el nombre de cada población es el identificador de cada una de ellas.

# Almacenamiento

## Datos de cada cámara

- **Matrícula:** 10-20 caracteres (+/- 20 bytes).
- **Hora y fecha:** +/- 16 caracteres (+/- 16 bytes).
- **Ubicación:** +/- 50 caracteres (+/- 50 bytes).
- **Otros datos (ID de cámara):** +/- 50 bytes.
- **Tamaño aproximado por evento:** 150 bytes/evento.

## Frecuencia de los eventos

Supongamos que cada cámara detecta un promedio de 1 vehículo por segundo (en zonas de tráfico muy alto).  

Eso equivale a:

- **60 vehículos/minuto**  
- **3.600 vehículos/hora**  
- **86.400 vehículos/día por cámara**  

## Número de cámaras

- **Total:** 478 cámaras.

## Cálculo del Almacenamiento Total

### 1. Datos por día por cámara:
- **Datos del evento:** 150 bytes.
- **Eventos diarios por cámara:** 86.400 vehículos.

### 2. Datos del día por cámara:
- `150 bytes × 86.400 vehículos por día = 12,96 MEGABYTE`

### 3. Datos por día para 478 cámaras:
- `12.96MB × 478 = 6,19 GB/día`

### 4. Datos por año para 478 cámaras:
- `6.2GB/día × 365 = 2,263 TB/año`

## Espacio Adicional para Indexación y Redundancia

### **Indexación y bases de datos**
Incrementar el tamaño estimado un **20%** por indexación:  
`2.2TB × 1.2 = 2.64TB /año`

### **Redundancia (RAID)**
Usando **RAID 6** (20%-30% más de espacio requerido):  
`2.64TB × 1.3 = 3.43TB /año`  

**Razón para usar RAID 6:**  
RAID 6 es más seguro que RAID 5 y tiene mayor disponibilidad de datos.  
Permite el fallo de hasta **2 discos sin pérdida de datos**, ya que cuenta con doble paridad.

## Recomendación de Tamaño del NAS/SAN

### **1. Capacidad por tiempo de retención:**
- **1 año de retención:** 3.5 TB de capacidad útil.
- **5 años de retención:** 17.5 TB de capacidad útil.

### **2. Considerar crecimiento futuro:**
Con un margen adicional del **50%** para crecimiento:
- **1 año de retención:** 5 TB.
- **5 años de retención:** 26 TB.

### **3. Configuración del almacenamiento:**
Para cubrir **5 años con margen**:
- **Discos:** 8 x 8 TB HDD (64 TB brutos, 46 TB útiles en RAID 6).
- Esto permitiría cubrir hasta **10 años** si fuera necesario.

---

## **Ventajas de usar discos de mayor capacidad (8TB)**

### **1. Coste por GB más eficiente**
Los discos de mayor capacidad tienden a ser más económicos por GB comparado con discos más pequeños.

### **2. Menor número de discos necesarios**
Menos discos físicos reducen costes de infraestructura (racks, cables, etc.).

### **3. Mejor rendimiento en discos HDD**
Si se configuran correctamente en **RAID 6**, los discos grandes pueden ofrecer velocidad similar a discos pequeños.

### **4. Menos consumo de energía y menos espacio**
Menos discos físicos = **menor consumo energético** y más espacio libre en el CPD.

### **5. Escalabilidad**
Los discos de mayor capacidad facilitan la expansión sin necesidad de cambiar la infraestructura.

### **6. Resiliencia a largo plazo**
RAID 6 ofrece **redundancia adicional** y reduce el riesgo de fallos simultáneos.

---

# **Infraestructura del CPD**

## **1. Cortes o secciones**
- **Altura mínima:** 3 metros para garantizar la ventilación.
- **Acceso restringido** en áreas críticas.
- **Instalación de sistemas** de aire acondicionado, bandejas portacables y sistemas contra incendios.

## **2. Fachadas**
- **Diseño minimalista** y reforzado.
- **Materiales resistentes** al clima y vandalismo.
- **Indicación clara** de accesos y salidas de emergencia.

## **3. Detalles constructivos**
- **Sistema de refrigeración redundante (N+1).**
- **Suelos elevados** para paso de cableado.
- **Sistemas contra incendios** con gases inertes.

## **4. Planos estructurales**
- **Columnas y vigas** diseñadas para soportar la carga de los equipos.
- **Pisos elevados** y **paredes aisladas térmica y acústicamente**.

## **5. Instalaciones**

### **Eléctricas:**
- **Circuitos separados** para equipos esenciales y no esenciales.
- **Iluminación LED** distribuida uniformemente.
- **UPS y generadores** para redundancia eléctrica.

### **Hidrosanitarias:**
- **Drenaje** para posibles escapes de agua.
- **Suministro de agua** para refrigeración.

### **Mecánicas o especiales:**
- **Aire acondicionado redundante**.
- **Ventilación controlada** y **monitoreo de humedad**.

---

# **Especificaciones Técnicas**

## **1. Materiales y acabados**
- **Suelos:** Antiestáticos, elevados y de fácil mantenimiento.
- **Paredes:** Revestimientos ignífugos y aislantes acústicos.
- **Techos:** Paneles desmontables para mantenimiento.

## **2. Información Gráfica y Simbólica**
- **Simbología**: Identificación de puertas, ventanas, racks, bandejas y tomas eléctricas.
- **Orientación Norte** para facilitar la ubicación del proyecto.
- **Texturas y colores**:
  - **Concreto:** Gris moteado.
  - **Vidrio:** Transparente con bordes azules.
  - **Madera:** Marrón claro para detalles no críticos.

---

# **Ubicación de las Cámaras de Control de Tráfico**

### **Entradas y salidas de la población**
📍 **¿Por qué?**  
Estas zonas concentran alto tráfico, especialmente en horas punta.

✅ **Beneficios**  
- Permiten **monitorear el flujo** de vehículos.  
- Ayudan a **detectar congestión** y **supervisar accesos**.  

📌 **Conclusión:**  
Las cámaras deben instalarse en **las entradas/salidas de todos los municipios sin excepción** para maximizar la seguridad y la eficiencia del tráfico.
