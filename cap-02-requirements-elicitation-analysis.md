# Requirements Elicitations & Analysis

Esta etapa es fundamental en el desarrollo de nuestro sistema, ya que permite identificar, comprender y definir las necesidades reales de los usuarios y del negocio. En esta fase, se recopila información a partir de diferentes fuentes, como entrevistas, observación y análisis del contexto, con el objetivo de obtener una visión clara de los problemas existentes y las funcionalidades que la solución debe cubrir.

## **2.1. Competidores**

### **Competidor 1: IoT Smart Gas Platform**

**IoT Smart Gas** es una solución tecnológica basada en IoT que permite monitorear balones y tanques de gas en tiempo real mediante sensores conectados. Sus funcionalidades incluyen la medición de niveles de gas, presión y consumo, así como la visualización de datos a través de plataformas web o móviles, facilitando la gestión de inventario y la planificación de reposiciones. Es un competidor directo frente a nuestra startup, ya que también ofrece monitoreo y seguimiento en tiempo real; sin embargo, su enfoque está centrado principalmente en el consumo y control del suministro de gas, y no abarca de manera integral aspectos como la seguridad en almacenes mediante sensores ambientales, la gestión de cobranzas o el control completo de la distribución, que sí forman parte de la propuesta de Regula.

### **Competidor 2: GasSense (innovateIT – Smart LPG Monitoring)**

**GasSense** permite monitorear balones de gas en tiempo real mediante sensores inteligentes. Sus funcionalidades incluyen la medición del nivel de gas, generación de alertas cuando el contenido es bajo, análisis del consumo y visualización de datos a través de una plataforma web o aplicación móvil. Está orientado tanto a usuarios domésticos como a entornos industriales, buscando optimizar el uso y disponibilidad del gas. Es un competidor directo frente a nuestra startup, ya que también integra monitoreo en tiempo real y análisis de datos; sin embargo, su alcance se limita principalmente al seguimiento del estado del gas a nivel de consumo, sin integrar una solución enfocada en la operación del negocio, como la coordinación de distribución, el registro de movimientos de inventario o la administración financiera de los clientes.

### **Competidor 3: .one Meter (plataforma LPG de Aton)**

**.one Meter** es una solución empresarial orientada al sector energético que permite supervisar grandes volúmenes de balones y tanques de gas mediante tecnologías como IoT y RFID. Su sistema centraliza información en la nube y ofrece funcionalidades como trazabilidad de activos, geolocalización de unidades de transporte, control de operaciones y análisis de datos a nivel corporativo. Está diseñada principalmente para compañías de gran escala que requieren visibilidad completa de sus procesos logísticos y operativos. En relación con nuestra startup, representa un competidor directo en el ámbito del control y seguimiento de activos; sin embargo, su enfoque está dirigido a organizaciones más grandes y complejas, con soluciones menos accesibles para distribuidores pequeños o medianos.

| **Competitive Analysis Landscape** |     |
| ---- | ----- |
|  ¿Por qué llevar a cabo este análisis? |   Este análisis se realiza para comprender a fondo los problemas del sector, identificar las necesidades reales de los usuarios y definir requisitos claros que permitan desarrollar una solución efectiva. En el caso de Regula, permite asegurar que la aplicación web responda a problemas críticos como el control de inventario, la seguridad y la gestión de cobranzas. |

## Perfil

|                       | **Regula (Startup)** | Competidor 1 – **IoT Smart Gas Platform** <br> <img src="../../report/assets/images/smart-gas.png">| Competidor 2 – **GasSense** <br> <img src="../../report/assets/images/gas-sense.png"> | Competidor 3 – **.one Meter** <br> <img src="../../report/assets/images/.one-meter.png"> |
|-----------------------|----------------------------------|---------------------------------------------|--------------------------------|----------------------------------------|
| **Perfil / Overview** | Plataforma web orientada a empresas envasadoras y distribuidores de balones de gas que permite gestionar inventario, distribución y cobranzas, además de mejorar la seguridad mediante monitoreo ambiental con sensores de gas en almacenes. | Plataforma basada en IoT que permite monitorear balones y tanques de gas en tiempo real, enfocada en el seguimiento del consumo, niveles de gas y optimización del abastecimiento. | Sistema inteligente que utiliza sensores para supervisar el nivel de gas y generar alertas de consumo, orientado a mejorar la disponibilidad del recurso en hogares e industrias mediante análisis de datos. | Plataforma empresarial que permite el seguimiento y control de activos de gas a gran escala mediante tecnologías como IoT y RFID, ofreciendo trazabilidad, geolocalización y análisis centralizado de operaciones. |
| **Ventaja competitiva / Valor** | Ofrece una solución integral que combina gestión operativa con seguridad mediante monitoreo ambiental de gas en almacenes, todo centralizado en una aplicación web accesible y fácil de usar para empresas y distribuidores. | Su ventaja radica en el monitoreo en tiempo real del consumo y nivel de gas mediante sensores IoT, lo que permite optimizar el abastecimiento y evitar interrupciones en el suministro. | Ofrece como valor principal la predicción y control del consumo de gas a través de análisis de datos, facilitando alertas tempranas y una mejor planificación del uso del recurso. | Su ventaja competitiva es la capacidad de gestionar y supervisar grandes volúmenes de activos de gas con trazabilidad y geolocalización en tiempo real, orientado a operaciones de gran escala. |

## Perfil de Marketing


|                       | **Regula (Startup)** | Competidor 1 – **IoT Smart Gas Platform** <br> <img src="../../report/assets/images/smart-gas.png">| Competidor 2 – **GasSense** <br> <img src="../../report/assets/images/gas-sense.png"> | Competidor 3 – **.one Meter** <br> <img src="../../report/assets/images/.one-meter.png"> |
|-----------------------|----------------------------------|---------------------------------------------|--------------------------------|----------------------------------------|
| **Mercado objetivo** | Empresas envasadoras de gas y distribuidores de balones de GLP, especialmente pequeñas y medianas empresas que necesitan mejorar su control de inventario, distribución, cobranzas y seguridad operativa. | Empresas de gas, industrias y organizaciones que buscan optimizar el abastecimiento mediante monitoreo del consumo y niveles de gas en tanques o cilindros. | Usuarios domésticos, comercios e industrias que desean controlar el consumo de gas y recibir alertas para una mejor gestión del suministro. | Grandes corporaciones del sector energético y empresas de distribución de gas que operan a gran escala y requieren soluciones avanzadas para la gestión y seguimiento de activos. |
| **Estrategias de marketing** | Estrategia enfocada en un modelo B2B, con captación directa de clientes mediante demostraciones del sistema, visitas a distribuidores y alianzas con empresas del sector gas. Se complementa con presencia digital (redes, landing page) y un enfoque en mostrar ahorro de costos, control operativo y mejora en seguridad como propuesta de valor. | Estrategia basada en marketing tecnológico, destacando innovación IoT, automatización y eficiencia operativa. Utiliza canales digitales, demostraciones del producto y contenido técnico para atraer empresas interesadas en la transformación digital. | Estrategia mixta B2C y B2B, enfocada en resaltar comodidad, control del consumo y ahorro. Utiliza marketing digital, aplicaciones móviles y comunicación directa de beneficios al usuario final. | Estrategia corporativa dirigida a grandes empresas, basada en soluciones empresariales a medida, participación en ferias del sector energético y posicionamiento como proveedor tecnológico avanzado a nivel internacional. |

