# CPD para sistemas de cámaras con reconocimiento automático de matriculas

# Definición Del Proyecto

El objetivo es crear un **CPD** para toda la policía de la comarca **La Safor**, en la cual mediante las **cámaras de control de vehículos** de cada municipio, vayan leyendo las **matrículas** de cada coche, para después, se envíe al CPD con el **día, la hora, la calle y el número de cámara**, para que cualquier policía de la Safor desde su comisaría pueda buscar la matrícula y le aparezca **por dónde va o ha ido** un vehículo.

Las cámaras estarán equipadas con una **tarjeta SIM** que permitirá su conexión con el CPD. Una vez establecida la conexión, el sistema podrá recibir y procesar los datos capturados por cada cámara, incluyendo:

- **Matrícula**
- **Fecha y hora**
- **Localidad y calle**

En el CPD, los servidores operan con **Windows Server**, encargado de gestionar los datos y facilitar el acceso a la plataforma web. Desde cualquier comisaría policial de la comarca de La Safor, los agentes, mediante una **clave de acceso** proporcionada, podrán consultar el historial de circulación de un vehículo introduciendo su número de matrícula.

> **Nota:** El sistema **no almacena imágenes captadas por las cámaras**, sino únicamente los **datos derivados**, garantizando que el CPD se enfoque en la gestión de datos y no en la vigilancia policial.

---

## Datos Generales del Proyecto

- **Ubicación del CPD**: Polígono industrial Benieto, Gandia.
- **¿Quién realizará las instalaciones?**  
  La instalación del CPD y de las cámaras será realizada por el **personal contratado** para el mantenimiento y gestión del centro.  
  - No se contratarán empresas externas, reduciendo costes.
  - Se contará con **profesionales graduados en CFGS de Administración de Sistemas Informáticos y Redes**.

---

## Esquema Técnico

El **Centro de Procesamiento de Datos (CPD)** está diseñado para garantizar **seguridad, eficiencia y continuidad operativa**.

- **Infraestructura**:
  - **Servidores de alto rendimiento**
  - **Almacenamiento NAS/SAN**
  - **Switches avanzados**
  - **Generadores con autonomía de 12 horas**
- **Software**:
  - Plataforma de monitoreo
  - Integración con cámaras municipales
- **Seguridad y respaldo**:
  - **Respaldo diario fuera del sitio**
  - **Mobiliario ergonómico**
  - **Armarios de seguridad**

### 1. Planta

#### Distribución de espacios:

- **Sala de servidores principal**: 50 m²  
  - Hardware crítico del CPD (servidores, racks, switches).
- **Sala de comunicaciones**: 25 m²  
  - Gestión de redes y telecomunicaciones.
- **Sala de control y monitoreo**: 40 m²  
  - Centro de operaciones con pantallas para visualización de datos.
- **Almacenamiento y archivo**  
  - Espacio para copias de seguridad físicas y digitales.
- **Área de soporte técnico**: 30 m²  
  - Espacio para técnicos y herramientas.
- **Sala de energía y climatización**: 20 m²  
  - Ubicación de **UPS, generadores y sistemas de aire acondicionado**.

---

## Hardware

### **1. Equipos Necesarios**
- **Servidores** de procesamiento de imágenes (ALPR), almacenamiento y base de datos (**3-6 servidores**).
- **Almacenamiento en red (NAS/SAN)**: **2-4 unidades** para redundancia.
- **Equipos de red** (switches, routers, firewalls): **2-3 unidades**.
- **Espacio de crecimiento futuro**: **20-30% adicional**.

### **2. Capacidad de un Rack Estándar**
- Un rack típico mide **42U** (1U = 1.75 pulgadas de altura).
- **Servidores estándar** ocupan **1U-2U** cada uno.
- **Equipos de almacenamiento** ocupan **4U-8U** por unidad.
- **Switches y routers** ocupan **1U-2U** cada uno.

**Distribución de espacio estimado:**
- **Servidores**: 6 servidores × 2U = **12U**.
- **Almacenamiento**: 4 unidades × 6U = **24U**.
- **Equipos de red**: 3 equipos × 2U = **6U**.
- **Espacio adicional** (PDUs, cableado, mantenimiento): **5U**.
- **Espacio reservado** para crecimiento futuro: **20U**.

**Total espacio necesario**: **75U**.

### **3. Racks Necesarios**
- Cada rack tiene **42U**, pero se recomienda usar **70-80%** por ventilación y cableado.
- Usando **30U-34U útiles por rack**, se necesitarán **3 racks**.
  - **Rack 1**: Servidores y switches principales.
  - **Rack 2**: Almacenamiento y equipos secundarios.
  - **Rack 3**: Redundancia y crecimiento futuro.

---

## Tarjetas SIM

Se optó por usar **tarjetas SIM** en lugar de antenas **P2P**, debido a:
- **Grandes distancias y montañas** que dificultan la conexión P2P.
- **Menos pérdidas de datos y mejor estabilidad** con la red de telefonía móvil.
- **Menor coste y tiempo de instalación**.

**Total de tarjetas SIM necesarias**: **478** (una por cada cámara).  

---

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
**¿Por qué?**  
Estas zonas concentran alto tráfico, especialmente en horas punta.

**Beneficios**  
- Permiten **monitorear el flujo** de vehículos.  
- Ayudan a **detectar congestión** y **supervisar accesos**.  

Las cámaras deben instalarse en **las entradas/salidas de todos los municipios sin excepción** para maximizar la seguridad y la eficiencia del tráfico.

---

