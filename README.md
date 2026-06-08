# Analisis de datos sobre el uso de IA en estudiantes universitarios

## Descripcion

Este proyecto fue realizado en Databricks Community Edition con el fin de poner en practica conceptos relacionados con almacenamiento, procesamiento y analisis de datos utilizando Apache Spark y SQL.

Para el desarrollo de la actividad se utilizo un dataset obtenido de Kaggle que contiene informacion sobre estudiantes universitarios y su relacion con herramientas de Inteligencia Artificial, incluyendo horas de uso, rendimiento academico, dependencia percibida y riesgo de burnout.

---

## Objetivos

* Diseñar un esquema de almacenamiento para el conjunto de datos.
* Cargar datos desde Kaggle en Databricks.
* Crear una tabla para almacenar la informacion.
* Realizar consultas utilizando Spark y SQL.
* Validar la calidad y consistencia de los datos.
* Comparar el uso de SQL y Spark para el analisis de datos.

---

## Dataset utilizado

El dataset contiene informacion relacionada con:

* Categoria academica del estudiante.
* Año de estudio.
* Promedio antes y despues del semestre.
* Horas semanales de uso de herramientas de IA.
* Nivel de dependencia hacia la IA.
* Diversidad de herramientas utilizadas.
* Riesgo de burnout.
* Politicas institucionales sobre el uso de IA.

---

## Tecnologias utilizadas

* Databricks Community Edition
* Apache Spark
* PySpark
* Spark SQL
* Kaggle

---

## Estructura de los datos

La entidad principal es **Estudiante**.

| Campo                      | Tipo    |
| -------------------------- | ------- |
| Student_ID                 | BIGINT  |
| Major_Category             | STRING  |
| Year_of_Study              | STRING  |
| Pre_Semester_GPA           | DOUBLE  |
| Weekly_GenAI_Hours         | DOUBLE  |
| Primary_Use_Case           | STRING  |
| Prompt_Engineering_Skill   | STRING  |
| Tool_Diversity             | INT     |
| Paid_Subscription          | BOOLEAN |
| Traditional_Study_Hours    | DOUBLE  |
| Perceived_AI_Dependency    | INT     |
| Institutional_Policy       | STRING  |
| Anxiety_Level_During_Exams | INT     |
| Post_Semester_GPA          | DOUBLE  |
| Skill_Retention_Score      | DOUBLE  |
| Burnout_Risk_Level         | STRING  |

---

## Proceso realizado

1. Diseño del esquema de almacenamiento.
2. Carga del archivo CSV en Databricks.
3. Creacion de la tabla `workspace.default.ai_student`.
4. Validacion del esquema mediante Spark y SQL.
5. Obtencion de estadisticas descriptivas.
6. Ejecucion de consultas SELECT, GROUP BY y filtros.
7. Comparacion de resultados entre Spark y SQL.

---

## Validaciones realizadas

### Metadatos

* DESCRIBE TABLE
* SHOW CREATE TABLE
* printSchema()

### Estadisticas descriptivas

* describe()
* COUNT()
* AVG()
* MIN()
* MAX()

### Consultas

* SELECT
* LIMIT
* WHERE
* GROUP BY

### Conteos

* Total de registros
* Verificacion de columnas
* Revision de muestras de datos

---

## SQL vs Spark

### Ventajas de SQL

* Sintaxis sencilla y facil de entender.
* Permite realizar consultas rapidamente.
* Es ideal para exploracion de datos.

### Desventajas de SQL

* Menor flexibilidad para procesos complejos.
* Limitado para analisis avanzados.

### Ventajas de Spark

* Permite trabajar con grandes volumenes de datos.
* Integra procesamiento distribuido.
* Se puede utilizar junto con Python.

### Desventajas de Spark

* Requiere mas conocimiento tecnico.
* El codigo suele ser mas extenso que en SQL.

---

## Conclusiones

Durante el desarrollo de la actividad fue posible cargar y procesar un conjunto de datos utilizando Databricks. Las validaciones realizadas permitieron comprobar que la informacion fue almacenada correctamente y que los resultados obtenidos mediante Spark y SQL fueron consistentes.

Ademas, se pudo observar que SQL es una buena opcion para consultas sencillas, mientras que Spark ofrece una mayor capacidad para trabajar con grandes cantidades de datos y procesos mas complejos.

---


Institucion Universitaria Digital de Antioquia
