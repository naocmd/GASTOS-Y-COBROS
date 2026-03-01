# PRESUPUESTO_PERSONAL

# Descripción del Proyecto

Presupuesto Personal es un sistema de base de datos relacional diseñado para gestionar ingresos, gastos y presupuestos mensuales de forma estructurada y escalable.

El proyecto combina:

🗄️ Diseño y modelado de base de datos en MySQL

🔐 Integridad referencial y restricciones

📊 Visualización y análisis de datos con Power BI

El objetivo es simular un entorno real de gestión financiera y análisis empresarial.

# Objetivos del Proyecto

Diseñar una base de datos normalizada (3FN)

Aplicar buenas prácticas de modelado relacional

Implementar claves primarias, foráneas y restricciones CHECK

Garantizar integridad y coherencia de los datos

Explorar análisis y visualización de datos con Power BI

Simular un flujo real: Base de Datos → Análisis → Dashboard

# Modelo de Datos

📌 Tablas principales

Tabla	Descripción
EMPRESAS	Entidades asociadas a ingresos y gastos
FUENTEINGRESOS	Clasificación del origen del ingreso
CATEGORIA	Clasificación de los gastos
GASTOS	Registro detallado de gastos
INGRESOS	Registro detallado de ingresos
PRESUPUESTO	Presupuesto mensual por categoría y empresa

🔗 Relaciones

Una empresa puede tener múltiples ingresos y gastos.

Cada gasto pertenece a una categoría.

Cada ingreso pertenece a una fuente de ingreso.

El presupuesto se asigna por empresa y categoría.

Todas las relaciones están protegidas mediante claves foráneas.

🔐 Restricciones Implementadas

✔️ PRIMARY KEY en todas las entidades
✔️ FOREIGN KEY para integridad referencial
✔️ UNIQUE para evitar duplicados
✔️ CHECK para validación de datos:

Tipo de gasto → FIJO / VARIABLE

Tipo de fuente → FIJO / EXTRA

Método de pago → EFECTIVO / TARJETA

# Análisis y Visualización con Power BI

Este proyecto incluye una fase de análisis mediante Power BI, conectando la base de datos MySQL para crear dashboards interactivos.

# Métricas Analizadas

Total de ingresos mensuales

Total de gastos mensuales

Balance mensual

Distribución de gastos por categoría

Comparación Presupuesto vs Gasto Real

Gastos fijos vs variables

Ingresos fijos vs extras

# Visualizaciones Incluidas

Gráfico de barras → Gastos por categoría

Gráfico de líneas → Evolución mensual

KPI Cards → Balance mensual

Tabla dinámica → Detalle por empresa

Segmentadores (filtros) por fecha y tipo

# Flujo del Proyecto
Diseño SQL → Creación de datos → Modelado relacional → 
Conexión Power BI → Transformación de datos → Dashboard interactivo
🛠️ Tecnologías Utilizadas

MySQL

SQL

Power BI

Git

GitHub

# Estructura del Repositorio
/presupuesto_personal
│── schema.sql
│── data.sql
│── presupuesto_powerbi.pbix
│── README.md
│── modelo_relacional.png
│── dashboard_preview.png
