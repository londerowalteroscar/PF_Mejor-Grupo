### Proyecto "FindEden"

#### Descripción del Proyecto
El proyecto "FindEden" tiene como objetivo desarrollar una aplicación que recomiende a los usuarios los mejores lugares para alquilar o comprar propiedades, utilizando datos de diversas fuentes y técnicas avanzadas de machine learning. La aplicación permitirá a los usuarios seleccionar las características que valoran en una vivienda y, basándose en esos filtros, determinará las mejores ubicaciones disponibles. El producto será vendido a empresas inmobiliarias, facilitando a sus clientes encontrar su vivienda ideal.

#### Objetivos
1. Recomendar los mejores lugares para vivir basado en preferencias y características especificadas por el usuario.
2. Mejorar la experiencia del usuario ofreciendo recomendaciones personalizadas que cumplan con sus expectativas.
3. Optimizar la gestión de propiedades proporcionando a las inmobiliarias con insights valiosos para reducir tiempos de vacancia y aumentar la satisfacción del inquilino.

### Alcance del Proyecto
- Desarrollo de una aplicación interactiva de recomendación de viviendas.
- Integración de técnicas de machine learning para personalizar las recomendaciones.
- Uso de AWS para almacenamiento de datos y modelado de machine learning.
- Implementación de un dashboard interactivo para visualización de datos.
- Venta del producto a empresas inmobiliarias para mejorar su servicio al cliente.

### Stack Tecnológico e Implementación

#### Tecnologías Locales:
- **Python:** Para limpieza de datos y desarrollo de modelos de machine learning.
- **Jupyter Notebooks:** Para exploración de datos y desarrollo de modelos.
- **Pandas, NumPy, Scikit-Learn:** Para análisis y modelado de datos.

#### Tecnologías en la Nube (AWS):
- **Amazon S3:** Para almacenamiento de datos sin procesar y resultados procesados.
- **Amazon Redshift:** Para almacenamiento y análisis de datos estructurados.
- **Amazon SageMaker:** Para construir, entrenar y desplegar modelos de machine learning.
- **Amazon QuickSight:** Para visualización y creación de dashboards interactivos.

### Implementación del Stack Tecnológico

1. **Almacenamiento de Datos:**
   - **Amazon S3:** Almacenar datos sin procesar y resultados procesados.
   - **Amazon Redshift:** Configurar y mantener un Data Warehouse para almacenamiento y análisis de datos estructurados.

2. **Preparación y Transformación de Datos:**
   - Realizar limpieza y preparación de datos localmente usando Python, Pandas y NumPy.
   - Transferir datos limpios a Amazon Redshift para análisis adicional.

3. **Desarrollo de Modelos de Machine Learning:**
   - Utilizar Jupyter Notebooks localmente para exploración y desarrollo inicial de modelos.
   - Entrenar y desplegar modelos en Amazon SageMaker.

4. **Visualización y Dashboards:**
   - Crear visualizaciones y dashboards interactivos en Amazon QuickSight para mostrar las recomendaciones y análisis de datos.

### Metodología de Trabajo

Se utilizará **Scrum** como metodología ágil para asegurar una entrega eficiente, colaborativa y adaptable a cambios.

#### Principales Eventos de Scrum:
- **Sprint Planning:** Planificación del trabajo a realizar en el sprint.
- **Daily Stand-up:** Reuniones diarias para revisar el progreso y resolver bloqueos.
- **Sprint Review:** Revisión del trabajo completado al final del sprint.
- **Sprint Retrospective:** Evaluación del proceso y definición de mejoras para el siguiente sprint.

### Diseño Detallado

1. **Interfaz de Usuario:**
   - Filtros para que los usuarios seleccionen sus preferencias (e.g., tipo de propiedad, presupuesto, características deseadas).
   - Visualización de recomendaciones basadas en los filtros seleccionados.

2. **Backend y Almacenamiento:**
   - Procesamiento y almacenamiento de datos en Amazon Redshift.
   - Utilización de Amazon S3 para almacenamiento de datos sin procesar.

3. **Modelos de Machine Learning:**
   - Desarrollo de modelos en Jupyter Notebooks.
   - Entrenamiento y despliegue en Amazon SageMaker.

