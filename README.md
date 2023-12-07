# Sistema AquaMonitor

## Introducción

El proyecto AquaMonitor surge como respuesta a la creciente necesidad de implementar soluciones tecnológicas innovadoras para el control y monitoreo eficiente de sistemas de nivel de agua. Con un enfoque integral, AquaMonitor integra hardware y software de vanguardia, incluyendo el PLC LOGO! de Siemens, un servidor local y el servicio en la nube Quantum. Este conjunto de tecnologías colabora para ofrecer un sistema robusto y adaptable que garantiza una gestión eficaz de los recursos hídricos.

### Objetivo del Proyecto:
El principal objetivo de AquaMonitor es proporcionar a los usuarios una herramienta avanzada para la supervisión en tiempo real, control y análisis predictivo de niveles de agua en entornos como cisternas, depósitos o sistemas hidráulicos complejos. Al aprovechar la inteligencia artificial, este proyecto no solo responde a las necesidades actuales, sino que también anticipa eventos futuros, permitiendo una toma de decisiones proactiva.

### Componentes Clave del Proyecto:

1. **LOGO! PLC de Siemens**
Actúa como el cerebro del sistema, gestionando las entradas y salidas analógicas y digitales, así como la interacción con el servidor local y Quantum.

2. **Servidor Local**
Proporciona una interfaz de usuario intuitiva para configuraciones manuales y control remoto. Almacena datos en una base local para análisis retrospectivo.

3. **Quantum**
El servicio en la nube Quantum desempeña un papel crucial, permitiendo la creación de dashboards personalizados, la programación de alertas y el análisis predictivo con inteligencia artificial.
### Beneficios del Proyecto:

**Eficiencia Operativa**: AquaMonitor mejora la eficiencia operativa al proporcionar una visión completa de los niveles de agua, presión y estado del sistema en tiempo real.

**Seguridad y Redundancia**: La inclusión de características como la boya de seguridad y las redundancias en las comunicaciones garantiza un funcionamiento seguro y fiable.

**Toma de Decisiones Informada**: La combinación de datos históricos y análisis predictivo permite a los usuarios tomar decisiones informadas para la gestión óptima de los recursos hídricos.

## Componentes del Sistema

### 1. Sensor de Presión

El sensor de presión de agua implementado en este sistema opera bajo el principio de medición de la presión ejercida por el nivel del agua. Diseñado para funcionar en un rango de profundidad de 0 a 5 metros, este transductor convierte la presión hidrostática generada por la columna de agua en una señal eléctrica de corriente proporcional.

El sensor utiliza la escala de corriente de 4 a 20 mA para representar el rango completo de mediciones. En condiciones normales, cuando el nivel de agua es mínimo (0 metros), el sensor emite una corriente de 4 mA. A medida que el nivel de agua aumenta, la presión hidrostática también lo hace, lo que resulta en un incremento lineal de la corriente de salida. En su punto máximo (5 metros), la corriente de salida alcanza los 20 mA.

Esta variación de corriente proporciona una señal continua que refleja con precisión el nivel actual de agua en la ubicación del sensor. Esta señal de corriente es transmitida al PLC (Controlador Lógico Programable), donde es interpretada y procesada para obtener datos precisos sobre el nivel de agua.

El PLC, a través de su lógica programada, puede tomar decisiones automáticas basadas en las lecturas del sensor, como activar alarmas, controlar bombas o realizar ajustes en el sistema según los requerimientos específicos. Esta integración del sensor de presión de agua con el PLC garantiza una supervisión efectiva y un control adaptativo del nivel de agua, contribuyendo a la eficiencia y seguridad del sistema en su conjunto.

### 2. Logo PLC

El PLC Siemens LOGO! 230RC es la piedra angular de nuestro sistema de control, desempeñando un papel crucial en la gestión avanzada del suministro de agua. Operando en conjunto con el sistema de presión constante y las bombas de agua, el PLC garantiza un control preciso y una respuesta adaptativa basada en las condiciones del nivel de agua.

