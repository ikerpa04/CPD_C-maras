# CPD para sistemas de cámaras con reconocimiento automático de matrículas

```
Daniel Ibáñez Martí - Iker Ariel Patiño Alvarez - Francisco Sánchez Garcia
```

## ÍNDICE

- Definición Del Proyecto
- Datos Generales del proyecto
- Esquema Técnico
- Material a utilizar
- Distribución sugerida de los racks
   - Tarjetas SIM
- Almacenamiento
- Cálculo del Almacenamiento Total
- Espacio Adicional para Indexación y Redundancia
- Recomendación de Tamaño del NAS/SAN
   - 1. Cortes o secciones
   - 2. Fachadas
   - 3. Detalles constructivos
   - 4. Planos estructurales
   - 5. Instalaciones
- Especificaciones Técnicas
   - 1. Materiales y acabados
- Información Gráfica y Simbólica
   - 1. Simbología
   - 2. Norte
   - 3. Texturas y colores
- Ubicación de las cámaras de control de tráfico
- Presupuesto del Material
- Costes Aproximados de las cámaras:
- Costes de las tarjetas SIM:
- Evaluación de riesgos
   - RIESGOS DE SEGURIDAD INFORMÁTICA
   - RIESGOS OPERATIVOS
   - RIESGOS DE PRIVACIDAD
   - RIESGOS FÍSICOS
   - RIESGOS TECNOLÓGICOS
- Planes de contingencia
   - CONTINGENCIA PARA CIBERATAQUES
   - CONTINGENCIA PARA FALLOS OPERATIVOS
   - CONTINGENCIA PARA DESASTRES FÍSICOS
   - CONTINGENCIA DE PRIVACIDAD
   - PLAN DE FORMACIÓN Y SIMULACROS

  - 5 Arquitectura del CPD
      - Infraestructura Física
      - Infraestructura de Red
      - Servidores y Almacenamiento
- Diagrama de los Racks
   - Configuraciones Implementadas
      - Configuración de Red
      - Seguridad y Protección
   - Decisiones Tomadas
      - Redundancia y Alta Disponibilidad
      - Seguridad
      - Escalabilidad
   - Manuales de Usuario y Guías de Administración
      - Manual de Usuario
      - Guía de Administración
   - Procedimientos de Mantenimiento y Gestión de Recursos
      - Procedimientos de Mantenimiento
      - Gestión de Recursos
      - Plan de Respuesta ante Incidentes
   - Conclusión
- Seguridad Informática
   - Protección contra Amenazas
   - Protección de Recursos del CPD
- Plan de Recuperación del CPD
   - Copias de seguridad
   - Almacenamiento Seguro de copias
   - Restauración Rápida
   - Mecanismos Redundantes

## Definición Del Proyecto

El objetivo es crear un CPD para toda la policía de la comarca la Safor, en la cual
mediante las cámaras de control de vehículos de cada municipio, vayan leyendo las
matrículas de cada coche, para después, se envíe al CPD con el día, la hora, la calle y
el número de cámara, para que cualquier policía de la Safor desde su comisaría pueda
buscar la matrícula y le aparezca por donde va o ha ido x vehiculo.

Las cámaras estarán equipadas con una tarjeta SIM que permitirá su conexión con el
CPD. Una vez establecida la conexión, el sistema podrá recibir y procesar los datos
capturados por cada cámara, incluyendo el número de matrícula, fecha, hora, localidad
y calle.

En el CPD, los servidores operan con Windows Server, encargado de gestionar los
datos y facilitar el acceso a la plataforma web. Desde cualquier comisaría policial de la
comarca de La Safor, los agentes, mediante una clave de acceso proporcionada por
nosotros, podrán consultar el historial de circulación de un vehículo introduciendo su
número de matrícula.

Es importante destacar que el sistema no almacena imágenes captadas por las
cámaras , sino únicamente los datos derivados, como la matrícula, fecha, hora y
localización. Esto garantiza que el CPD se enfoque en la gestión de datos y no en la
vigilancia policial.


## Datos Generales del proyecto

**Ubicación del CPD:** Polígono industrial Benieto, Gandia.

**¿Quién realizará las instalaciones?¿ Nosotros o una empresa externa?**
La instalación del CPD y de las cámaras será realizada por el personal contratado para
el mantenimiento y gestión del centro.

Ahorramos en gastos extra al contratar terceras personas y contaremos con personal
cualificado para realizar dicha tarea.

El personal que buscaremos serán profesionales graduados en CFGS de
Administración de Sistemas Informáticos y Redes.

## Esquema Técnico

- El **Centro de Procesamiento de Datos (CPD)** está diseñado para garantizar
**seguridad, eficiencia y continuidad operativa**.

- El CPD contará con **servidores de alto rendimiento, almacenamiento NAS/SAN,
switches avanzados y generadores de autonomía de 12 horas**.

- A nivel de software, incluirá una **plataforma de monitoreo e integración con cámaras
municipales**.

- Finalmente, se implementarán **respaldo diario fuera del sitio, mobiliario ergonómico
en la sala de monitoreo y armarios de seguridad** , garantizando una operación
eficiente y protegida. Este diseño asegura un CPD escalable, confiable y preparado
para futuras necesidades.

**1. Planta**

**Distribución de espacios con sus respectivas funciones** :

- Sala de servidores principal: Alojará el hardware crítico del CPD, como
      los servidores, los racks, switches,.
      
- Sala de comunicaciones: Gestión de redes y telecomunicaciones.
      
- Sala de control y monitoreo: Centro de operaciones con pantallas para
          visualización de datos y cámaras.
          
- Almacenamiento y archivo: Espacio dedicado a copias de seguridad
          físicas y digitales.
          
- Área de soporte técnico: Espacio para técnicos y herramientas.
       
- Sala de energía y climatización: Ubicación de UPS, generadores y
          sistemas de aire acondicionado.
          
- Zonas de acceso restringido y seguridad.



***Dimensiones (medidas) :***

 - Sala de servidores: 50 m².

 - Sala de comunicaciones: 25 m².

 - Sala de control: 40 m².

 - Espacio técnico: 30 m².

 - Sala de energía y climatización: 20 m².

**Mobiliario sugerido :**

 > Hardware

 - Servidores de alta capacidad con redundancia.

 - Almacenamiento escalable en red (NAS o SAN).

 - Switches y routers de última generación con soporte para VLAN.

 - UPS y generadores con autonomía de 12 horas mínimo.

 > Software

 - Sistema de gestión de bases de datos para registro de matrículas.

 - Plataforma centralizada de monitoreo.

 - Sistema de gestión de accesos y registros.

 > Otros Requisitos

 - Enlaces de red redundantes con alto ancho de banda.

 - Integración con cámaras de vigilancia municipales.

 - Seguridad física: Control de acceso biométrico y videovigilancia.

 - Sistema de respaldo diario con almacenamiento fuera del sitio.

 - Escritorios y sillas ergonómicas en sala de monitoreo.

 - Armarios para almacenamiento seguro de equipos.


## Material a utilizar

> Equipos necesarios:

- Servidores de procesamiento de imágenes (ALPR), servidores de
almacenamiento y de base de datos: Aproximadamente 3-6 servidores
dependiendo del volumen de datos.

- Almacenamiento en red (NAS/SAN): 2-4 unidades para garantizar
redundancia.

- Equipos de red (switches, routers, firewalls): 2-3 unidades.

- Espacio para crecimiento futuro: Se recomienda al menos un 20-30%
adicional.

> Capacidad de un rack estándar:

- Un rack típico mide 42U (1U = 1.75 pulgadas de altura).

- Servidores estándar ocupan entre 1U y 2U cada uno.

- Equipos de almacenamiento suelen ocupar entre 4U y 8U por unidad.

- Switches y routers: 1U-2U cada uno.

> Estimación total de espacio necesario:

- Servidores: Unos 6 servidores x 2U = 12U.

- Almacenamiento: 4 unidades x 6U (promedio) = 24U.

- Equipos de red: 3 equipos x 2U = 6U.

- Espacio adicional para PDUs (distribución de energía) y mantenimiento: 5U.

- Espacio reservado para crecimiento futuro: 20U.
Total: 75U de espacio necesario.

> Distribución en racks:

- Cada rack tiene 42U, pero por ventilación y cableado no se debe llenar al
100%.

- Usando un 70-80% de capacidad por rack, cada uno puede albergar
30U-34U útiles.

> Racks necesarios:

- 3 racks serán suficientes (2 llenos + 1 para redundancia y expansión).

---

## Distribución sugerida de los racks

Rack 1: Servidores y switches principales.

Rack 2: Almacenamiento y equipos secundarios.

Rack 3: Redundancia, espacio para futuros equipos y crecimiento.

Para garantizar un diseño eficiente del Centro de Procesamiento de Datos (CPD) y
cumplir con los requerimientos del proyecto, se ha realizado una estimación detallada
de los equipos necesarios y su distribución en racks. A continuación, se justifica por qué
se requieren tres racks.

Un rack típico tiene 42U, pero en la práctica no se puede ocupar al 100% debido a
varios factores:

Ventilación y flujo de aire: Se recomienda dejar un margen de al menos un 20-30% libre
para evitar sobrecalentamiento y permitir un flujo de aire adecuado.

Gestión de cableado: Un espacio adicional permite una mejor organización del cableado
de red y energía, reduciendo interferencias y mejorando la accesibilidad para
mantenimiento.

Expansión futura: Contar con espacio libre dentro de los racks facilita la incorporación
de nuevos equipos sin necesidad de reorganizar o trasladar equipos ya instalados.

Por estos motivos, se considera que cada rack puede utilizar entre 30U y 34U de
manera eficiente.

### Tarjetas SIM

Hemos cambiado la opción de instalar antenas P2P, por las tarjetas SIM, ya que en
verdad hay una gran distancia, montañas, etc... Es muy difícil tener una buena
conexión y no tener pérdidas de conexión y datos.

Por eso hemos buscado otra opción y es la de implementar *una tarjeta SIM a cada
cámara*, ya que así, aparte de tener una buena conexión y utilizar los servicios ya
instalados de telefonía, reducimos los costes y tiempo de instalación.

Nos harán falta 478 tarjetas SIM (una por cada cámara), para conectar las cámaras por
vía telefónica al CPD.

El resultado total del número de cámaras a las que le tenemos que poner tarjetas SIM,
se encuentran aquí, donde cada número al lado de el nombre de cada población es el
identificador de cada una de ellas.

### Costes de las tarjetas SIM:

**Estudio sobre las distintas compañias de telefonia:**

>> ChipIOT

ChipIOT proporciona tarjetas SIM multioperador y eSIM con cobertura global para
dispositivos IoT y M2M. Ofrecen planes personalizados y destacan por tener precios
hasta un 50% más económicos, para obtener una cotización específica para un plan de
100 GB.

>> hings Mobile

Things Mobile es un operador global dedicado a dispositivos IoT y M2M, con cobertura
en más de 165 países y más de 350 operadores de roaming. Ofrecen tarifas flexibles
según el consumo, sin costes iniciales ni suscripciones. Por ejemplo, tienen una tarifa
de 0,10 $/MB en los principales países, lo que equivaldría a aproximadamente 10 $ por
GB. Para un plan de 100 GB, esto representaría alrededor de 1.000 $.

>> emnify

emnify ofrece tarjetas SIM IoT con conectividad global y una plataforma de gestión
avanzada. El precio de sus tarjetas SIM comienza desde menos de 2 € para una tarjeta
SIM de grado comercial y menos de 3 € para una tarjeta SIM IoT de grado industrial,
dependiendo del volumen del pedido.

>> Movistar

Internet móvil y 5G+
Navega de forma ilimitada a 2 Mb una vez alcanzados los 20 GB a velocidad 5G+.
Llamadas y SMS
Llamadas ilimitadas a fijos y móviles. SMS a 30 cts.
Roaming: habla y navega fuera de España
25GB para navegar y llamadas ilimitadas en la UE, Reino Unido, Noruega, Islandia o
Liechtenstein. Consulta las tarifas de Roaming de cualquier país.

**Nuestra elección:**

Basándonos en el estudio que hemos realizado, hemos pensado, que la mejor opción
es comprar las **tarjetas SIM a XENET**, ya que es una compañía de la Comunidad
Valenciana que ofrece servicios de telecomunicaciones simples, con la máxima calidad
posible y a un precio netamente inferior al de mercado.

Tienen un plan de Xenet-100 Llamadas ilimitadas, establecimiento incluido y 100 Gb de
datos al mes. Por 5,90€/mes IVA incluído.

Puedes seleccionar qué empresa prefieres para tu cobertura, si Orange con cobertura
5G con Gigas acumulables o Vodafone con solo cobertura 5G. Nosotros elegimos con
Orange ya que tienen una masa más amplia de cobertura.


## Almacenamiento

> 1. Datos de cada cámara :

- Matrícula: 10-20 caracteres (+/- 20 bytes).

- Hora y fecha: +/- 16 caracteres (+/- 16 bytes).

- Ubicación: +/- 50 caracteres (+/- 50 bytes).

- Otros datos (ID de cámara): +/- 50 bytes.

- Tamaño aproximado por evento : 150 bytes/evento.

> 2. Frecuencia de los eventos :

- Supongamos que cada cámara detecta un promedio de 1 vehículo por segundo (en zonas de tráfico muy alto).
    
> 3. Eso equivale a:

- 60 vehículos/minuto.

- 3.600 vehículos/hora.

- 86.400 vehículos/día por cámara.

> 4. Número de cámaras :

- Total: 478 cámaras.

## Cálculo del Almacenamiento Total

> 1. Datos por día por cámara:
  
- Datos del evento: 150 bytes.

- Eventos diarios por cámara: 86,

> 2. Datos del día por cámara :**
  
- 150 bytes × 86.400 vehículos por día = 12,96 MEGABYTE

> 3. Datos por día para 478 cámaras:**

- 12.96MB × 478 = 6,19 MB = 6.2GB/día

> 4. Datos por año para 478 cámaras:**
  
- 6.2GB/día × 365 = 2,263 GB = 2.2TB/año


## Espacio Adicional para Indexación y Redundancia

> 1. Indexación y bases de datos :
  
  - Incrementar el tamaño estimado un 20% por indexación: 2.2TB × 1.2 = 2.64TB /año

> 2. Redundancia (RAID):

  - Usando RAID 6 (20%-30% más de espacio requerido): 2.64TB × 1.3 = 3.43TB /año

Usaremos el RAID 6, debido a que es más seguro que el RAID 5 y tiene mas
disponibilidad de datos. En este caso, para un CPD es más importante la seguridad de
los datos y la disponibilidad que la velocidad de escritura.

Este RAID 6 nos permite una mayor tolerancia a fallos que el RAID 5, permitiendo el
fallo de hasta 2 discos sin perder datos ya que cuenta con doble paridad

## Recomendación de Tamaño del NAS/SAN