4. **Visualización:**
   - Dashboards interactivos creados en Amazon QuickSight para mostrar resultados y recomendaciones.

### Equipo de Trabajo - Roles y Responsabilidades

1. **Product Owner (PO):**
   - Define características y prioridades del producto.
   - Gestiona y prioriza el backlog del producto.

2. **Scrum Master (SM):**
   - Facilita el proceso Scrum y asegura adherencia a prácticas ágiles.
   - Elimina obstáculos que puedan afectar el progreso del equipo.

3. **Data Engineers (2):**
   - Configuran y mantienen sistemas de almacenamiento y procesamiento de datos.
   - Desarrollan pipelines de datos en AWS Glue.

4. **Data Scientist (1):**
   - Prepara datos y desarrolla modelos de machine learning en Amazon SageMaker.
   - Optimiza modelos para obtener mejores resultados.

5. **Data Analysts (2):**
   - Realizan análisis exploratorio de datos (EDA) y crean visualizaciones en Amazon QuickSight.
   - Generan informes y presentaciones basados en los análisis.

### KPI’s

1. **Tiempo promedio de vacancia de inmuebles**
   - **Categoría:** Indicador de ocupación
   - **Fuente de datos:** Datos históricos del estado de California y base de datos interna.
   - **Descripción:** Evalúa la eficiencia y rentabilidad de una propiedad mediante el tiempo que permanece vacante.
   - **Meta:** Mantenerse por debajo del promedio de vacancia general semestral del estado de California.
   - **Cálculo:** 
     \[
     \text{TPV (Tiempo promedio de vacancia)} = \frac{\text{Duración de periodos de vacancia}}{\text{Número total de propiedades evaluadas}}
     \]

2. **Índice de renovación de contratos (IRC)**
   - **Categoría:** Indicador de gestión
   - **Fuente de datos:** Base de datos interna de nuestro sistema y encuestas de satisfacción a inquilinos.
   - **Descripción:** Mide la proporción de contratos de arrendamiento que se renuevan en un período determinado.
   - **Meta:** Mantenerse al menos un 10% por encima del IRC promedio anual del estado de California.
   - **Cálculo:** 
     \[
     \text{Índice de renovación de contratos} = \frac{\text{N contratos renovados}}{\text{N total de contratos}} \times 100
     \]

3. **Índice de expectativa satisfecha (IES) del inquilino**
   - **Categoría:** Indicador de satisfacción del inquilino
   - **Fuente de datos:** Encuesta de satisfacción de inquilinos al finalizar sus contratos.
   - **Descripción:** Refleja el grado en que el sistema de recomendación cumple con las expectativas de los usuarios.
   - **Meta:** Mantenerse por encima de los 7 puntos y tener como máximo una disminución de -10% respecto al año anterior.
   - **Cálculo:** 
     \[
     \text{IES} = \frac{\text{Puntuaciones de satisfacción de los inquilinos}}{\text{Número total de puntuaciones de satisfacción de los inquilinos}}
     \]

### Cronograma General - Diagrama de Gantt

| Fase                      | Duración  | Semana 1 | Semana 2 | Semana 3 | Semana 4 | Semana 5 | Semana 6 | Semana 7 | Semana 8 | Semana 9 | Semana 10 |
|---------------------------|-----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|-----------|
| Sprint 0 (Preparación)    | 1 semana  | X        |          |          |          |          |          |          |          |          |           |
| Sprint 1                  | 2 semanas |          | X        | X        |          |          |          |          |          |          |           |
| Sprint 2                  | 2 semanas |          |          |          | X        | X        |          |          |          |          |           |
| Sprint 3                  | 2 semanas |          |          |          |          |          | X        | X        |          |          |           |
| Sprint 4                  | 2 semanas |          |          |          |          |          |          |          | X        | X        |           |
| Sprint 5                  | 2 semanas |          |          |          |          |          |          |          |          |          | X         |

Este cronograma se adapta a un marco de trabajo ágil, permitiendo iteraciones y entregas incrementales del producto, garantizando flexibilidad y capacidad de respuesta a cambios en los requisitos del cliente.

---

Este esquema cubre todos los aspectos necesarios para llevar a cabo el proyecto "FindEden" de manera estructurada y eficiente, utilizando una combinación de herramientas locales y servicios en la nube de AWS.