## Perfil de producto

|                       | **Regula (Startup)** | Competidor 1 – **IoT Smart Gas Platform** <br> <img src="../../report/assets/images/smart-gas.png">| Competidor 2 – **GasSense** <br> <img src="../../report/assets/images/gas-sense.png"> | Competidor 3 – **.one Meter** <br> <img src="../../report/assets/images/.one-meter.png"> |
|-----------------------|----------------------------------|---------------------------------------------|--------------------------------|----------------------------------------|
| **Productos & Servicios** | Aplicación web para gestión de inventario, distribución y cobranzas, junto con monitoreo ambiental de gas en almacenes mediante sensores y alertas en tiempo real. | Plataforma IoT con sensores para monitoreo de niveles, consumo y estado del gas, con visualización de datos en tiempo real. | Sistema de monitoreo de gas con sensores inteligentes, alertas de nivel bajo y análisis de consumo accesible desde app o web. | Plataforma empresarial para gestión de activos de gas con IoT y RFID, incluyendo trazabilidad, geolocalización y análisis de datos. |
| **Precios & Costos** | Regula utiliza un modelo SaaS basado en suscripción mensual, donde los clientes pagan por el acceso a la plataforma según su tamaño o uso. Adicionalmente, puede generar ingresos por servicios complementarios como implementación inicial y venta o integración de sensores de gas. | Opera con un modelo híbrido que combina la venta de dispositivos IoT (sensores) con suscripciones a una plataforma digital para monitoreo y gestión de datos. | Su modelo de negocio se basa en la comercialización de sensores inteligentes junto con el acceso a su sistema de monitoreo mediante suscripción, ofreciendo valor a través del análisis del consumo. | Funciona bajo un modelo empresarial que combina licencias de software, servicios personalizados e integración tecnológica, generalmente mediante contratos y suscripciones dirigidas a grandes compañías. |
| **Canales de distribución (Web y/o Móvil)** | Principalmente a través de una aplicación web, accesible desde cualquier dispositivo con internet, con posibilidad de integración futura con versión móvil. | Acceso mediante plataforma web y aplicación móvil, complementado con dispositivos físicos conectados (sensores IoT). | Uso de aplicación móvil y plataforma web para monitoreo y visualización de datos en tiempo real. | Distribución a través de plataforma web empresarial en la nube, con acceso remoto para gestión y monitoreo de operaciones. |


## Análisis SWOT

*Análisis FODA*

|                       | **Regula (Startup)** | Competidor 1 – **IoT Smart Gas Platform** <br> <img src="../../report/assets/images/smart-gas.png">| Competidor 2 – **GasSense** <br> <img src="../../report/assets/images/gas-sense.png"> | Competidor 3 – **.one Meter** <br> <img src="../../report/assets/images/.one-meter.png"> |
|-----------------------|----------------------------------|---------------------------------------------|--------------------------------|----------------------------------------|
| **Fortalezas** | Solución integral que combina gestión operativa y seguridad, fácil de usar, accesible para PYMES y enfocada en necesidades reales del sector. | Monitoreo en tiempo real mediante IoT, automatización de datos y optimización del abastecimiento de gas. | Capacidad de análisis y predicción de consumo, con alertas inteligentes que mejoran la gestión del uso de gas. | Alta escalabilidad, trazabilidad de activos y gestión centralizada para operaciones de gran volumen. |
| **Debilidades** | Marca nueva en el mercado, menor experiencia en el sector y dependencia de adopción tecnológica por parte de usuarios tradicionales. | Dependencia de hardware (sensores) que eleva costos iniciales y enfoque limitado al monitoreo del gas, sin cubrir procesos del negocio. | Enfoque centrado en consumo y no en la gestión operativa completa, con menor utilidad para distribuidores o empresas logísticas. | Alto costo y complejidad de implementación, orientado a grandes empresas, lo que dificulta su adopción en PYMES. |
| **Oportunidades** | Creciente necesidad de digitalización en el sector, baja adopción tecnológica en distribuidores y demanda por mejorar seguridad y control operativo. | Creciente necesidad de digitalización en el sector, baja adopción tecnológica en distribuidores y demanda por mejorar seguridad y control operativo. | Mayor interés en eficiencia energética y control de consumo tanto en hogares como en industrias. | Crecimiento de grandes empresas energéticas que requieren soluciones avanzadas para optimizar sus operaciones a gran escala. |
| **Amenazas** | Competencia de soluciones tecnológicas ya posicionadas, resistencia al cambio por parte de usuarios tradicionales y posibles limitaciones en adopción por presupuesto. | Alta competencia en el mercado IoT y barreras de adopción por costos iniciales o complejidad técnica. | Saturación de soluciones similares enfocadas en consumo y dificultad para diferenciarse en el mercado. | Dependencia de grandes clientes y competencia de soluciones más accesibles que pueden captar segmentos más pequeños del mercado. |


## Estrategias y tácticas preliminares frente a la competencia

Para definir las estrategias y tácticas preliminares de Regula frente a la competencia, se toma como base el análisis competitivo realizado, considerando las fortalezas y debilidades de cada competidor, así como las oportunidades del mercado y las amenazas presentes en el sector de distribución y monitoreo de gas GLP.

---

## Estrategias para afrontar las fortalezas de los competidores

### Frente a IoT Smart Gas Platform

La principal fortaleza de IoT Smart Gas Platform es el monitoreo en tiempo real mediante sensores IoT y la optimización del abastecimiento de gas. Frente a ello, Regula aplica una estrategia de diferenciación funcional integral.

Mientras IoT Smart Gas se enfoca principalmente en el consumo y suministro de gas, Regula incorpora además gestión de inventario, distribución, cobranzas y monitoreo ambiental de seguridad en almacenes dentro de una sola plataforma.

**Táctica:**  
Posicionar a Regula como una solución completa para empresas distribuidoras y envasadoras, resaltando que no solo monitorea el gas, sino que también optimiza toda la operación del negocio.

### Frente a GasSense

GasSense tiene como principal fortaleza el análisis predictivo del consumo y las alertas inteligentes para usuarios domésticos e industriales. Frente a ello, Regula aplica una estrategia de especialización orientada al sector empresarial B2B.

GasSense está enfocado principalmente en el control del consumo de gas, mientras que Regula cubre necesidades operativas críticas de distribuidores y empresas envasadoras.

**Táctica:**  
Destacar que la plataforma fue diseñada específicamente para resolver problemas de logística, control de inventario, cobranzas y seguridad operativa, aspectos que GasSense no aborda de forma integral.

### Frente a .one Meter