> 1. Capacidad por tiempo de retención:
  
  - 1 año de retención : Necesitarás 3,5 TB de capacidad útil.

  - 5 años de retención : Necesitarás 17,5 TB de capacidad útil.

> 2. Considerar crecimiento futuro:

  - Con un margen adicional del 50% para crecimiento, necesitarías:
    
       ○ 1 año de retención : 5 TB.

       ○ 5 años de retención : 26 TB.

> 3. Configuración del almacenamiento:
   
   - Para cubrir 5 años con margen:
     
       ○ Discos : 8 x 8 TB HDD (64 TB brutos, 46 TB útiles en RAID 6).
     
       ○ Esto permitiría cubrir hasta 10 años si fuera necesario.


**1. Coste por GB más eficiente:**
    Los discos de mayor capacidad (como los de 8TB) tienden a ser más económicos por
    GB comparado con discos más pequeños. Es decir, el costo por terabyte suele ser
    menor en discos de 8TB, lo que resulta en un ahorro a largo plazo.

**2. Menor número de discos necesarios:**
    Al elegir discos de mayor capacidad, se necesita un menor número de discos físicos
    para alcanzar la capacidad de almacenamiento requerida. Esto reduce los costes de
    infraestructura (como los racks, cables y otros componentes).

**3. Mejor rendimiento en discos HDD:**
    Aunque los discos más pequeños puedan parecer que proporcionan una recuperación
    más rápida, los discos más grandes pueden ofrecer una velocidad de lectura/escritura
    similar si se usan de manera adecuada en un entorno con configuraciones de RAID
    como RAID 6.

**4. Menos consumo de energía y menos espacio:**
    Tener menos discos físicos también reduce el consumo energético, lo que tiene un
    impacto positivo en los costes operativos y en el uso de espacio en la sala del CPD. Al
    usar discos de mayor capacidad, se optimiza el uso del espacio disponible en los racks.

**5. Escalabilidad:**
    A medida que los requisitos de almacenamiento crecen, los discos de mayor capacidad
    ofrecen mayor flexibilidad para expandir sin necesidad de cambiar toda la
    infraestructura o añadir más racks de servidores.

**6. Resiliencia a largo plazo:**
    RAID 6 proporciona redundancia adicional. En el caso de discos de 8TB, se reduce la
    probabilidad de fallos simultáneos de discos durante el tiempo de vida útil de los discos,
    ya que los discos de mayor capacidad suelen ser más fiables a medida que maduran.
   
**Comparación con discos más pequeños**
    Aunque los discos más pequeños puedan tener ciertas ventajas en términos de
    recuperación de datos, en escenarios de almacenamiento de grandes volúmenes de
    datos, la diferencia en la velocidad de recuperación es generalmente mínima,
    especialmente cuando se utiliza RAID 6 para distribuir los datos y la paridad entre los
    discos.


**1. Cortes o secciones**
    
- **Vistas transversales o longitudinales** :

  - Altura mínima de la sala de servidores: 3 metros para garantizar la ventilación.
         
  - Niveles de acceso restringido en áreas críticas.
       
  - Detalles de instalación de sistemas de aire acondicionado, bandejas portacables, y sistemas contra incendios.

**2. Fachadas**

- **Vista exterior desde distintos ángulos** :
       
   - Diseño minimalista y reforzado.
       
   - Materiales resistentes al clima y al vandalismo.
       
   - Indicación clara de acceso principal y salidas de emergencia.

**3. Detalles constructivos**

- **Información ampliada de áreas críticas** :

   - Sistema de refrigeración redundante (N+1).

   - Acabados de suelos elevados para el paso de cableado.

   - Sistemas contra incendios con gases inertes.
       
   - Sellado de uniones para evitar polvo y humedad.

**4. Planos estructurales**

   - **Columnas y vigas** :
     
       - Diseño para soportar la carga de equipos pesados.

   - **Otros elementos estructurales** :
     
       - Pisos elevados y paredes aisladas térmica y acústicamente.

**5. Instalaciones**
   
- **Eléctricas** :
       
  - Circuitos separados para equipos esenciales y no esenciales.
       
  - Puntos de luz LED distribuidos uniformemente.
    
  - Enchufes industriales y redundancia eléctrica con UPS y generadores.
    
 - **Hidrosanitarias** :

   - Sistemas de drenaje para posibles escapes de agua.

   - Suministro de agua para sistemas de refrigeración.
    
- **Mecánicas o especiales** :
       
   - Aire acondicionado con redundancia.
       
   - Sistemas de ventilación controlada y monitoreo de humedad.


## Especificaciones Técnicas

> 1. Materiales y acabados

   - Suelos: Antiestáticos, elevados y de fácil mantenimiento.
   
   - Paredes: Revestimientos ignífugos y aislantes acústicos.
   
   - Techos: Paneles desmontables para mantenimiento.

---

## Información Gráfica y Simbólica

> 1. Simbología

- Identificación de puertas, ventanas, racks, bandejas, tomas eléctricas, y otros elementos relevantes.

> 2. Norte
    
- Indicación precisa de la orientación para facilitar la ubicación del proyecto.

> 3. Texturas y colores

- Representación gráfica de materiales:

     ○ Concreto: Textura gris moteada.

     ○ Vidrio: Transparente con bordes azules.

     ○ Madera: Textura marrón claro para detalles no críticos.

---

## Ubicación de las cámaras de control de tráfico

### Entradas y salidas de la población

● **Por qué:** Estas zonas suelen ser puntos donde se concentra mucho tráfico,
especialmente en horas punta.

● **Beneficios:** Permiten monitorear el flujo de vehículos, detectar congestión y
supervisar el acceso a la población.

En resumen, las cámaras deben instalarse donde puedan generar el mayor impacto
positivo en la seguridad y eficiencia del tráfico, ubicandolas en las entradas/salidas de
todos los municipios sin excepción.

---

### - Cámaras puestas por la población

Pincha aquí:

[Ver en Google](https://docs.google.com/spreadsheets/d/e/2PACX-1vRe6aq3EfQ-7jng487EhPubw0G6TPfqSOqJHG4IKbeqMuCc52lgcDv3aVPqUi4JTKMmEoisgJaS4PY-/pubhtml?gid=0&single=true)

[Ver en Github](https://github.com/ikerpa04/CPD_Camaras/blob/334e08f519b3217d6a6ce38285651be4522f5799/Contacto%20de%20c%C3%A1maras%20-%20C%C3%A1maras.csv)

### Tabla de Contacto de Cámaras con su respectivo precio

Para el coste aproximado de las cámaras, hemos realizado una tabla en la que
realizamos un análisis de las poblaciones de la Safor, introducimos las cámaras que
necesitamos y los precios de cada cámara. Esta tabla es una aproximación al coste real
del proyecto.

> Columnas de la tabla:

- **Municipios** : Nombres de los municipios a instalar

- **Cámaras** : Número de cámaras que hay en los municipios ya instaladas

- **Cámaras que queremos poner** : Número de cámaras que queremos tener en cada municipio

- **Camaras a poner** : Cámaras que hay que poner restando el número de cámaras ya existentes

- **Precio** : Precio total de las cámaras de cada municipio

| Municipios                   | Camarás   | Cámaras que queremos poner   | Camaras A Poner   | Precio total   |
|:-----------------------------|:----------|:-----------------------------|:------------------|:---------------|
| Gandía                       | 9         | 47                           | 38                | 79.085,60 €    |
| Oliva                        | 16        | 29                           | 13                | 27.055,60 €    |
| Tavernes de la Valldigna     | 3         | 19                           | 16                | 33.299,20 €    |
| Xeraco                       |           | 20                           | 20                | 41.624,00 €    |
| Bellreguart                  |           | 15                           | 15                | 31.218,00 €    |
| Villalonga                   | 2         | 25                           | 23                | 47.867,60 €    |
| La Font d'en Carrós          |           | 14                           | 14                | 29.136,80 €    |
| Daimús                       | 2         | 22                           | 20                | 41.624,00 €    |
| Simat de la Valldigna        |           | 11                           | 11                | 22.893,20 €    |
| Piles                        |           | 19                           | 19                | 39.542,80 €    |
| Miramar                      |           | 16                           | 16                | 33.299,20 €    |
| Real de Gandía               | 30        | 12                           | 0                 | 0,00 €         |
| Almoines                     | 20        | 13                           | 0                 | 0,00 €         |
| Xeresa                       |           | 9                            | 9                 | 18.730,80 €    |
| Beniarjó                     | 11        | 11                           | 0                 | 0,00 €         |
| Palma de Gandía              |           | 6                            | 6                 | 12.487,20 €    |
| Ador                         |           | 8                            | 8                 | 16.649,60 €    |
| Benirredrá                   |           | 12                           | 12                | 24.974,40 €    |
| Benifairó de la Valldigna    |           | 10                           | 10                | 20.812,00 €    |
| Alquería de la Condesa       |           | 15                           | 15                | 31.218,00 €    |
| Barx                         |           | 17                           | 17                | 35.380,40 €    |
| Rafelcofer                   |           | 15                           | 15                | 31.218,00 €    |
| Rótova                       | 26        | 5                            | 5                 | 10.406,00 €    |
| Potríes                      |           | 11                           | 11                | 22.893,20 €    |
| Palmera                      |           | 10                           | 10                | 20.812,00 €    |
| Guardamar de la Safor        |           | 14                           | 14                | 29.136,80 €    |
| Llocnou de Sant Jeroni       |           | 13                           | 13                | 27.055,60 €    |
| Beniflá                      | 30        | 11                           | 0                 | 0,00 €         |
| Alfauir                      | 9         | 3                            | 3                 | 6.243,60 €     |
| Almiserat                    |           | 6                            | 6                 | 12.487,20 €    |
| Castellonet                  |           | 6                            | 6                 | 12.487,20 €    |
| **TOTAL**                    | 158       | 444                          | 365               | **759.638,00 €**   |

#### Precio de cámaras por unidad: **1.720,00 € + IVA (21%) = 2.081,20 €**

## —------------------------------------------------------


## Presupuesto del Material

Para proporcionar una estimación actualizada de los costes de un sistema de
Reconocimiento Automático de Matrícula (ALPR), se ha hecho una aproximación del
mercado actual:

**1. Servidores de procesamiento de imágenes (ALPR):** Para manejar eficientemente
el procesamiento de imágenes, se requieren entre 5 y 10 servidores, dependiendo del
volumen de datos. El coste de los servidores adecuados para esta tarea varían según
las especificaciones, pero generalmente oscila entre 2.000 y 5.000 euros por unidad.
Por lo tanto, la inversión total en servidores estaría entre 10.000 y 50.000 euros.

**2. Almacenamiento en red (NAS/SAN):** Para garantizar redundancia y capacidad
suficiente, se recomiendan de 2 a 4 unidades de almacenamiento en red. Los
dispositivos NAS de calidad, tienen un precio aproximado de 460 euros.
Las soluciones SAN suelen ser más costosas debido a su rendimiento y escalabilidad
superiores. El coste total para el almacenamiento en red puede variar entre 1.000 y
10.000 euros, dependiendo de la capacidad y tecnología seleccionada.

**3. Equipos de red (switches, routers, firewalls):** Para asegurar una conectividad
robusta y segura, se requieren entre 2 y 3 dispositivos de red. El coste de switches y
routers de calidad empresarial suele oscilar entre 500 y 1.500 euros por unidad,
mientras que los firewalls pueden costar entre 1.000 y 3.000 euros. En total, la inversión
en equipos de red estaría entre 2.000 y 9.000 euros.

**4. Racks y accesorios:** Considerando que cada rack estándar tiene una capacidad de
42U y que se recomienda utilizar entre el 70% y 80% de su capacidad para una
ventilación y cableado óptimos, se necesitan aproximadamente 3 racks para alojar todo
el equipo, incluyendo espacio para crecimiento futuro. El coste de un rack estándar
suele estar entre 800 y 1.500 euros. Además, es importante considerar accesorios
como unidades de distribución de energía (PDUs) y sistemas de ventilación, que
pueden sumar entre 500 y 1.000 euros adicionales por rack. En total, la inversión en
racks y accesorios estaría entre 3.900 y 7.500 euros.

> Resumen de costes estimados:

   - Servidores de procesamiento de imágenes (ALPR): 10.000 - 50.000 euros
    
   - Almacenamiento en red (NAS/SAN): 1.000 - 10.000 euros
    
   - Equipos de red (switches, routers, firewalls): 2.000 - 9.000 euros
    
   - Racks y accesorios: 3.900 - 7.500 euros
    
   - Total estimado: 16.900 - 76.500 euros

---

## Evaluación de riesgos

En nuestro CPD, podemos encontrar diversos riesgos a nivel de seguridad informática,
ya sean ciberataques, fugas de datos, etc. A continuación veremos que tipos de riesgos
podemos encontrar para valorar el nivel de seguridad que necesitaremos llevar a cabo.

**_Ciberataques:_**

**- Ataques DDOS:** Estos ataques sobrecargan los servidores y los dejan
inoperativos por un tiempo indeterminado

**- Acceso no autorizado:** El acceso no autorizado aprovechando vulnerabilidades
pueden hacernos perder muchos datos o fallos en el sistema.

**- Ransomware:** Un virus el cual los datos los encripta y nos pedirá un “rescate”,
esto puede ser peligroso al poder robar datos personales de miles de
ciudadanos.

**- Man in the middle:** Entran al CPD sin darnos cuenta e interceptan los datos que
recibimos o enviamos, esto perjudica la seguridad e integridad de los datos.

**- Fugas de datos**

**- Robo de datos:** Al acceder un “hacker” al sistema pueden robar datos e
información muy importante como pueden ser datos de los vehículos,
ciudadanos, etc.

**- Dark web:** Los datos robados pueden ser vendidos o publicados en la Dark
web, es decir el mercado negro

### Protección deficiente:


- **Vulnerabilidades:** Podemos encontrar vulnerabilidades en el sistema debido a
parches de seguridad deficiente o con fallos, también en la falta de
actualizaciones del sistema.

- **Contraseñas vulnerables:** Debido a contraseñas vulnerables o por compartir la
contraseña, pueden acceder quien no debe al sistema y producir fallos.

## RIESGOS OPERATIVOS

También podemos encontrar diferentes riesgos o problemas a nivel operativo, ya sea
hardware o por terceras personas, a continuación veremos los siguientes riesgos.

### Hardware:

● Hardware: Podemos encontrar fallos en dispositivos hardware, ya sean los
discos duros o sistemas de almacenamiento o servidores, causando pérdida de
datos o interrupciones del funcionamiento correcto del CPD.

### Energía:

● Energía: Un riesgo posible muy importante es la energía, es decir, los cortes de
luz o sobretensión. Esto puede afectar al correcto funcionamiento o inclusive se
pueden quemar o dañar los dispositivos

### Humanos:

● Configuración: Debido a errores de configuración pueden haber errores en los
sistemas.

● Eliminación datos: Debido a errores humanos, pueden eliminar datos
importantes o archivos de configuración.

● Mala gestión: Una mala gestión de las actualizaciones o de los mantenimientos
necesarios puede provocar fallas en el CPD.

### Capacidad Insuficiente:

● Capacidad: Debido al crecimiento de datos nuevos cada día, puede aumentar
tanto la capacidad de almacenamiento que no permitirá añadir nuevos datos e
inclusive producir fallos en el sistema.

---

## RIESGOS DE PRIVACIDAD

A continuación, veremos diferentes riesgos o incumplimientos sobre la protección de
datos que debemos llevar a cabo para el correcto funcionamiento del CPD. Esta parte
es muy importante por su delicadeza del tratamiento de datos.

### Protección de datos:

● RGPD: El incumplimiento del Reglamento General de Protección de Datos
puede conllevar sanciones en cuanto al uso y almacenamiento de datos
personales.

### Uso indebido de los datos:

● Datos: Las grabaciones en sitios no autorizados o que apunten a sitios
reservados pueden acarrear sanciones estipuladas por el reglamento.

### Anonimización:

● Anonimización: Si los datos almacenados en el CPD no son anonimizados que
podrían ser vinculados directamente a ciudadanos, puede aumentar el riesgo de
abusos u otros problemas.

---

## RIESGOS FÍSICOS

Aquí veremos diferentes riesgos físicos que pueden afectar en la seguridad del CPD.
Estos riesgos pueden acarrear diferentes problemas con difícil solución a corto plazo.

### No autorizado:


● Intrusos: Pueden acceder al CPD, personal no autorizado o intrusos que
puedan robar o dañar los datos almacenados en el mismo.

● Robo: El robo de dispositivos físicos que contengan datos sensibles pueden
acarrear problemas legales o del correcto funcionamiento del CPD.

### Desastres:


● Desastres: Pueden ocurrir incendios o inundaciones que dañan los servidores o
los sistemas de almacenamiento. También pueden ocurrir diferentes desastres
naturales como terremotos.

### Vandalismo:


● Sabotaje: Los intentos intencionados de dañar equipos o instalaciones del CPD
pueden dañar el funcionamiento correcto del mismo.

---

## RIESGOS TECNOLÓGICOS

Existen también riesgos tecnológicos, estos son riesgos ya sea por obsolescencia de
los equipos, incompatibilidad, etc. Esto puede producir gastos inconvenientes a corto
plazo por no elegir correctamente el equipo necesario.

### Obsolescencia:


● Obsolescencia: El uso de hardware o software antiguo o sin actualizarse,
pueden acarrear problemas. Al usar hardware antiguo puede ocasionar lentitud
en la lectura o escritura de datos. También al usar software antiguo, pueden
tener problemas de seguridad.

### Interoperabilidad:

● Compatibilidad: La falta de compatibilidad de diferentes sistemas de cámaras,
sistemas de almacenamiento, servidores, etc; pueden producir fallos en el CPD
y no funcionar al máximo de rendimiento.

### Reconocimiento:

● Errores: La tasa de errores en la detección de matrículas, generando errores en
la información o información insuficiente.

---

**Planes de contingencia para ciberataques**

### Prevención:


● Firewalls: Al instalar firewalls actualizados y sistemas de prevención de intrusos
prevenimos hackeos o virus que se metan al CPD.

● Pruebas: Deberemos realizar pruebas contra intrusos para verificar la fiabilidad
del sistema instalado evitando hackeos.

● Cifrar: Cifrando los datos que entran y salen del CPD evitamos que alguien
pueda acceder a ellos fácilmente.

### Respuesta:

● CSIRT: Definiendo un equipo de respuesta ante incidentes para actuar
rápidamente en caso de un ciberataque.

● Aislamiento: Aislando los sistemas afectados para contener ciberataques y
evitar la propagación dañando el CPD completo.

● Respaldo: Activando un sistema de respaldo para mantener la operación y así
no perder tiempo en el procesamiento de datos.

● Restauración: Teniendo copias de seguridad actualizadas y verificadas
podemos restaurar datos en caso de pérdida.

● Parches: Aplicando parches a sistemas vulnerables y reforzando los controles
de seguridad.

### Recuperación:

● Investigación: Investigando el origen del ataque y reforzando los sistemas,
podemos prevenir ataques similares.

● Notificar: En caso de fallo en la seguridad, hay que notificar a las autoridades
pertinentes y a los ciudadanos afectados según las leyes de protección de
datos.

---

## CONTINGENCIA PARA FALLOS OPERATIVOS

### Prevención:

● Redundancia: Diseñando una infraestructura redundante para servidores,
almacenamiento y energía para evitar pérdidas en el sistema.

● Balanceadores: Implementando “balanceadores” de carga para evitar que se
saturen los sistemas y así evitar servicios tardíos.

● Mantenimiento: Realizando un mantenimiento adecuado periódicamente el
hardware y el software que usamos, evitamos que se dañen en un momento
inoportuno.

● Actualizaciones: Actualizando los sistemas y reemplazando los equipos
obsoletos antes de que comiencen a fallar.

### Respuesta:

● Respaldo: Activando sistemas de respaldo para cambiar automáticamente a
servidores secundarios en caso de fallos para no perder tiempo.

● Copias: Usando copias de seguridad incrementales diarias evitando la pérdida
de datos.

● Monitoreo: Implementando sistemas de monitoreo continuo que envíen alertas
en tiempo real si surge algún problema en el CPD.

● Diagnóstico: Estableciendo procedimientos de diagnóstico podemos identificar
rápidamente el fallo antes o durante que ocurra.

---

### Recuperación:

● Restauración: En caso de restaurar, deberemos priorizar la recuperación de
servicios esenciales como la comunicación con cámaras críticas e importantes.

● Verificación: Verificando la integridad de los datos restaurados verificamos que
está todo correctamente y no hemos tenido pérdidas de datos.

---

## CONTINGENCIA PARA DESASTRES FÍSICOS

### Prevención:

● Protección: Ubicando el CPD en una zona segura, lejos de inundaciones como
localidades “altas” o evitando áreas sísmicas, evitamos que pueda tener algún
desastre físico.

● Incendios: Contando con un sistema contra incendios podemos evitar un
incendio o en caso de incendio evitar el máximo daño posible.

● Respaldo: Implementando replicaciones de datos en un CPD secundario
ubicado en otra región puede ser caro pero en caso de “mal mayor” puede
ayudarnos mucho.

● Nube: Usando servicios de almacenamiento como la nube como
almacenamiento de respaldo podemos evitar pérdidas de datos.

### Respuesta:

● Reparar: Reparando el CPD afectado y trasladando los datos y servicios desde
el CPD secundario podemos evitar perder mucho tiempo en la restauración o
reparación de nuestro CPD.

● Respaldo: Activando sistemas de respaldo en el CPD secundario para continuar
las operaciones de reparación.

### Recuperación:

● Reparación: Para reparar al completo el CPD, tendremos que trasladar los
datos y servicios desde el CPD secundario.

● Probar: Probando los sistemas antes de restaurar el CPD principal evitaremos
otra vez daños o pérdidas de tiempo de reparación.

---

## Planes de contingencia

### Prevención:

● Políticas: Estableciendo políticas claras de privacidad y protección de datos,
cumpliento con el RGPD y normativas locales, evitaremos problemas legales.

● Anonimizar: Hay que anonimizar todos los datos siempre que sean posibles
porque podremos tener problemas legales con los ciudadanos o autoridades
pertinentes.

● Auditorías: Tendremos que contratar auditorías externas para verificar
constantemente el cumplimiento legal y técnico del CPD.

### Respuesta:

● Informar: Deberemos informar a las autoridades y afectados sobre fugas de
datos en un plazo de 72 horas, según el RGPD.

● Análisis: Debemos realizar un análisis de impacto para entender la magnitud
del incidente.

### Recuperación:

**● Políticas:** Deberemos ajustar las políticas y sistemas para evitar
vulnerabilidades futuras.

**● Capacitación:** Deberemos capacitar nuevamente al personal en mejores
prácticas de privacidad y seguridad.

—---------------------------------------------------------

## PLAN DE FORMACIÓN Y SIMULACROS

### Prevención:

● Capacitación: Debemos entrenar a los empleados en ciberseguridad, gestión
de los datos y protocolos de emergencia, para poder evitar ciberataques o
problemas de seguridad y evitar robo de datos.

● Simulacros: Deberíamos realizar simulaciones de fallos críticos, ciberataques y
desastres naturales para probar la efectividad de los planes de contingencia.

### Respuesta:


● Evaluación: Deberemos evaluar e identificar las áreas de mejora tras cada
simulacro y ajustar los planes según sea necesario.

> **_Interconexión:_**

● **Telemáticamente:** Los clientes tendrán acceso a los servicios del CPD
mediante una aplicación o página web. En dicha página o app habrá 3 tipos de
usuarios, administradores, policía/guardia civil y ayuntamientos.

**○ Administradores:** Los administradores tendrán acceso a todos los datos
según lo requiera para el mantenimiento o modificación del programa o
app.

**○ Policía:** La policía local, nacional y guardia civil tendrán acceso a los
datos completos de las matrículas registradas, para investigaciones.

**○ Ayuntamientos:** Tendrán acceso solamente a datos simples que les
pueda ayudar a mejorar sus municipios. Es decir: número de coches que
pasan por sus localidades y en qué frecuencia horaria, con tal de mejorar
su seguridad y controlar el tráfico.

**● Físicamente:** Los únicos que pueden acceder al CPD físicamente serán los
trabajadores que estén autorizados para realizar el mantenimiento pertinente. En
casos extremos para la revisión de datos, podrá acceder las autoridades
policiales.

> **_Inundaciones_**

La zona escogida para instalar el CPD, que es el **_Polígono Industrial Benieto_** es un
sitio alejado de zona del mar evitando inundaciones por esa parte pero en caso de
riesgo meteorológico, pueden haber lluvias intensas que puedan provocar
inundaciones.

Según el siguiente estudio, observamos que en un periodo de 500 años, la zona de
Gandia, donde se ubica el CPD, sería inundable. A corto plazo no se ve viable una
inundación.


> **_Simulacros_**
Podemos realizar diferentes simulacros como el de incendios o terremotos. Aunque
Gandia no es una zona donde se suelen frecuentar sismos, suelen haber sismos
cercanos que pueden afectar a la infraestructura.

Un simulacro de incendios podremos realizarlos empleando la ayuda especializada del
cuerpo de bomberos. Aun teniendo sistemas contra incendios, es bueno realizar
simulacros para evitar daños en el personal y formar a dicho personal para evitar un mal
mayor.

En un simulacro de terremotos, debemos evitar el pánico y evacuar ordenadamente o
protegerse debajo de una mesa en caso de no poder evacuar. Todos estos
procedimientos estarán escritos en un **plan de evacuación**.

> **_Plan de Evacuación:_**

En el plan de evacuación debe quedar registrado por escrito las rutas de evacuación
más próximas al puesto de trabajo, así como la ubicación de los extintores en caso de
incendio. Todo el plan, debe ser realizado por personal cualificado y firmado por el
responsable de la empresa.

---

**Seguridad Informática**

*Protección contra Amenazas*

** Firewalls:** Implementaremos cortafuegos que controlen el tráfico de la red que
entra y sale, bloqueando así mismo, accesos no autorizados y previniendo
ataques externos, como ataques DDoS que nos in-utilizarían los servicios o
algún malware proveniente de páginas no seguras.

** Detección de intrusos:** Instalaremos sistemas de detección de intrusos que
monitoreen la red en busca de actividades maliciosas o sospechosas. Este
sistema alertará al equipo encargado con la seguridad en caso de un ataque y
así evitando y adelantándose para evitar cualquier mal mayor.

** Políticas de acceso:** Estableceremos políticas de acceso seguras y estrictas
para garantizar que solamente el personal autorizado pueda acceder a los
recursos del CPD. Incluiremos la autenticación de dos factores y asignación de
permisos basados en roles.

** Confidencialidad:** Aseguramos que la información sensible solo será accesible
para aquellos con los permisos adecuados. Esto se realizará mediante cifrado
de datos y gestión de claves de seguridad.

**● Integridad:** Implementaremos controles para asegurar que los datos
almacenados no sean adulterados de manera no autorizada. Incluye la
verificación de integridad de archivos y el uso de firmas digitales.

**● Disponibilidad:** Garantizamos que los sistemas y datos estén disponibles las
24h del día, los 365 días del año; implementando sistemas redundantes y planes
de contingencia.

> **Plan de Recuperación del CPD**

*Copias de seguridad*

**● Completa:** Realizaremos copias de seguridad completas de todos los datos y
sistemas en intervalos regulares. Este tipo de copia incluye todo el contenido
necesario para restaurar el sistema en caso de una falla total.

**● Incremental:** A su vez realizaremos copias de seguridad incrementales que solo
incluyen los cambios realizados en base a las copias completas o incrementales
anteriores. Este tipo de copia ahorra tiempo en caso de recuperación de datos y
ahorra espacio de almacenamiento necesario.

**● Diferencial:** También realizaremos copias de seguridad diferenciales que
incluyen todos los cambios realizados desde la última copia completa, esto
proporciona equilibrio entre el tiempo de restauración y el espacio de
almacenamiento.

**● Local:** Las copias de seguridad se almacenarán de manera local en dispositivos
instalados dentro del CPD con acceso restringido y medidas de protección física
muy estrictas.

**● Nube:** Utilizaremos servicios de almacenamiento en la nube para garantizar la
redundancia y disponibilidad de las copias de seguridad en caso de desastres
locales.

>> Restauración Rápida

**● Procedimiento de restauración:** Estableceremos procedimientos detallados
para la restauración rápida de sistemas y datos. Los procedimientos incluirán
pasos específicos para recuperar sistemas críticos y datos esenciales e
importantes en el menor tiempo posible.

**● Pruebas regulares:** Realizaremos pruebas regulares para garantizar la eficacia
del plan de recuperación. Incluiremos en las pruebas, simulacros de desastres y
ejercicios de restauración para identificar y corregir posibles fallos.
Mecanismos Redundantes

**● Sistemas RAID:** Implementaremos sistemas RAID para asegurar redundancia
de datos y mejorar la disponibilidad del sistema.

**● Sistemas SALS:** Utilizaremos sistemas de almacenamiento conectado en red
(SAN) y sistemas de almacenamiento en red (NAS) que nos garantiza la
redundancia y escalabilidad del almacenamiento.

**● Documentación de protocolos:** Documentamos los protocolos a seguir en
caso de desastres, incluyendo roles y responsabilidades del personal,
procedimientos y planes de contingencia.

---

## SELECCIÓN DE SOFTWARE

> **Sistema Operativo:** Windows Server 2022 Datacenter para funcionalidades avanzadas de
virtualización y gestión de redes.

**Virtualización** : Hyper-V integrado en Windows Server para optimizar los recursos de los
servidores.

**Monitorización:** Software de vigilancia como Milestone XProtect o Avigilon Control Center
para gestionar las 478 cámaras.

**Bases de datos:** Microsoft SQL Server para almacenar registros de acontecimientos y
metadatos de las cámaras.

**Seguridad:** Microsoft Defender for Endpoint y soluciones de firewall como FortiGate para
proteger la infraestructura.

## SELECCIÓN DE HARDWARE

**Servidores:** 3x Servidores Dell PowerEdge R750 con procesadores Intel Xeon Gold
(mínimo 32 núcleos), 256 GB RAM cada uno.
Tarjetas de red 10GbE por alta velocidad en transmisión de datos.

**Almacenamiento:** Cabina de discos NAS/SAN Dell EMC PowerVault ME5 con 1 TB de
almacenamiento HDD.
RAID 6 por redundancia y seguridad de datos.

**Red:** Switchs Cisco Catalyst 9500 con capacidad de 10/40GbE para garantizar un ancho de
banda suficiente.
Firewall Fortinet FortiGate 600E por seguridad perimetral.

**Alimentación y Enfriamiento:** Sistemas de alimentación ininterrumpida (UPS) APC
Smart-UPS de 10 kVA para evitar cortes eléctricos.
Sistemas de climatización de precisión para mantener la temperatura estable en el CPD.

**Justificación de la Selección:** Windows Server 2022 Datacenter permite gestionar
eficientemente máquinas virtuales y servicios necesarios para la plataforma de
videovigilancia.

**CONCLUSIÓN:**

El uso de servidores de alto rendimiento asegura la capacidad de procesar grandes
volúmenes de datos en tiempo real.

El almacenamiento SAN proporciona velocidad, redundancia y capacidad suficiente para
archivar las grabaciones de las cámaras.

La infraestructura de red y seguridad garantiza un entorno estable y protegido contra
ciberamenazas.

Esta configuración garantiza la funcionalidad óptima del CPD para gestionar las 478
cámaras de control de tráfico de manera eficiente y segura.

### 5 Arquitectura del CPD

#### Infraestructura Física

**Ubicación:** El CPD se encuentra en una sala climatizada con control de acceso restringido.

**Sistema de Energía:** Se cuenta con alimentación redundante mediante UPS y un generador de
respaldo.

**Control de Temperatura:** Se utilizan sistemas de climatización con redundancia para garantizar
una temperatura óptima.

**Protección Contra Incendios:** Se ha instalado un sistema de detección y extinción automática de
incendios.

#### Infraestructura de Red

**Topología:** Red segmentada en VLANs para separar los distintos servicios.

**Conectividad:** Se han implementado enlaces redundantes con balanceo de carga.

**Seguridad:** Firewalls perimetrales, IDS/IPS y segmentación de red para minimizar riesgos.

#### Servidores y Almacenamiento

**Servidores:** Se utilizan servidores físicos y virtualizados para optimizar el uso de recursos.

**Almacenamiento:** Se implementó un sistema de almacenamiento SAN con replicación y respaldo
automático.

**Virtualización:** Uso de hipervisores para mejorar la eficiencia y gestión de los recursos.

---

## Diagrama de los Racks

En el diagrama de arriba podemos ver los 3 racks de los que dispondremos.

![11](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104024.png)

1. Los patch panels para la organización del cableado (3 en total)

![12](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104114.png)

2. Un switch por rack para la interconexión de dispositivos (3 en total)
   
![13](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104135.png)

3. Servidores donde llegan las imágenes de las cámaras y donde se procesan (
    donde llegan las imágenes y 2 donde se procesan y se extraen los datos (en este
    caso, solo están en uso 1 de cada, y los otros 2 son para respaldo en caso de caída
    del primer servidor))
   
![14](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104213.png)

4. Servidores NAS de almacenamiento (3 en total (en el primer rack se almacenan los
    datos, en el segundo se hace una copia de los datos del primer NAS y el otro para
    respaldo en caso de fallida en uno de los NAS anteriores))
   
![15](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104226.png)

5. Un router en el segundo rack, de donde saldrán las VLANs (La VLAN10 para los
    administradores, la VLAN20 que tendrán los servidores y la VLAN30 que tendrá el
    personal de seguridad)
   
![16](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104247.png)

6. UPS para en caso de caida de la red eléctrica, los servidores puedan seguir
    funcionando con un raspaldo energético de 12 horas mínimo
   
![17](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/Sprint2/Captura%20de%20pantalla%202025-04-03%20104300.png)

---

### Configuraciones Implementadas

#### Configuración de Red

VLANs separadas para tráfico administrativo, de producción y de seguridad.
Protocolos de enrutamiento dinámico ante fallos.

#### Seguridad y Protección

Firewalls con reglas estrictas de acceso.
Implementación de autenticación multifactor (MFA) para accesos críticos.
Políticas de respaldo y recuperación ante desastres.

### Decisiones Tomadas

#### Redundancia y Alta Disponibilidad

Se optó por una arquitectura redundante en energía, red y almacenamiento para evitar
interrupciones.

#### Seguridad

Se prioriza la seguridad con segmentación de red, control de accesos y monitoreo activo.

#### Escalabilidad

Se eligieron tecnologías que permitan escalabilidad vertical y horizontal para futuras
expansiones.

### Manuales de Usuario y Guías de Administración

#### Manual de Usuario

Acceso al sistema: Instrucciones para iniciar sesión y utilizar los recursos del CPD.
Gestión de datos: Procedimientos para almacenamiento y recuperación de información.
Resolución de problemas básicos: Guía para identificar y solucionar incidencias comunes.

#### Guía de Administración

Mantenimiento del CPD: Procedimientos para actualización de hardware y software.
Gestión de seguridad: Configuración de accesos, auditorías y monitoreo.
Recuperación ante fallos: Planes de contingencia y restauración de servicios.

### Procedimientos de Mantenimiento y Gestión de Recursos

#### Procedimientos de Mantenimiento

Monitoreo del rendimiento: Revisión periódica de logs y métricas de desempeño.
Actualización de software y firmware: Aplicación de parches de seguridad y mejoras.
Limpieza y revisión de hardware: Inspección física para prevenir fallos.

#### Gestión de Recursos

Asignación de capacidad: Distribución eficiente del almacenamiento y cómputo.
Optimización de red: Análisis de tráfico y ajustes para mejorar el rendimiento.
Gestión de accesos: Control de usuarios, permisos y autenticaciones.

#### Plan de Respuesta ante Incidentes

Identificación de problemas: Detección temprana de fallos en los sistemas.
Procedimientos de escalado: Contacto con equipos de soporte en casos críticos.
Documentación y aprendizaje: Registro de incidentes para mejorar procesos futuros.

### Conclusión

La arquitectura y configuraciones del CPD garantizan un entorno seguro, eficiente y escalable,
cumpliendo con los requerimientos operativos y de seguridad necesarios para su correcto
funcionamiento. La documentación realizada asegura la trazabilidad y correcto mantenimiento
del sistema, facilitando la gestión y optimización de recursos.

## Seguridad Informática

### Protección contra Amenazas


● Firewalls: Implementaremos cortafuegos que controlen el tráfico de la red que entra
y sale, bloqueando así mismo, accesos no autorizados y previniendo ataques
externos, como ataques DDoS que nos in-utilizarían los servicios o algún malware
proveniente de páginas no seguras.
● Detección de intrusos: Instalaremos sistemas de detección de intrusos que
monitoreen la red en busca de actividades maliciosas o sospechosas. Este sistema
alertará al equipo encargado con la seguridad en caso de un ataque y así evitando y
adelantándose para evitar cualquier mal mayor.
● Políticas de acceso: Estableceremos políticas de acceso seguras y estrictas para
garantizar que solamente el personal autorizado pueda acceder a los recursos del
CPD. Incluiremos la autenticación de dos factores y asignación de permisos basados
en roles.

### Protección de Recursos del CPD


● Confidencialidad: Aseguramos que la información sensible solo será accesible para
aquellos con los permisos adecuados. Esto se realizará mediante cifrado de datos y
gestión de claves de seguridad.

● Integridad: Implementaremos controles para asegurar que los datos almacenados
no sean adulterados de manera no autorizada. Incluye la verificación de integridad
de archivos y el uso de firmas digitales.

● Disponibilidad: Garantizamos que los sistemas y datos estén disponibles las 24h
del día, los 365 días del año; implementando sistemas redundantes y planes de
contingencia.

## Plan de Recuperación del CPD

### Copias de seguridad

● Completa: Realizaremos copias de seguridad completas de todos los datos y
sistemas en intervalos regulares. Este tipo de copia incluye todo el contenido
necesario para restaurar el sistema en caso de una falla total.

● Incremental: A su vez realizaremos copias de seguridad incrementales que solo
incluyen los cambios realizados en base a las copias completas o incrementales
anteriores. Este tipo de copia ahorra tiempo en caso de recuperación de datos y
ahorra espacio de almacenamiento necesario.

● Diferencial: También realizaremos copias de seguridad diferenciales que incluyen
todos los cambios realizados desde la última copia completa, esto proporciona
equilibrio entre el tiempo de restauración y el espacio de almacenamiento.

### Almacenamiento Seguro de copias

● Local: Las copias de seguridad se almacenarán de manera local en dispositivos
instalados dentro del CPD con acceso restringido y medidas de protección física
muy estrictas.

● Nube: Utilizaremos servicios de almacenamiento en la nube para garantizar la
redundancia y disponibilidad de las copias de seguridad en caso de desastres
locales.

### Restauración Rápida

● Procedimiento de restauración: Estableceremos procedimientos detallados para la
restauración rápida de sistemas y datos. Los procedimientos incluirán pasos
específicos para recuperar sistemas críticos y datos esenciales e importantes en el
menor tiempo posible.

● Pruebas regulares: Realizaremos pruebas regulares para garantizar la eficacia del
plan de recuperación. Incluiremos en las pruebas, simulacros de desastres y
ejercicios de restauración para identificar y corregir posibles fallos.

### Mecanismos Redundantes


● Sistemas RAID: Implementaremos sistemas RAID para asegurar redundancia de
datos y mejorar la disponibilidad del sistema.

● Sistemas SALS: Utilizaremos sistemas de almacenamiento conectado en red (SAN)
y sistemas de almacenamiento en red (NAS) que nos garantiza la redundancia y
escalabilidad del almacenamiento.

● Documentación de protocolos: Documentamos los protocolos a seguir en caso de
desastres, incluyendo roles y responsabilidades del personal, procedimientos y
planes de contingencia.


# Simulación de instalación del CPD

## Configuración del Router

![1](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112344.png)

Para realizar la configuración al router, nos conectaremos mediante un cable ethernet al
ordenador/portatil y accederemos mediante el enlace “http://cudy.net” e introducimos el
usuario y la contraseña iniciales que se encuentran en la parte inferior del router.
Una vez hemos accedido, configuramos la hora local.

![2](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112416.png)

El siguiente paso es darle configuración rápida al punto de acceso que vamos a crear.

![3](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112436.png)

A continuación crearemos la red inalámbrica creando 2 tipos de red, cada una con un ancho
de banda distinto.

![4](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112457.png)

Este es el resultado de la configuración realizada.

![5](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112524.png)

El siguiente paso es ponerle una IP al router con su correspondiente máscara de red.

![6](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112605.png)

Y configurar el DHCP para que nos de ip al conectarnos de manera dinámica

![7](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112617.png)

El escenario simulado es el siguiente:

![8](https://github.com/ikerpa04/CPD_Camaras/blob/8461daebf9bd0dea8d0c15e42a01f41a66c17361/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112628.png)

## Configuración de Proxmox

En esta primera captura se puede ver la pantalla principal al arrancar Proxmox.

![9](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112640.png)

Aquí proxmox comienza a arrancar.

![10](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112656.png)

Aceptamos la licencia para el usuario.

![11](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112711.png)


Aquí nos pregunta en que disco queremos instalarlo (en nuestro caso elegimos el del PC el
cual va a hacer de servidor).

![12](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112725.png)

Configuramos la zona horaria.

![13](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112740.png)

El siguiente paso que nos pide es crear las credenciales para acceder dentro de Proxmox
(nuestras credenciales son: Usuario: root / Email: danibanezmarti@gmail.com / Contraseña:
admin ).

![14](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112755.png)

Configuramos el hostname de la máquina y nos da una IP (nuestro hostname es: CPD
/ IP: 192.168.0.254 / gateway: 192.168.0.1).

![15](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112809.png)

Nos aparece el resumen de la creación de la máquina:

![16](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112822.png)

Comenzamos la instalación del Proxmox en el PC.

![17](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112835.png)

Cuando se haya terminado la instalación se reiniciará la máquina y nos aparecerá el
siguiente menú.

![18](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112852.png)

Por último, cuando elijamos la opción de Proxmox, accedemos donde nos pide el usuario y
la contraseña configurados previamente.

![19](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112910.png)

Una vez conectado desde el Portátil usando este enlace (https://IP:puerto) te pide el usuario
y la contraseña configurada al hacer la instalación del Proxmox, nos conectaremos
mediante esa IP con el portátil para acceder de manera remota.

![20](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112927.png)

Una vez dentro del Proxmox podemos observar el siguiente escenario.

![21](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112942.png)

Cuando ya hemos accedido, creamos una máquina virtual Truenas usando la imagen iso,
desde el Portátil.

![22](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20112957.png)

Iniciamos la instalación del TrueNas una vez puesta la ISO.

Elegimos la opción de instalar.

![23](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113007.png)

En este paso seleccionaremos el disco del PC servidor conectado con el portátil.

![24](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113016.png)

Elegimos el usuario con el que vamos a gestionar el TrueNAS.

![25](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113026.png)

Una vez finalice la instalación, si todo ha salido bien nos aparece un mensaje como el
siguiente:

![26](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113039.png)

Para poder acceder al TrueNAS, de manera remota desde ProxMox, ponemos el enlace en
el navegador que nos aparece más abajo (http://IPTrueNAS / en nuestro caso la IP es
192.168.0.216).

![27](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113051.png)

Entramos dentro del TrueNas mediante la IP que nos proporciona el propio TrueNas y ha
sido nombrada anteriormente.

![28](https://github.com/ikerpa04/CPD_Camaras/blob/6d3804c0797a6ff976e470a9b4e47832f975ad98/Imagenes/sprint3/Captura%20de%20pantalla%202025-04-03%20113108.png)

Cuando nos hayamos logueado, creamos 3 discos virtuales para después poder hacer un
RAID


A continuación descargamos la iso de la Raspberry, la cual pondremos dentro del TrueNas.

***Cuando iniciamos la instalación, la máquina nos da error y no hemos podido seguir con el proceso***