La incorporación del sistema de nivel de agua como mejora adicional demuestra nuestro compromiso con la seguridad y la eficiencia operativa. El PLC, con su capacidad de lógica programable, monitoriza de manera continua las lecturas del sensor de presión de agua. Cuando se detecta un nivel bajo de agua, el PLC toma decisiones automatizadas para prevenir el funcionamiento de las bombas, evitando posibles daños a los equipos y garantizando un suministro de agua fiable.

Esta función de prevención y control adaptativo no solo protege las bombas de agua de posibles daños, sino que también contribuye a la eficiencia energética y al mantenimiento a largo plazo del sistema. La capacidad del PLC para analizar y responder dinámicamente a las condiciones del nivel de agua mejora significativamente la gestión integral del suministro de agua, asegurando un rendimiento óptimo y una prolongada vida útil de los componentes del sistema.

En resumen, el PLC Siemens LOGO! 230RC, en combinación con el sistema de nivel de agua, representa una solución integral que aporta seguridad, eficiencia y confiabilidad al control del suministro de agua, garantizando un funcionamiento fluido y la protección de los equipos asociados.

La pantalla HMI (Interfaz Hombre-Máquina) es una parte integral de nuestro sistema de control, sirviendo como un dispositivo multifuncional que ofrece visualización, interactividad y control. Como indicador principal, la HMI proporciona información en tiempo real sobre diversos aspectos críticos del sistema, permitiendo una supervisión efectiva y rápida toma de decisiones.

### 3. Funciones clave de la Pantalla HMI

1. **Visualización de Niveles de Agua y Presión:**
   La HMI muestra de manera clara y comprensible los niveles de agua actuales y la presión en el sistema de agua potable. Esto facilita una evaluación rápida del estado del sistema y permite una respuesta inmediata a cualquier variación.

2. **Estado del Equipo y Posibles Errores:**
   Proporciona información detallada sobre el funcionamiento del equipo, así como alertas y mensajes de error en caso de cualquier anomalía. Esto facilita la identificación y resolución eficiente de problemas, contribuyendo a la confiabilidad del sistema.

3. **Control Manual:**
   La HMI actúa como un dispositivo de control manual, permitiendo a los operadores realizar ajustes y modificaciones directas en el sistema según sea necesario. Esto añade flexibilidad y capacidad de respuesta a las operaciones cotidianas.

4. **Reinicio del Sistema:**
   Ofrece la capacidad de reiniciar el sistema de manera segura y controlada. Esto es esencial para restablecer el funcionamiento normal después de ciertos eventos o mantenimientos programados.

5. **Interfaz con el PLC:**
   Como dispositivo de entrada para el PLC, la HMI facilita la comunicación bidireccional entre los operadores y el sistema de control. Los comandos introducidos a través de la HMI son interpretados por el PLC, permitiendo una ejecución precisa de las acciones necesarias.

La Pantalla HMI representa una herramienta valiosa para la gestión y supervisión del sistema en tiempo real. Su diseño intuitivo y funciones diversificadas contribuyen a la eficiencia operativa y a la capacidad de respuesta del personal encargado del control del sistema.

### 4. Servidor Local

El servidor local representa la columna vertebral de nuestro sistema de monitoreo y control, desempeñando múltiples funciones clave para garantizar la eficiencia operativa y la toma de decisiones informada. Este dispositivo integral está diseñado para ejecutar un programa especializado que actúa como lector y operador del PLC, permitiendo la extracción de datos cruciales mediante el protocolo Modbus a través de la red local LAN.

**Funciones Clave del Servidor Local:**

1. **Interfaz con el PLC y Extracción de Datos:**
   El servidor local actúa como intermediario entre el PLC y el sistema en su conjunto. A través del protocolo Modbus, extrae datos relevantes, como niveles de agua, presión del sistema, estado de funcionamiento y otros parámetros esenciales para el monitoreo y control.

2. **Aplicación Web para Visualización:**
   Presenta los datos de manera clara y accesible a través de una aplicación web. Esta interfaz permite a los usuarios visualizar en tiempo real información crítica, como el nivel de agua, la presión y el estado del sistema, desde cualquier dispositivo con conexión a la red.