La principal ventaja competitiva de .one Meter es la gestión de grandes volúmenes de activos mediante IoT y RFID con trazabilidad corporativa. Frente a ello, Regula aplica una estrategia de accesibilidad y enfoque en PYMES.

Aunque .one Meter ofrece soluciones avanzadas para grandes compañías, su complejidad y costos dificultan su adopción en distribuidores pequeños y medianos.

**Táctica:**  
Posicionar a Regula como una alternativa moderna, sencilla y accesible económicamente, permitiendo que empresas con menor capacidad de inversión puedan digitalizar sus operaciones sin requerir infraestructuras complejas.

---

## Estrategias para aprovechar las debilidades de los competidores

### Debilidad de IoT Smart Gas Platform

Su enfoque está limitado principalmente al monitoreo del gas y depende considerablemente de hardware especializado, lo que incrementa costos de implementación.

Regula aprovecha esta debilidad ofreciendo una plataforma centrada también en procesos administrativos y operativos del negocio, reduciendo la dependencia exclusiva del monitoreo físico.

**Táctica:**  
Enfatizar el ahorro operativo y la facilidad de implementación mediante una aplicación web accesible desde cualquier dispositivo con internet.

### Debilidad de GasSense

Su propuesta se concentra en el análisis del consumo y no en la gestión integral de operaciones empresariales.

Regula aprovecha esta brecha ofreciendo módulos orientados específicamente al control de distribución, inventario y cobranzas.

**Táctica:**  
Mostrar casos de uso relacionados con empresas distribuidoras de GLP, evidenciando cómo Regula mejora la eficiencia operativa y reduce problemas administrativos cotidianos.

### Debilidad de .one Meter

Su alto costo y complejidad de implementación dificultan la adopción por parte de pequeñas y medianas empresas.

Regula aprovecha esta debilidad mediante una estrategia de penetración en el segmento pyme, ofreciendo una solución SaaS más flexible y económica.

**Táctica:**  
Brindar demostraciones gratuitas, pruebas piloto y acompañamiento inicial para facilitar la adopción tecnológica por parte de distribuidores tradicionales.

---

## Estrategias para aprovechar las oportunidades del entorno

El sector de distribución de GLP presenta una baja digitalización y todavía depende en gran medida de procesos manuales para el control de inventario, distribución y cobranzas.

Regula aprovecha esta oportunidad mediante una estrategia de transformación digital accesible, enfocándose en empresas que necesitan modernizar sus operaciones sin realizar inversiones elevadas.

**Táctica:**  
Ofrecer una plataforma intuitiva y fácil de implementar, acompañada de capacitaciones y soporte básico para acelerar la adopción.

Asimismo, existe una creciente preocupación por la seguridad en almacenes y operaciones relacionadas con gas GLP, especialmente en empresas que aún no cuentan con sistemas de monitoreo ambiental.

Regula aprovecha esta oportunidad integrando sensores ambientales y alertas en tiempo real dentro de su propuesta de valor.

**Táctica:**  
Comunicar la importancia de la prevención de fugas y riesgos operativos como un beneficio diferencial frente a otras soluciones centradas únicamente en consumo o logística.

Otra oportunidad importante es el incremento del interés por soluciones IoT y plataformas inteligentes en el sector energético.

Regula aprovecha este contexto posicionándose como una startup innovadora que integra monitoreo y gestión operativa en una única solución.

**Táctica:**  
Fortalecer la presencia digital mediante landing pages, redes sociales y demostraciones enfocadas en mostrar beneficios reales para distribuidores y empresas envasadoras.

---

## Estrategias para mitigar las amenazas del entorno

Una de las principales amenazas identificadas es la presencia de empresas tecnológicas ya posicionadas en el mercado IoT y energético, las cuales cuentan con mayor reconocimiento y experiencia.

Para mitigar esta amenaza, Regula aplica una estrategia de diferenciación basada en cercanía con el cliente y adaptación a necesidades reales del sector GLP.

**Táctica:**  
Mantener comunicación constante con los primeros clientes para incorporar mejoras continuas al sistema según sus problemas operativos reales.

Otra amenaza importante es la resistencia al cambio y la baja adopción tecnológica por parte de distribuidores tradicionales que aún trabajan con métodos manuales.

Regula enfrenta esta situación mediante una estrategia de simplificación de uso y acompañamiento inicial.

**Táctica:**  
Ofrecer capacitaciones, soporte básico y una interfaz intuitiva que reduzca la dificultad de transición hacia procesos digitalizados.

Finalmente, existe la amenaza de que nuevas soluciones tecnológicas más económicas ingresen al mercado y compitan directamente con Regula.

Para reducir este riesgo, la startup aplica una estrategia de fidelización temprana, buscando construir relaciones sólidas con sus primeros clientes.

**Táctica:**  
Proporcionar atención personalizada, actualizaciones frecuentes y mejoras constantes que generen confianza y dependencia positiva hacia la plataforma.

## **2.2. Entrevistas**

### **2.2.1. Diseño de entrevistas**

**Segmento Objetivo 1: Empresas de gas (productoras y distribuidoras a gran escala)**

1. ¿Cómo gestionan actualmente el control de inventario de balones de gas?
2. ¿Qué tipo de problemas han tenido con fugas de gas en sus instalaciones o almacenes?
3. ¿Cómo detectan actualmente una posible fuga de gas?
4. ¿Han tenido pérdidas económicas por fugas de gas o balones en mal estado?
5. ¿Cómo registran las entradas y salidas de balones en su empresa?
6. ¿Utilizan algún sistema digital o lo manejan de forma manual? (papel, excel, etc.)
7. ¿Qué tan frecuente es que tengan errores en el inventario o desorden en los registros?
8. ¿Han tenido problemas de robos o pérdidas de balones durante el transporte?
9. ¿Cuentan con algún sistema de monitoreo o seguimiento de sus camiones en ruta?
10. ¿Qué dificultades enfrentan al momento de gestionar la distribución de balones?
11. ¿Cómo manejan actualmente la cobranza a sus clientes?
12. ¿Tienen problemas con clientes que no pagan a tiempo? ¿Con qué frecuencia ocurre?
13. ¿Como registran y hacen seguimiento a las deudas de sus clientes?
14. ¿Qué áreas conforman a la empresa, cual es su función?
15. ¿Si existiera una solución/aplicación que permita monitorear almacenes, distribución e inventario en tiempo real, qué funcionalidades considerarían más importantes?

**Segmento Objetivo 2: Distribuidores de gas (minoristas y puntos de venta)**

