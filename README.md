[MAPA MENTAL](https://jpiedramacas.github.io/EXAM-Mod2/mapa_mental.html)

#### Resumen del Curso: Programador de Sistemas AWS - Módulo 2

### Introducción al Ciclo de Vida del Software
El ciclo de vida del software es una estructura utilizada para planificar y controlar el proceso de desarrollo de un sistema de información. Los modelos de ciclo de vida del software proporcionan una metodología para mejorar la calidad del software y la administración del proyecto. Se dividen en dos grandes categorías: modelos prescriptivos y modelos adaptativos.

# Modelos del Ciclo de Vida del Software:

## Modelo en Cascada
El modelo en cascada es un enfoque lineal y secuencial donde el progreso fluye en una sola dirección hacia abajo como una cascada a través de las fases de análisis, diseño, implementación, pruebas, despliegue y mantenimiento.
![Modelo en Cascada](assets/modelo%20de%20cascada.jpg)
- **Fases**:
  - **Pre Análisis**: Identificación de la necesidad del proyecto y su viabilidad.
  - **Análisis**: Recolección y documentación de requisitos.
  - **Diseño**: Especificación de la arquitectura y componentes del sistema.
  - **Desarrollo**: Codificación del software según el diseño.
  - **Pruebas**: Verificación y validación del software.
  - **Implantación**: Despliegue del software en el entorno de producción.
  - **Mantenimiento**: Corrección de errores y mejoras.

- **Ventajas**:
  - Estructura clara y sencilla de entender y usar.
  - Fácil gestión debido a su rigidez y fases bien definidas.

- **Desventajas**:
  - No es adecuado para proyectos donde los requisitos cambian frecuentemente.
  - Dificultad para volver a fases anteriores sin afectar las siguientes.

## Modelo Iterativo
El modelo iterativo se basa en la repetición de un conjunto de actividades durante cada iteración, permitiendo mejoras y refinamientos sucesivos del sistema.
![Modelo Iterativo](assets/Modelo%20Iterativo.jpg)
- **Características**:
  - Desarrollos en ciclos repetitivos.
  - Retroalimentación continua y ajustes basados en pruebas y evaluación del cliente.

- **Beneficios**:
  - Identificación temprana de problemas.
  - Mayor flexibilidad y adaptación a cambios en los requisitos.

## Modelo Incremental
El modelo incremental combina elementos del modelo en cascada con el enfoque iterativo. Se desarrolla una versión básica del software y, en incrementos sucesivos, se añaden funcionalidades adicionales.
![Modelo Incremental](assets/Modelo%20Incremental.jpg)

- **Diferencia con Iterativo**:
  - Cada iteración añade una funcionalidad completa al producto, en lugar de mejorar continuamente todo el sistema.

- **Beneficios**:
  - Permite la entrega progresiva de partes funcionales del software.
  - Proporciona mayor estabilidad y confiabilidad del sistema con cada incremento.

## Modelo en V
El modelo en V es una extensión del modelo en cascada que enfatiza la verificación y validación en cada fase de desarrollo.
![Modelo en V](assets/Modelo%20en%20V.png)

- **Fases**:
  - **Planificación y Análisis**: Similar al modelo en cascada.
  - **Diseño de Sistema y Arquitectura**: Especificaciones detalladas de la arquitectura.
  - **Diseño de Módulo y Detalles**: Detallado de componentes individuales.
  - **Implementación**: Codificación de módulos.
  - **Pruebas Unitarias, Integración y de Sistema**: Validación y verificación de cada componente y del sistema completo.

- **Ventajas**:
  - Asegura la calidad mediante pruebas rigurosas.
  - Las pruebas tempranas reducen el costo de errores posteriores.

## Modelo Basado en Componentes (CBSE)
El desarrollo basado en componentes se enfoca en la reutilización de módulos existentes con interfaces definidas y claramente especificadas.

![CBSE](assets/Modelo%20Basado%20en%20Componentes%20(CBSE).png)

- **Enfoque**:
  - Descomposición del sistema en componentes funcionales que pueden ser desarrollados de forma independiente.

- **Beneficios**:
  - Reducción de tiempo y costos al reutilizar componentes.
  - Mejora la calidad al usar módulos probados previamente.

- **Desafíos**:
  - Integración de componentes heterogéneos.
  - Garantizar la compatibilidad y la cohesión del sistema.

## Modelo de Desarrollo Rápido (RAD)
El RAD es un modelo que enfatiza el desarrollo rápido mediante prototipos y un enfoque iterativo con entregas rápidas.
![RAD](assets/Modelo%20de%20Desarrollo%20Rápido%20(RAD).png)

- **Fases**:
  - **Modelado de Gestión**: Identificación de requisitos a nivel de negocio.
  - **Modelado de Datos**: Diseño de estructuras de datos.
  - **Modelado de Proceso**: Diseño de procesos de negocio.
  - **Generación de Aplicaciones**: Desarrollo del software a partir de modelos.
  - **Pruebas de Entrega**: Validación de prototipos.

- **Ventajas**:
  - Desarrollo rápido y respuesta eficiente a cambios.
  - Alta visibilidad y retroalimentación constante del cliente.

- **Desventajas**:
  - Riesgo de producir prototipos que no se ajustan al producto final.
  - Posible incremento en el costo de cambios frecuentes.

### Metodologías Ágiles
Las metodologías ágiles son un conjunto de principios para el desarrollo de software que valoran la flexibilidad, la colaboración y la entrega continua de valor al cliente.

- **Agile**: Se centra en adaptarse a los cambios rápidos y la entrega continua de software funcional.

- **Principios Fundamentales**:
  1. Entrega temprana y continua de software valioso.
  2. Bienvenida a cambios de requisitos, incluso en etapas tardías.
  3. Entregas frecuentes de software funcional, con preferencia por períodos cortos.
  4. Colaboración constante entre el equipo de desarrollo y el cliente.
  5. Proyectos construidos en torno a individuos motivados, con apoyo y confianza.
  6. Comunicación cara a cara como la forma más eficiente de transmitir información.
  7. Software funcionando como principal medida de progreso.
  8. Promoción del desarrollo sostenible, manteniendo un ritmo constante.
  9. Atención continua a la excelencia técnica y buen diseño.
  10. Simplicidad como arte de maximizar la cantidad de trabajo no realizado.
  11. Equipos autoorganizados que generan las mejores arquitecturas, requisitos y diseños.
  12. Adaptación regular a circunstancias cambiantes, ajustando el comportamiento del equipo.

## Metodología Scrum

**Scrum** es una metodología ágil que se enfoca en la entrega incremental de valor en proyectos de desarrollo de software. Se basa en un marco de trabajo iterativo y colaborativo, estructurado en roles, artefactos y eventos específicos.

![Scrum](assets/ScrumPoster.png)

#### Roles en Scrum

1. **Product Owner (PO)**:
   - **Gestión del Product Backlog**: Responsable de priorizar y gestionar esta lista de funcionalidades y requisitos.
   - **Definición de Requisitos**: Colabora con stakeholders para definir y priorizar las necesidades del producto.
   - **Toma de Decisiones**: Decide qué funcionalidades incluir en cada sprint.
   - **Representación del Cliente**: Actúa como la voz del cliente, asegurando que se cumplan sus necesidades.
   - **Participación en Eventos de Scrum**: Participa en las reuniones clave, proporcionando orientación y feedback 【3†source】.

2. **Scrum Master**:
   - **Facilitador del Proceso Scrum**: Ayuda al equipo a seguir las reglas y procesos de Scrum.
   - **Eliminador de Impedimentos**: Identifica y elimina obstáculos que afectan el progreso del equipo.
   - **Coach del Equipo**: Enseña y guía al equipo en la aplicación de Scrum, promoviendo prácticas ágiles .

3. **Equipo de Desarrollo**:
   - **Multidisciplinario y Autoorganizado**: Posee todas las habilidades necesarias para entregar incrementos de valor.
   - **Responsable de la Entrega del Producto**: Trabaja en ciclos iterativos para completar las tareas del sprint .

#### Artefactos de Scrum

1. **Product Backlog**: Lista priorizada de todo el trabajo por hacer en el proyecto, gestionada por el PO.
2. **Sprint Backlog**: Conjunto de elementos del Product Backlog seleccionados para ser trabajados en el sprint actual.
3. **Incremento**: Resultado del trabajo realizado durante un sprint, que debe ser una versión potencialmente entregable del producto  .

#### Eventos de Scrum

1. **Sprint**: Periodo de trabajo de 1 a 4 semanas donde se completa un incremento de producto.
2. **Reunión de Planificación del Sprint**: Definición de los objetivos y la planificación del trabajo del sprint.
3. **Daily Scrum**: Reunión diaria de 15 minutos para sincronizar actividades y discutir impedimentos.
4. **Revisión del Sprint**: Evaluación del incremento desarrollado y recepción de feedback de los stakeholders.
5. **Retrospectiva del Sprint**: Reflexión sobre el proceso del sprint y discusión de mejoras continuas 【3†source】 .

#### Beneficios de Scrum

1. **Mayor Transparencia y Adaptabilidad**:
   - Proporciona una visión clara del progreso del proyecto a través de artefactos como el Product Backlog y el Sprint Backlog.
   - Facilita la adaptación a los cambios en los requisitos del cliente o del mercado  .

2. **Entrega Temprana de Valor y Satisfacción del Cliente**:
   - Permite la entrega frecuente de funcionalidades priorizadas, obteniendo retroalimentación continua del cliente.
   - Mejora la satisfacción del cliente al desarrollar productos que realmente agregan valor  .

#### Desafíos de Scrum

1. **Resistencia al Cambio**:
   - Equipos y organizaciones acostumbrados a métodos tradicionales pueden mostrar resistencia a adoptar Scrum.
   - La transición hacia una cultura ágil requiere un cambio de mentalidad significativo  .

2. **Complejidad en la Gestión de Equipos y Stakeholders**:
   - Roles y responsabilidades claras pueden ser desafiantes de gestionar en equipos grandes o distribuidos.
   - La gestión de múltiples stakeholders con diferentes expectativas añade complejidad adicional al proceso  .

#### Escalado de Scrum

1. **Scrum of Scrums**: Coordinación entre múltiples equipos Scrum mediante representantes que se reúnen regularmente.
2. **SAFe (Scaled Agile Framework)**: Proporciona una estructura para escalar Scrum a nivel empresarial, con roles y eventos adicionales.
3. **LeSS (Large-Scale Scrum)**: Framework minimalista que se enfoca en la simplicidad y la colaboración entre múltiples equipos.

