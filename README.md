# Proyecto Final de Ingeniería en Electronica

## Estacionando: una solución al problema de conseguir estacionamiento

## Autores:
- Emanuel Cima (@cimaemanuel)
- Diego Sarina (@sarinadiego)

## Citar esta Versión
Este proyecto fue desarrollado completametente por Emanuel Cima y Diego Sarina bajo la supervisión de la catedra de Proyecto de Ingeniería Electrónica, Universidad Nacional de Rosario.

Si este trabajo ayuda a su investigación, por favor considere citarlo con la siguiente referencia:

```
Sarina Diego, Emanuel Cima, 2023. Estacionando: una solución al problema de conseguir estacionamiento
```

**Bibtext:**
```bibtex
@misc{Smart_Parking_System_2023,
    author       = {Diego Sarina, Emanuel Cima},
    title        = {Estacionando: una solución al problema de conseguir estacionamiento},
    year         = {2023},
    url = {\url{https://github.com/dsec-thesis/project_report}},
}
```


### Índice
- [Introducción](#introducción)
- [Organización](#organización)
- [Conclusiones](#conclusiones)

### Introducción
El objetivo principal de este proyecto es desarrollar un sistema de estacionamiento inteligente, que combina la tecnología de sensores y la potencia de cálculo en la nube y en el borde (edge computing). Se ha realizado un exhaustivo estudio del estado del arte en esta área, investigando los diferentes tipos de sensores disponibles y su aplicabilidad en entornos de estacionamiento.


Se llevaron a cabo pruebas de campo para evaluar la precisión y confiabilidad de los sensores en la detección de la disponibilidad de espacios de estacionamiento. Estas pruebas permitieron recopilar datos sobre la ocupación de los espacios en tiempo real y evaluar el rendimiento de los sensores en condiciones reales.


Además, se diseñó y desarrolló una aplicación móvil utilizando Flutter, un framework de desarrollo multiplataforma, que permite a los usuarios acceder a la información en tiempo real sobre la disponibilidad de espacios de estacionamiento. La aplicación ofrece funcionalidades como la búsqueda de estacionamiento cercano y la reserva de una plaza en el mismo.


Para garantizar un rendimiento óptimo y una respuesta rápida, se aprovechó la potencia de cálculo tanto en la nube como la computación de borde para el procesamiento de los datos de los sensores. Utilizando una Raspberry Pi se pudieron procesar de una manera eficiente los datos enviados por los sensores a través de LoRa y proporcionar actualizaciones en tiempo real a los usuarios de la aplicación.


En resumen, este proyecto abarcó desde el análisis del estado del arte hasta la construcción de un sistema de estacionamiento inteligente (prototipo). Se investigaron los sensores adecuados, se realizaron pruebas de campo, se desarrolló una aplicación móvil y se implementaron soluciones de computación en la nube y en el edge para ofrecer una experiencia completa al usuario. Finalmente se desarrolló un apartado de posibles mejoras al mismo.

### Organización
Todo el código relacionado a este proyecto se encuentra publicado dentro de la organización de GitHub `dsec-thesis` en ella se encuentran los siguientes repositorios:

- project_report: es el repositorio que usted esta visualizado.
- [sensor](https://github.com/dsec-thesis/sensor)
- [concentrator](https://github.com/dsec-thesis/concentrator) 
- [backend](https://github.com/dsec-thesis/backend)
- [application](https://github.com/dsec-thesis/application)

### Conclusiones
En este último capítulo, se presentan las conclusiones finales del trabajo realizado, además se exponen las limitaciones y problemas encontrados en el diseño y configuración de los equipos, junto con las interpretaciones de las pruebas realizadas.

En la concepción de la arquitectura propuesta, hemos explorado diversas perspectivas en cuanto a la integración de módulos diversos, priorizando principios de escalabilidad, seguridad y descentralización. En consecuencia, hemos concebido y desarrollado una arquitectura para sistemas de estacionamiento inteligente, aprovechando las capacidades de la computación en la nube. Hemos abordado metodologías innovadoras para la gestión dinámica de la información en la base de datos (DynamoDB), lo cual otorga la flexibilidad necesaria para la incorporación de nuevas funcionalidades y la adaptación de componentes futuros al sistema.

Hemos conseguido desarrollar un prototipo IoT que detecta la presencia de vehículos y manda esa información a través de LoRa hacia el nodo de borde. En este punto, también pudimos proveer de seguridad y autenticación con credenciales únicas para cada nodo asegurando la información que se envía al cloud. Junto con lo anterior hemos desarrollado una aplicación móvil para la interacción del usuario con el sistema, proporcionando una experiencia fluida y efectiva como si se tratase de un producto profesional.

La aplicación móvil ha sido testeada en una variedad de dispositivos Android y emuladores, para poder demostrar su robustez en términos de comunicación y desempeño. La arquitectura en su conjunto ha revelado su versatilidad y capacidad para gestionar de manera eficiente las demandas de tráfico entrante en entornos de testeo.

Este proyecto destaca la eficacia de las plataformas tipo PaaS (Platform as a Service), las cuales ofrecen un entorno integral para la implementación de sistemas IoT. Estas plataformas solventan cuestiones técnicas y de seguridad, aseguran la conectividad de extremo a extremo, garantizan la calidad del servicio y posibilitan una escalabilidad sostenible a largo plazo. Además, abren la posibilidad de adoptar modelos de pago por uso en el futuro, lo que contribuiría a la optimización de los recursos y a la reducción de costos innecesarios.

No obstante, es crucial reconocer que la creación de un prototipo funcional ha conllevado desafíos sustanciales en términos de investigación, cálculos de batería e implementación. Para llevar esta iniciativa a la etapa de producto, es necesario continuar con estudios profundos, como la sustitución del microcontrolador principal por una alternativa de menor consumo energético y la optimización del diseño del PCB a través del empleo de chips de montaje superficial (SMD). Además, se requiere un análisis exhaustivo de los materiales para la selección adecuada de la carcasa del dispositivo, garantizando su resistencia ante posibles aplastamientos accidentales.

Por último, la ejecución de este proyecto nos permitió aplicar y reforzar conocimientos adquiridos a lo largo de la carrera, como son: programación en C, arquitectura de sistemas embebidos, conceptos de cloud computing vistos en materia como sistemas digitales avanzados, entre otros.