1. ¿Cómo controlan los balones en su almacén? ¿Anotan en cuaderno o usan algún sistema?
2. ¿Cómo se dan cuenta si un balón está mal o defectuoso?
3. ¿Qué hacen cuando ven que un balón tiene fuga?
4. ¿Qué parte del trabajo les toma más tiempo en el día?
5. ¿Qué les preocupa más en el negocio: perder dinero, problemas de seguridad o perder clientes? ¿Por qué?
6. ¿Qué problemas suelen tener cuando hacen entregas?
7. ¿Ah tenido problemas con sus repartidores? (entregas tardías, motorizado no conoce la zona, etc)
8. ¿Tienen clientes que compran fiado? ¿Es difícil cobrarles después?
9. ¿Es importante para ustedes saber lo que pasa en tiempo real (ventas, entregas, etc.)?
10. ¿Usan una computadora o celular para gestionar su trabajo, o lo hacen todo en papel?
11. ¿Si pudieran mejorar algo de su trabajo, ¿qué cambiarían?
12. ¿Les gustaría tener una app de apoyo que les permita ver a sus motorizados en tiempo real?
13. ¿Qué opinas de usar una app que te ayude a gestionar mejor tu flujo de ventas y compra de balones?

### **2.2.2. Registro de entrevistas**

**Segmento Objetivo 1: Empresas de gas**

 <table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #1<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Eric</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Tello Ortíz</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>43 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Los Olivos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-1-1 AW.png" alt="Entrevista a Eric Tello"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td> 30:09 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>05:54 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado indica que es representante de una empresa de gas con un perfil práctico y operativo, basado en la experiencia y en procesos mayormente manuales. El control de stock se realiza mediante un conteo visual y registros en cuadernos, considerando también los balones vacíos para estimar reposición. No utiliza sistemas digitales, lo que genera errores frecuentes como olvidos de pedidos, error de cálculos o duplicidad de registros. La detección de fugas se hace con métodos tradicionales como usar agua con jabón para saber el lugar exacto de la fuga en el balón y por el olor a gas, identificando fallas en válvulas o en la estructura del balón, lo que en algunos casos ha generado pérdida de clientes por desconfianza o miedo a un accidente por fuga de gas en sus casas. Los pedidos se gestionan mediante llamadas telefónicas y mensajes de WhatsApp, utilizando un celular Samsung S26, lo que refleja un canal de atención directo y tradicional. Presenta créditos a clientes recurrentes, pero presenta dificultades en la cobranza por falta de seguimiento. Podemos observar que muestra una operación tradicional. Nos damos cuenta de que hay claras oportunidades de mejora en digitalización, control de inventario y gestión de distribución, registro de ventas y una geolocalización de tiempo real de sus vehículos.
</td>
  </tr>
</tbody>
</table>

<br><br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #2<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Rafael</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Palacios Arana</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>60 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Chosica</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-1-2 AW.png" alt="Entrevista a Rafael Palacios"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td> 36:20 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>10:34 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado, de 60 años y residente en Chosica, es representante de una empresa distribuidora y envasadora de gas con amplia experiencia. Presenta un perfil técnico y orientado a la seguridad, utilizando Microsoft Excel en computadora junto con registros físicos para controlar inventarios mediante guías de remisión y conteos diarios. La recepción de pedidos se realiza principalmente por llamadas a un celular con sistema Android, el cual es un Samsung S25, reflejando un canal tradicional.
Identifica como principales problemas las fugas de gas y el uso de cilindros antiguos, detectándose con métodos básicos como agua jabonosa. Aunque no presenta grandes fallas operativas, ha sufrido robos durante el transporte de balones en camiones, por lo que utiliza un servicio de GPS para monitoreo de sus unidades en tiempo real. A nivel comercial, trabaja solo al contado debido a problemas previos con créditos y cuenta con áreas organizadas (administración, ventas, producción y seguridad). En conjunto, muestra una empresa con buen control operativo y experiencia, pero con oportunidades de mejora en digitalización sus registros de compra y venta. 

</td>
  </tr>
</tbody>
</table>



<br><br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #3<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Maximiliano</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Flores</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>42 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Martín de Porres</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-1-3 AW.png" alt="Entrevista a Maximiliano"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td>46:42 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>08:38 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado, Maximiliano Flores, de 42 años y residente en San Martín de Porres, es representante de una empresa embasadora de gas con un perfil práctico y empírico, basado en la experiencia y en procesos manuales. Gestiona inventario, compras, ventas y cobranzas mediante cuadernos, lo que genera errores frecuentes, olvidos y mayor carga de trabajo, incluso teniendo que duplicar registros para evitar pérdida de información. En cuanto a la seguridad, realiza revisiones constantes de los balones para evitar fugas, las cuales se presentan principalmente por mala manipulación de los clientes. La gestión de pedidos se realiza por llamadas y WhatsApp, utilizando un celular Android marca Samsung, reflejando un canal de atención tradicional .

Presenta bajo nivel de conocimiento tecnológico y no utiliza sistemas digitales ni monitoreo de transporte, aunque muestra interés en implementar herramientas tecnológicas que le permitan optimizar su trabajo. En conjunto, evidencia una operación tradicional con oportunidades claras de mejora en digitalización, control de información y eficiencia operativa.

</td>
  </tr>
</tbody>
</table>
<br><br>

**Segmento Objetivo 2: Distribuidores de gas**

<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #1<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Roberto</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Arriola</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>55 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Puente Piedra</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-2-1 AW.png" alt="Entrevista a Roberto Arriola"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td> 00:07 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>09:16 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado Roberto Arriola es un distribuidor de gas con un perfil operativo y empírico. Gestiona el inventario de forma manual en cuadernos, que luego son digitalizados en Microsoft Excel, evidenciando bajo nivel de digitalización directa. Se comunica con clientes mediante llamadas desde un celular Android marca Honor, usando canales como llamadas por WhatsApp o llamadas al celular fijo.
Considera que las fugas provienen principalmente de válvulas de los clientes, las cuales soluciona en el momento con herramientas simples. Sus principales problemas son el tráfico y dificultades en entregas (direcciones poco claras y edificios sin ascensor), además de retrasos de repartidores. Su mayor preocupación es la pérdida de clientes por el crecimiento del gas natural. No trabaja con crédito y maneja pagos inmediatos. Tecnologías implementadas: Computadora con componentes de oficina con sistema Microsoft integrado y dispositivo móvil Android marca Honor. Aunque su operación es manual, muestra apertura al uso de tecnología, especialmente apps para monitoreo y gestión, lo que evidencia oportunidades de mejora en digitalización y optimización logística.


</td>
  </tr>
</tbody>
</table>