3. **Almacenamiento en Base de Datos:**
   El servidor local integra una base de datos para almacenar históricamente datos relevantes, como mediciones de presión, niveles de agua y alertas generadas. Esto facilita el análisis retrospectivo y la identificación de patrones a lo largo del tiempo.

4. **Comunicación con Servicios en la Nube:**
   Facilita la comunicación bidireccional con servicios en la nube para compartir datos y recibir actualizaciones. Esto permite una mayor accesibilidad a la información y la posibilidad de aprovechar recursos adicionales en la nube.

5. **Alertas y Comunicación Externa:**
   Incorpora la capacidad de enviar alertas a los administradores mediante diversas formas de comunicación, como correo electrónico, mensajes SMS u otras plataformas. La integración con aplicaciones externas como Quantum asegura una comunicación efectiva y oportuna ante eventos críticos.

El servidor local se posiciona como un nodo central, unificando la información del PLC y facilitando su acceso y gestión. Su papel es esencial para la toma de decisiones informadas y la optimización continua del sistema de control de nivel de agua.

### 5. Quantum

Quantum, nuestro servicio central de comunicación y gestión en la nube, desempeña un papel vital en la optimización y supervisión avanzada de nuestro sistema de control de nivel de agua. Esta plataforma no solo facilita la transferencia segura de datos desde el PLC y el servidor local mediante una conexión VPN, sino que también ofrece características avanzadas para análisis, visualización y toma de decisiones proactivas.

**Funciones Clave de Quantum:**

1. **Comunicación y Transferencia Segura de Datos:**
   Quantum establece una conexión segura mediante VPN con el servidor local, asegurando la transferencia eficiente y protegida de datos desde el sistema local hasta la nube. Esto garantiza la confiabilidad y seguridad de la información transmitida.

2. **Creación de Dashboards Personalizados:**
   Quantum proporciona herramientas avanzadas para la creación de dashboards personalizados, permitiendo una visualización detallada y en tiempo real de los datos del sistema. Los administradores pueden personalizar la interfaz según sus necesidades específicas para una supervisión efectiva.

3. **Programación de Alertas Configurables:**
   Permite la configuración de alertas personalizadas basadas en umbrales específicos y condiciones críticas. La flexibilidad de Quantum facilita la programación de alertas automáticas, asegurando que los administradores sean notificados de inmediato ante eventos importantes.

4. **Graficación Avanzada con Canvas:**
   Facilita la creación de gráficos y visualizaciones detalladas mediante herramientas avanzadas de graficación con canvas. Esto mejora la interpretación de datos y proporciona una comprensión más profunda de los patrones operativos del sistema.

5. **Medios de Comunicación Multicanal:**
   Quantum integra medios de comunicación variados, desde notificaciones por correo electrónico y mensajes SMS hasta integraciones con aplicaciones externas como Quantum. Esto garantiza que los administradores reciban alertas y actualizaciones en tiempo real, facilitando una respuesta inmediata y eficaz.

6. **Monitoreo Predictivo con Inteligencia Artificial (IA):**
   Quantum incorpora capacidades de monitoreo predictivo mediante IA. Analiza los patrones históricos y actuales para prever el comportamiento futuro del sistema. Las alertas anticipadas permiten a los administradores tomar medidas preventivas antes de que ocurran situaciones críticas.

La incorporación de funciones avanzadas en Quantum no solo mejora la eficiencia operativa sino que también potencia la capacidad del sistema para adaptarse y prever eventos futuros, promoviendo una gestión proactiva y una toma de decisiones informada.

## Funcionamiento del Sistema

1. **Medición de Presión y Conversión a Litros:**
   - El transductor de presión mide la presión del agua y convierte esta información en una señal de corriente (4-20 mA).
   - La señal es recibida por la entrada analógica del Logo PLC.
   - El transductor asociado a este sistema opera a una tensión de 12 voltios de corriente continua (12 VDC). Es fundamental garantizar la alimentación eléctrica con una fuente de 12 VDC para un funcionamiento óptimo del transductor y la obtención de mediciones precisas. Por favor, asegúrese de cumplir con este requisito de alimentación para garantizar el rendimiento adecuado del sistema.

  