<br><br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #2<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Edgar</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Palacios Arango</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>45 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Los Olivos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-2-2 AW.png" alt="Entrevista a Edgar Palacios"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td> 09:53 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>14:14 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado, Edgar Palacios, es un distribuidor independiente de gas con más de 20 años de experiencia, con formación previa en una empresa envasadora de gas (Anta Gas). Presenta un perfil práctico y empírico, orientado a la seguridad y basado en la experiencia. Gestiona su negocio de forma autónoma, encargándose del almacenamiento, distribución y atención al cliente, destacando por su trato cercano y de confianza.
Su control de inventario lo realiza de forma manual en cuadernos, registrando entradas, salidas, ventas y créditos, lo que evidencia un bajo nivel de digitalización. Para detectar fugas utiliza métodos tradicionales como usar agua con jabón para detectar el lugar preciso de la fuga, revisando balón por balón y separando los defectuosos. Su principal preocupación es económica, especialmente ante la escasez de gas.
Los pedidos se gestionan mediante llamadas y WhatsApp, usando un celular Android (marca Honor), reflejando un canal de interacción directo. Además, usa Yape o Plin para sus pagos y así llevar un registro de imágenes de sus compras y ventas. No cuenta con sistema de monitoreo en tiempo real para sus pedidos, pero muestra interés en apps que integren un servicio de geolocalización, aunque mantiene desconfianza al delegar pedidos a motorizados tercerizados. Maneja pagos a crédito solo con clientes de confianza, apuntando todos su pagos pendientes y deudas de clientes en un cuadernillo.
En conjunto, representa un negocio pequeño pero estable, con procesos manuales y cercanía al cliente, pero con ciertos problemas al momento de llevar un historial de pagos y administración de stock de sus balones. El entrevistado concluye diciendo que una app web que le permita llevar sus registros económicos y que le permita usar un servicio de geolocalización en tiempo real para futuros motorizados le quitaría un gran peso de encima y facilitaría su trabajo.


</td>
  </tr>
</tbody>
</table>


<br><br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2">Entrevista #3<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Jesus</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Felices</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>22 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Puente Piedra</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="../../report/assets/interviews/entrevista-2-3 AW.png" alt="Entrevista a Jesus Felices"></td>
  </tr>
  <tr>
    <td>Link</td>
    <td><p><a target="_blank"  href="https://upcedupe-my.sharepoint.com/personal/u20241e321_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20241e321%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevistas%20AW%20%281%29%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eed871f48%2Dd85e%2D4371%2D9363%2D4e76ce0b5f4b&mode=Edit" title="Title">Microsoft Stream</p></td>
  </tr>
  <tr>
    <td>Minuto de inicio<br></td>
    <td> 23:38 min</td>
  </tr>
  <tr>
    <td>Duracion<br></td>
    <td>06:26 min</td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td>
		El entrevistado, Jesús Felices, es administrador y representante de una empresa distribuidora de gas que opera como sucursal, mostrando un perfil organizado, operativo y orientado a procesos formales. A diferencia de otros casos más tradicionales, evidencia un nivel de digitalización intermedio, ya que el control de inventario se realiza en un dispositivo de Microsoft mediante herramientas como Word y Excel en computadora, gestionadas por personal capacitado, aunque anteriormente utilizaban cuadernos. En cuanto a la gestión operativa, aplican revisiones individuales a cada balón para detectar fugas o defectos, los cuales son separados y devueltos al distribuidor principal, reflejando dependencia de un proveedor mayor. Su principal preocupación está en la eficiencia de la distribución, debido a zonas alejadas, direcciones imprecisas, lo que genera retrasos en las entregas y molestias en los clientes.
A nivel tecnológico, utilizan computadoras con sistema operativo Microsoft; no tan potentes, ideales para oficina, para la administración, y un celular Android (Xiaomi Redmi Note 11) para el monitoreo y coordinación de operaciones. Los pedidos se reciben mediante llamadas telefónicas y mensajes de WhatsApp, manteniendo un canal directo con los clientes. También manejan ventas al crédito con seguimiento periódico, sin mayores inconvenientes hasta el momento.
Observamos que tiene potencial para soluciones digitales para un registro de ventas, almacén y geolocalización de sus deliverys



</td>
  </tr>
</tbody>
</table>

<br><br>

# 2.2.3. Análisis de entrevistas

## Segmento Objetivo 1: Empresas de gas (productoras y distribuidoras a gran escala)

De acuerdo con las 3 entrevistas realizadas a representantes de empresas distribuidoras y envasadoras de gas, se identificaron patrones comunes relacionados con la operación, gestión logística, nivel de digitalización y seguridad operativa. A pesar de contar con una estructura organizativa más sólida que el segmento minorista, la mayoría de empresas aún depende parcialmente de procesos manuales y herramientas tecnológicas básicas.

---

## Nivel de digitalización

El 66% de los entrevistados (2 de 3) presenta un bajo nivel de digitalización, debido a que gestionan inventarios, ventas y cobranzas principalmente mediante cuadernos físicos y registros manuales.

Por otro lado, el 33% restante utiliza herramientas digitales básicas como Microsoft Excel complementadas con documentos físicos y guías de remisión.

Esto evidencia que, aunque existe una adopción parcial de tecnología, los procesos críticos del negocio aún no se encuentran centralizados y automatizados completamente.

---

## Gestión de inventario

El 100% de los entrevistados realiza control de inventario, aunque utilizando métodos distintos:

- 66% realiza controles manuales mediante conteos visuales, cuadernos y duplicación de registros.
- 33% utiliza un sistema mixto basado en Excel, documentos físicos y registros administrativos.

Se identificó que los procesos actuales generan errores de registro, pérdida de tiempo y dificultades para consultar información histórica de ventas o stock.

---

## Detección de fugas y seguridad

El 100% de los entrevistados utiliza métodos tradicionales para detectar fugas de gas, principalmente:

- Agua con jabón
- Inspección manual
- Revisión visual y olfativa

Además, los entrevistados manifestaron preocupación constante por accidentes relacionados con cilindros deteriorados o válvulas defectuosas, debido al riesgo operativo y a la posible pérdida de confianza de los clientes.

---

## Canales de interacción con clientes

El 100% de los entrevistados utiliza canales de comunicación tradicionales y de fácil acceso:

- Llamadas telefónicas
- WhatsApp

Esto demuestra que la atención al cliente continúa siendo directa y poco automatizada, utilizando principalmente celulares Android como herramienta principal de trabajo diario.

---

## Tecnología y dispositivos utilizados

Respecto al uso tecnológico, se identificó que:

- El 100% utiliza celulares Android para la coordinación operativa.
- El 33% utiliza sistemas GPS para monitoreo de transporte.
- El 33% emplea Microsoft Excel como principal herramienta digital de gestión.

En general, las empresas utilizan tecnología básica enfocada en comunicación y ofimática, sin contar con plataformas integradas especializadas para gestión logística y administrativa.

---

## Problemas principales identificados

Los problemas más frecuentes identificados durante las entrevistas fueron:

- Errores en registros manuales
- Dependencia excesiva de procesos físicos
- Estrés operativo por duplicación de información
- Riesgos logísticos y robos durante el transporte
- Dificultad para controlar créditos y cobranzas
- Falta de monitoreo centralizado en tiempo real

Asimismo, varios entrevistados manifestaron preocupación por la pérdida de clientes debido al crecimiento del gas natural y por la dificultad de mantener una operación eficiente utilizando únicamente procesos manuales.

---

## Modelo de cobranza

Se identificó que:

- 33% trabaja con créditos, aunque presenta dificultades de seguimiento.
- 33% opera únicamente al contado debido a malas experiencias previas.
- 33% mantiene un modelo tradicional sin procesos digitalizados de cobranza.

Esto evidencia que la gestión financiera aún presenta limitaciones y poca trazabilidad.

---

## Características objetivas identificadas