2. **Cálculo del Nivel de Agua, Litros y PSI a partir de un Sensor de Presión**
```plaintext
Variables
Estas seran la variables a usar:

- I_{sensor} es la corriente medida por el sensor en mA.
- I_{min} es la corriente correspondiente al nivel de agua mínimo (4 mA).
- I_{max} es la corriente correspondiente al nivel de agua máximo (20 mA).
- Profundidad_{cisterna} es la profundidad máxima de la cisterna en metros.
- Ancho_{cisterna} es el ancho de la cisterna en metros.
- Largo_{cisterna} es el largo de la cisterna en metros.

## Fórmula para el Nivel de Agua
La fórmula siguiente se utiliza para calcular el nivel de agua en porcentaje:
Nivel (%) = ((I_{sensor} - I_{min}) / I_{max} -  I_{min})) * 100

### Cálculo del Nivel en Porcentaje
Ejemplos:
100% = ((20 - 4) / (20 - 4)) * 100
75% = ((16 - 4) / (20 - 4)) * 100
50% = ((12 - 4) / (20 - 4)) * 100
25% = ((8 - 4) / (20 - 4)) * 100

## Cálculo del Volumen de Agua en Litros
Forma en base al porcentaje de la anterior formula:
Volumen (m3) = Largo_{cisterna} x Ancho_{cisterna} x Profundidad_{cisterna}
Volumen (litros cisterna) = Volumen (m3) * Nivel (%) x 1000

120 m3 = 8 m x 5 m x 3 m 
120000 L = 120 * 100 % * 1000

Nota: para poder tener una medida en en litros debemos trasnformar de m3 a litros que es litros = m3 x 1000
```
3. **Cálculo del Nivel de Agua, Litros y PSI a partir de un Sensor de Presión**

**Funcionamiento del Sistema del PLC LOGO! con Mediciones:**

## Funcionamiento del PLC:

1. **Entradas Analógicas y Digitales:**
   - *Sensores de Presión de Agua:* Las entradas analógicas del PLC reciben las señales del sensor de presión de agua, traduciendo la presión en niveles de voltaje proporcionales para su procesamiento.
   - *Boya de Seguridad (Entrada Digital):* La boya de seguridad, configurada como una entrada digital, actúa como un dispositivo de redundancia, detectando niveles bajos de agua como medida de precaución.

2. **Entradas y Salidas de Red:**
   - *Interacción con el Servidor Local (Entradas de Red):* El PLC recibe comandos y configuraciones desde el servidor local a través de entradas de red, permitiendo funciones como el control manual, el reinicio del sistema y otras operaciones específicas.
   - *Transmisión de Datos al Servidor Local (Salidas de Red):* Las salidas de red del PLC transmiten datos cruciales al servidor local, como la medición de la presión del nivel de agua, la presión del sistema y el estado de las bombas.

3. **Salidas Analógicas y Digitales:**
   - *Salida Analógica para la Medición de Presión:* El PLC emite una señal analógica que representa la medición de presión del nivel de agua. Esta información es crucial para el monitoreo en tiempo real y la visualización en el servidor local y Quantum.
   - *Salidas Digitales para el Control de las Bombas:* Las salidas digitales controlan el encendido y apagado de las bombas en función de las lecturas del sensor de presión y las decisiones programadas en el PLC.

4. **Almacenamiento de Datos:**
   - *Base de Datos en el Servidor Local:* Todos los datos leídos por el PLC y transmitidos desde el servidor local se almacenan en una base de datos local. Esto facilita el análisis retrospectivo y la gestión eficiente de la información histórica.

5. **Comunicación con Quantum:**
   - *Envío de Datos a Quantum:* Quantum recibe datos relevantes del PLC, incluidas las mediciones actuales y los estados de las bombas. Esta información se utiliza para la generación de alertas y el análisis predictivo mediante la inteligencia artificial.

6. **Interacción con el Usuario:**
   - *Configuración desde la Interfaz del Servidor Local:* Los usuarios pueden interactuar con la interfaz del servidor local para realizar configuraciones específicas, como el funcionamiento manual, el reinicio del sistema, etc. Estas configuraciones se transmiten al PLC para implementar las acciones correspondientes.