- Uso frecuente de celulares Android.
- Predominio de registros manuales.
- Uso limitado de herramientas digitales.
- Dependencia de llamadas y WhatsApp.
- Gestión administrativa parcialmente estructurada.
- Operaciones enfocadas en distribución y logística.

---

## Características subjetivas identificadas

- Estrés operativo generado por procesos manuales.
- Preocupación por pérdidas económicas y robos.
- Temor a accidentes relacionados con fugas.
- Interés en herramientas tecnológicas simples y accesibles.
- Necesidad de mayor control y monitoreo operativo.
- Interés en reducir errores humanos y tiempos de gestión.

---

## Key Insights

- Los usuarios muestran apertura hacia la digitalización, pero prefieren herramientas simples y fáciles de implementar.
- El principal problema no es únicamente el inventario, sino la falta de control operativo centralizado.
- WhatsApp se ha convertido en una herramienta operativa informal clave dentro del negocio.
- Existe interés en monitoreo logístico y automatización, especialmente para reducir errores y mejorar la trazabilidad.
- La seguridad y la confianza del cliente son factores prioritarios para las empresas entrevistadas.

---

## Relación con los User Persona

A partir de este segmento se identificaron perfiles potenciales para la construcción de User Persona, tales como:

- Administrador operativo tradicional
- Supervisor logístico
- Encargado de distribución y monitoreo

---

## Oportunidades identificadas

A partir de las entrevistas se identificaron oportunidades para implementar funcionalidades como:

- Control digital de inventario
- Registro automatizado de ventas y cobranzas
- Monitoreo GPS en tiempo real
- Gestión centralizada de clientes
- Alertas relacionadas con seguridad y fugas
- Dashboard administrativo para supervisión operativa

---

## Conclusión del segmento

El Segmento Objetivo 1 presenta un nivel mixto de digitalización, donde la mayoría de empresas aún depende de procesos manuales complementados parcialmente con herramientas digitales básicas. Aunque cuentan con mayor estructura organizativa, persisten problemas relacionados con control operativo, logística y administración de información.

Además, se evidenció una clara apertura hacia soluciones tecnológicas accesibles que permitan mejorar la eficiencia operativa, reducir errores manuales y optimizar el monitoreo de inventario, transporte y cobranzas en tiempo real.

---

## Resumen estadístico del segmento

| Aspecto evaluado | Resultado |
|---|---|
| Uso de celulares Android | 100% |
| Uso de llamadas telefónicas | 100% |
| Uso de WhatsApp | 100% |
| Uso de registros manuales | 66% |
| Uso de Microsoft Excel | 33% |
| Uso de monitoreo GPS | 33% |
| Uso de métodos tradicionales para detección de fugas | 100% |
| Empresas con dificultades en cobranzas | 66% |
| Empresas preocupadas por riesgos operativos y robos | 100% |
| Empresas interesadas en digitalización | 100% |
| Empresas con dificultades para monitoreo centralizado | 100% |
| Empresas que presentan estrés operativo por duplicidad de procesos | 66% |

---

## Patrones predominantes identificados

| Patrón identificado | Frecuencia | Impacto |
|---|---|---|
| Dependencia de procesos manuales | Alta | Genera errores administrativos y pérdida de tiempo |
| Uso intensivo de WhatsApp como canal operativo | Alta | Centraliza pedidos y coordinación diaria |
| Bajo nivel de automatización | Media-Alta | Limita el monitoreo y control operativo |
| Preocupación por fugas y seguridad | Alta | Influye en la confianza del cliente |
| Necesidad de trazabilidad logística | Alta | Justifica monitoreo y seguimiento de entregas |
| Dificultad en gestión de cobranzas | Media | Afecta organización financiera |
| Interés en herramientas simples y centralizadas | Alta | Impacta el diseño UX de la solución |

---

# Segmento Objetivo 2: Distribuidores de gas (minoristas y puntos de venta)

De acuerdo con las 3 entrevistas realizadas a distribuidores independientes y representantes de puntos de venta de gas, se identificaron patrones comunes relacionados con el bajo nivel de digitalización, dependencia de procesos manuales y dificultades logísticas durante la operación diaria.

---

## Nivel de digitalización

El 66% de los entrevistados presenta un nivel bajo de digitalización, ya que gestiona inventario, ventas y registros mediante cuadernos físicos y anotaciones manuales.

En contraste, el 33% utiliza herramientas digitales básicas como Microsoft Excel y Word, aunque aún complementadas con procesos manuales.

Esto demuestra que la digitalización dentro del segmento continúa siendo limitada y poco integrada.

---

## Gestión de inventario

El 100% de los entrevistados realiza control de inventario, aunque mediante métodos distintos:

- 66% utiliza controles manuales mediante cuadernos y anotaciones diarias.
- 33% realiza control digital básico desde computadora con apoyo administrativo.

Los entrevistados señalaron que los registros manuales generan pérdida de tiempo, errores frecuentes y dificultades para consultar información histórica.

---

## Detección de fugas y seguridad

El 100% utiliza métodos tradicionales para detectar fugas, principalmente:

- Agua con jabón
- Inspección manual

Asimismo, indicaron que los balones defectuosos suelen ser separados y enviados nuevamente al proveedor o distribuidor principal.

Los entrevistados mostraron preocupación por posibles accidentes relacionados con fugas y por la pérdida de confianza de los clientes frente a incidentes de seguridad.

---

## Canales de interacción con clientes

El 100% utiliza:

- Llamadas telefónicas
- WhatsApp

Esto evidencia que los celulares Android representan la principal herramienta de trabajo para coordinar pedidos, entregas y comunicación con clientes.

---

## Tecnología y dispositivos utilizados

Se identificó que:

- El 100% utiliza celulares Android para la operación diaria.
- El 66% utiliza herramientas digitales básicas como Excel.
- El 33% cuenta con una gestión más estructurada desde computadora.

En general, la tecnología utilizada se limita a herramientas básicas de comunicación y ofimática, sin plataformas especializadas integradas.

---

## Problemas principales identificados

Los principales problemas identificados fueron:

- Tráfico y retrasos en entregas
- Direcciones imprecisas
- Falta de monitoreo en tiempo real
- Errores en registros manuales
- Dificultad para controlar ventas y cobranzas
- Estrés operativo por exceso de tareas manuales

Además, algunos entrevistados manifestaron desconfianza hacia repartidores tercerizados y preocupación por perder clientes frente a otras alternativas energéticas.

---

## Modelo de cobranza

Se identificó que:

- El 66% limita el crédito únicamente a clientes de confianza.
- El 33% maneja seguimiento más estructurado de cobranzas.

Esto evidencia que la gestión de créditos aún depende principalmente de confianza y registros manuales.

---

## Características objetivas identificadas

- Uso generalizado de celulares Android.
- Dependencia de llamadas y WhatsApp.
- Uso frecuente de cuadernos físicos.
- Bajo nivel de automatización.
- Operaciones enfocadas en reparto y atención directa.

---

## Características subjetivas identificadas