## Flujo de Datos:
1. Los sensores envían mediciones al PLC.
2. El PLC procesa las señales y toma decisiones basadas en la lógica programada.
3. Los comandos del servidor local son recibidos por el PLC, afectando el funcionamiento del sistema.
4. Los datos relevantes se transmiten al servidor local y Quantum.
5. Quantum utiliza datos históricos y actuales para análisis predictivo y generación de alertas.
6. La información clave se almacena en la base de datos local para referencias futuras.

## Redundacias

Con el objetivo de fortalecer la confiabilidad del sistema y asegurar un monitoreo continuo del nivel de agua, hemos incorporado un sensor tipo boya como una medida de redundancia. Este sensor adicional actúa como salvaguarda ante posibles fallos, deterioro o transmisión incorrecta de datos por parte del sensor principal.

El sensor tipo boya entra en funcionamiento exclusivamente cuando el nivel de agua desciende a un umbral predefinido, activando los disparadores correspondientes para niveles bajos de agua. En este escenario, el sistema puede tomar acciones preventivas o alertar a los responsables para abordar la situación de manera proactiva.

La inclusión de este sensor tipo boya no solo garantiza un monitoreo ininterrumpido del nivel de agua, sino que también ofrece una capa adicional de seguridad y redundancia, contribuyendo a la fiabilidad y disponibilidad continua de información crítica para la gestión del agua.

Es crucial destacar que este enfoque busca maximizar la robustez del sistema, asegurando que factores críticos como el suministro de agua estén siempre bajo vigilancia, incluso en situaciones donde el sensor principal pueda experimentar dificultades. Esta estrategia de redundancia refuerza la integridad y eficiencia del sistema en su conjunto.

## Conclusiones

1. **Integración y Coherencia del Sistema:**
   - La combinación del PLC (LOGO! de Siemens), el servidor local y el servicio Quantum proporciona una solución integral para el control y monitoreo del sistema de nivel de agua.
  
2. **Redundancia y Seguridad:**
   - La inclusión de la boya de seguridad como una entrada digital de redundancia mejora la seguridad del sistema, garantizando que, en caso de fallas en el sensor principal, se tomen medidas preventivas.

3. **Interfaz de Usuario Intuitiva:**
   - La interfaz del servidor local brinda a los usuarios la capacidad de interactuar fácilmente con el sistema, permitiendo configuraciones manuales, reinicios y otras operaciones esenciales.

4. **Comunicación Eficiente:**
   - La comunicación segura entre el PLC y el servidor local a través de una conexión VPN garantiza la transmisión confiable de datos. La arquitectura de red permite al usuario controlar y configurar el sistema de manera remota.

5. **Almacenamiento y Gestión de Datos:**
   - La base de datos en el servidor local proporciona un almacenamiento centralizado de datos históricos, facilitando el análisis retrospectivo y la toma de decisiones informada.

6. **Potencial Predictivo con IA:**
   - La incorporación de Quantum permite un análisis avanzado de datos, incluida la implementación de inteligencia artificial para el monitoreo predictivo. Esto mejora la capacidad del sistema para anticipar eventos y tomar medidas proactivas.

7. **Notificaciones y Alertas Eficientes:**
   - La integración con Quantum posibilita la programación de alertas personalizadas, así como el uso de diversos canales de comunicación para informar a los administradores. Esto garantiza una respuesta rápida ante cualquier eventualidad.

8. **Visualización Clara y Accesible:**
   - La creación de dashboards personalizados en Quantum proporciona una visualización clara y accesible de los datos en tiempo real, mejorando la supervisión y facilitando la toma de decisiones.

En resumen, la combinación de tecnologías proporciona un sistema robusto y adaptable que no solo responde a las necesidades actuales, sino que también incorpora características avanzadas para enfrentar desafíos futuros. La arquitectura modular y la capacidad de análisis predictivo demuestran un enfoque progresivo hacia la gestión eficiente del sistema de control de nivel de agua.