- Estrés por retrasos y desorganización operativa.
- Temor a perder clientes.
- Desconfianza hacia terceros encargados de entregas.
- Interés en herramientas simples y económicas.
- Necesidad de mayor control sobre repartidores y ventas.

---

## Key Insights

- Los usuarios no rechazan la tecnología; rechazan herramientas complejas.
- WhatsApp se ha convertido en el centro operativo informal del negocio.
- El principal dolor no es únicamente el inventario, sino la pérdida de control operativo.
- Existe interés en la geolocalización debido a problemas de confianza y retrasos.
- Los usuarios priorizan simplicidad antes que automatización avanzada.

---

## Relación con los User Persona

A partir de este segmento se identificaron perfiles potenciales para User Persona como:

- Distribuidor independiente
- Microempresario tradicional
- Repartidor multifuncional

---

## Oportunidades identificadas

A partir de las entrevistas se identificaron oportunidades para implementar funcionalidades como:

- Geolocalización de repartidores
- Control digital de inventario
- Registro de ventas y clientes
- Historial de cobranzas
- Monitoreo de entregas en tiempo real
- Dashboard administrativo simplificado

---

## Resumen estadístico del segmento

| Aspecto evaluado | Resultado |
|---|---|
| Uso de celulares Android | 100% |
| Uso de llamadas telefónicas | 100% |
| Uso de WhatsApp | 100% |
| Uso de registros manuales | 66% |
| Uso de Microsoft Excel | 66% |
| Uso de computadora para gestión administrativa | 33% |
| Uso de métodos tradicionales para detección de fugas | 100% |
| Distribuidores con problemas logísticos y retrasos | 100% |
| Distribuidores con dificultades en cobranzas | 66% |
| Distribuidores interesados en monitoreo de repartidores | 100% |
| Distribuidores interesados en herramientas simples | 100% |
| Distribuidores con estrés operativo | 100% |

---

## Patrones predominantes identificados

| Patrón identificado | Frecuencia | Impacto |
|---|---|---|
| Dependencia de procesos manuales | Alta | Genera desorganización y errores frecuentes |
| Uso intensivo de WhatsApp | Alta | Se convierte en principal herramienta operativa |
| Problemas de logística y tráfico | Alta | Afecta tiempos de entrega |
| Necesidad de monitoreo de repartidores | Alta | Relacionado con confianza y control |
| Bajo nivel de automatización | Alta | Reduce eficiencia operativa |
| Estrés operativo por exceso de tareas manuales | Alta | Impacta productividad diaria |
| Interés en soluciones simples y económicas | Alta | Condiciona aceptación de la plataforma |
| Dificultad para controlar créditos y cobranzas | Media | Genera problemas financieros y seguimiento limitado |

---

## Conclusión del segmento

El Segmento Objetivo 2 presenta una alta dependencia de procesos manuales y un uso básico de tecnología centrado principalmente en celulares Android y herramientas de comunicación. Los principales problemas se concentran en la logística, control de inventario y monitoreo operativo.

Las entrevistas evidencian una clara oportunidad para implementar soluciones digitales accesibles, simples y centralizadas que permitan mejorar la organización del negocio, reducir errores manuales y optimizar la supervisión de entregas y ventas en tiempo real.

---

## Resumen final de patrones

| Patrón identificado | Frecuencia | Impacto |
|---|---|---|
| Dependencia de WhatsApp | Alta | Comunicación operativa |
| Uso de procesos manuales | Alta | Genera errores y retrasos |
| Interés en soluciones simples | Alta | Influye en diseño UX |
| Problemas de monitoreo | Media-Alta | Justifica geolocalización |
| Estrés operativo | Alta | Impacta eficiencia |



## **2.3. Needfinding**

### **2.3.1. User Personas**

Para diseñar una solución realmente útil, es fundamental entender a quién va dirigida. Por ello, se han desarrollado User Personas que representan de forma realista a nuestros dos segmentos principales: las empresas envasadoras de gas y los distribuidores de balones. Estos perfiles se construyen a partir de la información obtenida en entrevistas y análisis del contexto, reflejando sus necesidades, problemas y forma de trabajo en el día a día. De esta manera, las User Personas nos permiten tener una visión más clara del usuario, ayudando a que el diseño de la aplicación web Regula esté enfocado en resolver situaciones reales y aportar valor en sus operaciones.

Segmento Objetivo 1: Empresas de gas (productoras y distribuidoras a gran escala)

<div align="center">
    <img src="../../report/assets/diagrams/user-persona-Miguel-Hordoñez.png" alt="imagen user persona Miguel">
</div>

Miguel Hordoñez es un administrador de 58 años que trabaja en una empresa productora de gas, con amplia experiencia en la supervisión de operaciones de envasado y distribución. Su rol está más orientado a la gestión y control estratégico, manejando grandes volúmenes de balones y priorizando la seguridad, eficiencia y trazabilidad en todos los procesos.

Su principal objetivo es tener un control preciso del inventario y reducir pérdidas operativas como fugas, robos o errores en registros. Sin embargo, enfrenta problemas como la falta de digitalización completa, errores en procesos manuales y dificultad para centralizar información en tiempo real.

<br>
<br>

Segmento Objetivo 2: Distribuidores de gas (minoristas y puntos de venta)

<div align="center">
<img src="../../report/assets/diagrams/user-persona-Carlos-Mendoza .png" alt="imagen user persona Carlos">
</div>

Carlos Mendoza es un distribuidor independiente de balones de gas de 48 años, con más de 15 años de experiencia en el rubro. Maneja su negocio de forma autónoma, encargándose personalmente del inventario, las ventas y la distribución, basándose principalmente en su experiencia y en la relación de confianza con sus clientes.

Su principal objetivo es tener un mejor control de su negocio, reduciendo errores en los registros, organizando sus pedidos y aumentando sus ventas. Sin embargo, enfrenta problemas como el desorden en el seguimiento de pedidos, pérdida de tiempo en procesos manuales y dificultad para llevar control de clientes y deudas. Aunque no tiene un alto dominio tecnológico, está dispuesto a usar herramientas simples que le ayuden a trabajar de manera más rápida, ordenada y eficiente.

# 2.3.2. User Task Matrix

| Tasks | Administrador Operativo | Supervisor Logístico | Distribuidor Independiente | Encargado de Almacén |
|---|---|---|---|---|
| Supervisar operaciones diarias | Alta | Alta | Media | Media |
| Controlar inventario de balones | Alta | Media | Alta | Alta |
| Registrar ventas realizadas | Media | Baja | Alta | Media |
| Revisar cobranzas y pagos pendientes | Alta | Baja | Alta | Baja |
| Coordinar entregas y pedidos | Media | Alta | Alta | Baja |
| Supervisar repartidores | Media | Alta | Media | Baja |
| Verificar ubicación de entregas | Baja | Alta | Alta | Baja |
| Detectar posibles riesgos o fugas | Media | Media | Baja | Alta |
| Registrar entradas y salidas de balones | Baja | Baja | Media | Alta |
| Consultar información histórica de operaciones | Media | Media | Baja | Media |
| Comunicarse con clientes | Media | Media | Alta | Baja |
| Organizar rutas de distribución | Baja | Alta | Alta | Baja |
| Resolver problemas operativos diarios | Alta | Alta | Alta | Media |

---

A partir del análisis realizado, se identificó que las tareas con mayor frecuencia e importancia para la mayoría de User Persona están relacionadas con el control operativo, coordinación logística y supervisión de inventario. Estas actividades representan procesos críticos dentro de las operaciones diarias de distribución y comercialización de gas.

Se observó que el Administrador Operativo y el Supervisor Logístico presentan una alta participación en tareas relacionadas con supervisión general, monitoreo de operaciones y control administrativo. Por otro lado, el Distribuidor Independiente concentra principalmente actividades relacionadas con ventas, coordinación de pedidos y seguimiento de entregas, evidenciando una fuerte carga operativa diaria.

Asimismo, el Encargado de Almacén se enfoca principalmente en tareas relacionadas con control de inventario, registro de movimientos de balones y detección de riesgos operativos asociados al almacenamiento.

## Principales coincidencias identificadas entre los User Persona

- La necesidad de controlar inventario y operaciones diariamente.
- La importancia de coordinar correctamente entregas y distribución.
- La dependencia de procesos manuales para registrar información.
- La necesidad de resolver problemas operativos de manera constante.

Finalmente, las diferencias entre perfiles se evidencian principalmente en el nivel de responsabilidad logística y administrativa que cada usuario posee dentro de la operación. Mientras algunos perfiles priorizan supervisión estratégica y control administrativo, otros se enfocan en tareas operativas relacionadas directamente con reparto, ventas y atención diaria de clientes.
### **2.3.3. User Journey Mapping**

En esta sección se presentan los User Journey Mapping, los cuales permiten visualizar paso a paso la experiencia de los usuarios al realizar sus actividades dentro del proceso de gestión y distribución de balones de gas. A través de estos recorridos, se identifican las acciones, puntos de contacto, dificultades y emociones que experimentan los usuarios en cada etapa. Este análisis ayuda a comprender mejor su experiencia actual y detectar oportunidades donde Regula puede intervenir para mejorar la eficiencia, organización y seguridad en sus operaciones.

**Segmento Objetivo 1: Empresas de gas (productoras y distribuidoras a gran escala)**

![user-journey-map-1](../../report/assets/diagrams/Journey%20Map%20Miguel%20Hordoñez.png)


**Segmento Objetivo 2: Distribuidores de gas (minoristas y puntos de venta)**

![user-journey-map-2](../../report/assets/diagrams/Journey%20Map%20Carlos%20Mendoza.png)

<br>

### **2.3.4. Empathy Mapping**

Empathy Mapping es una herramienta que permite comprender de manera más profunda a los usuarios a partir de lo que piensan, sienten, dicen y hacen en su día a día. Este análisis se basa en los segmentos de distribuidores y empresas envasadoras de gas, con el objetivo de identificar sus preocupaciones, necesidades y motivaciones reales. De esta forma, se obtiene una visión más humana del usuario, lo que facilita diseñar una solución como Regula que responda mejor a sus problemas y mejore su experiencia en la gestión de sus operaciones.

**Segmento 1: Empresas de gas**

<div align="center">

![empathy-mapping-1](../../report/assets/diagrams/Empathy%20Mapping%20Miguel%20Hordoñez.png)

</div>

**Segmento 2: Distribuidoras de gas**

![empathy-mapping-1](../../report/assets/diagrams/Empathy%20Mapping%20Carlos%20Mendoza%20(1).png)
















# Glosario del Dominio - Plataforma de Balones de Gas

A continuación se presenta un glosario con los términos centrales del dominio de la plataforma. Este vocabulario compartido garantiza que todas las partes involucradas (usuarios, desarrolladores, stakeholders) utilicen un lenguaje consistente y sin ambigüedades.

| Término (Inglés)       | Término (Español)            | Definición clara y compartida |
|------------------------|-----------------------------|-------------------------------|
| Gas Cylinder          | Balón de gas                | Recipiente que almacena gas GLP utilizado para distribución y venta a clientes finales. |
| Gas Leak              | Fuga de gas                 | Escape de gas desde un balón, válvula o conexión, que representa un riesgo de seguridad y pérdida de producto. |
| Storage Area          | Área de almacenamiento      | Espacio físico donde se guardan los balones de gas antes de su distribución o venta. |
| Gas Detection         | Detección de gas            | Proceso de identificar la presencia de gas en el ambiente mediante sensores o inspección manual. |
| Inventory Control     | Control de inventario       | Registro y seguimiento de la cantidad, estado y movimiento de balones dentro del negocio. |
| Entry Record          | Registro de entrada         | Registro de balones que ingresan al almacén o punto de venta. |
| Exit Record           | Registro de salida          | Registro de balones que salen para distribución o venta. |
| Delivery Tracking     | Seguimiento de entregas     | Monitoreo del recorrido y estado de las entregas de balones en tiempo real. |
| Delivery Operator     | Repartidor / motorizado     | Persona encargada de transportar y entregar los balones de gas a los clientes. |
| Vehicle Identification| Identificación del vehículo | Información asociada al transporte de balones, como placa o tipo de unidad. |
| Route Monitoring      | Monitoreo de rutas          | Supervisión del recorrido de los vehículos durante la distribución de balones. |
| Stock Level           | Nivel de stock              | Cantidad disponible de balones en un almacén o punto de venta en un momento determinado. |
| Faulty Cylinder       | Balón defectuoso            | Balón que presenta fallas como fugas, corrosión o válvulas dañadas y no es apto para la venta. |
| Cylinder Inspection   | Inspección de balones       | Revisión del estado físico y funcional de los balones para detectar fallas o riesgos. |
| Soap Test             | Prueba con agua jabonosa    | Método manual utilizado para detectar fugas de gas mediante burbujas. |
| Gas Alert             | Alerta de gas               | Notificación generada al detectar presencia anormal de gas en el ambiente. |
| Real-time Monitoring  | Monitoreo en tiempo real    | Supervisión continua e inmediata de condiciones como presencia de gas o ubicación de entregas. |
| Credit Sale           | Venta al crédito            | Venta de balones donde el cliente paga en un momento posterior. |
| Debt Tracking         | Seguimiento de deudas       | Control de pagos pendientes de clientes que compran al crédito. |
| Supply Shortage       | Desabastecimiento           | Falta de balones disponibles para cubrir la demanda de los clientes. |
| Delivery Delay        | Retraso en entrega          | Demora en la entrega de balones debido a factores como tráfico o problemas de ubicación. |
| Inventory Loss        | Pérdida de inventario       | Disminución de balones por robos, fugas o mala gestión. |
| Operational Control   | Control operativo           | Supervisión general de las actividades del negocio relacionadas con inventario, distribución y seguridad. |
| Distribution Management | Gestión de distribución   | Organización y control del proceso de entrega de balones a clientes. |
| Cylinder Condition    | Estado del balón            | Situación física y funcional del balón (óptimo, defectuoso, en revisión). |



