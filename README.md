# Power-BI-Proyect-Retail-Sales
Power BI Retail Sales Dashboard

Proyecto: Dashboard de Ventas al Detalle basado en una planilla de Excel y desarrollado en Power BI.

Resumen
Este proyecto transforma y visualiza las ventas de los últimos 3 años a partir de una planilla de Excel. Se realiza ETL básico (extracción, transformación y carga), modelado de datos en un esquema estrella y la construcción de un dashboard interactivo en Power BI.


Contenido
Descripción del origen
Estructura de datos y flujo de transformación
Modelo de datos (Esquema estrella)
Visualización y uso del dashboard
Archivos y enlaces

Cómo contribuir

Créditos
1) Descripción del origen
Fuente: Planilla Excel de ventas (Sample - Superstore.xlsx).
Propósito: Analizar ventas de los últimos 3 años por producto, tienda, tiempo y cliente.
Herramientas: Excel para la planilla original, Power BI para la transformación y visualización.
2) Estructura de datos y flujo de transformación
Extracción:
Se toma la data directamente desde el archivo Excel fuente.
Transformación:
Limpieza de valores nulos e inconsistencias.
Normalización de formatos de fecha y unidades.
Enriquecimiento de datos con atributos derivados.
Carga y modelado:
Se cargan las tablas en un modelo de datos en Power BI.
Flujo conceptual:
Datos brutos (Excel) → Transformaciones → Modelo dimensional (estrella) → Dashboards
3) Modelo de datos (Esquema estrella)
Tabla de hechos:
Hechos_Ventas: métricas de ventas (importe, cantidad, descuento, costo, margen, fecha_id, producto_id, tienda_id, cliente_id, etc.).
Tablas dimensionales:
Dim_Tiempo: fecha_id, año, trimestre, mes, día, etc.
Dim_Producto: producto_id, nombre_producto, categoría, precio_unitario, marca, etc.
Dim_Tienda: tienda_id, nombre_tienda, ciudad, región, canal, formato.
Dim_Cliente: cliente_id, nombre_cliente, segmento, edad, sexo, comunidad.
Esquema:
Hechos_Ventas ←→ Dim_Tiempo (a través de fecha_id)
Hechos_Ventas ←→ Dim_Producto (a través de producto_id)
Hechos_Ventas ←→ Dim_Tienda (a través de tienda_id)
Hechos_Ventas ←→ Dim_Cliente (a través de cliente_id)
4) Visualización y uso del dashboard
Descripción general:
Dashboard interactivo con filtros por año, trimestre, producto y tienda.
Visualizaciones típicas: ventas por periodo, por producto, por tienda, margen y tendencias.
Interacciones clave:
Filtros globales para periodo (3 años), producto, tienda y cliente.
Drill-down por mes o trimestre en la dimensión tiempo.

Requisitos:
Power BI Desktop (o servicio Power BI para compartir).
Archivos de origen: la planilla Excel y el archivo PBIX con el modelo y las visualizaciones.
Mantenimiento:
Al actualizar Excel, actualizar la conexión y refrescar el modelo en Power BI.
6) Archivos y enlaces
Archivo de Excel fuente: Sample - Superstore.xlsx
Archivo Power BI (PBIX): https://drive.google.com/file/d/1-JjpXGrMxObTz8ADpe704-HuU51CY6Ai/view?usp=drive_link (El archivo debe descargarse para poder visualizar)

7) Cómo contribuir
Pasos sugeridos:
Clonar el repositorio.
Abrir el archivo Power BI (.pbix) y revisar el Modelo de datos y las visualizaciones.
Verificar la fuente de datos y actualizar el Excel si es necesario.
Realizar ajustes en el esquema dimensional si cambian las dimensiones o hechos.
Documentar cualquier cambio en el README y en las notas de versión.
Reglas de estilo:
Nombres consistentes para tablas y columnas.
Documentar transformaciones clave en una sección de Transformaciones del README.

9) Créditos
Autor/es: DataSet
Protagonistas:
Viviana Méndez — Aportaciones y revisión (créditos)
Fuente y recursos:
Planilla Excel de ventas original.
Power BI para ETL y visualización.
Agradecimientos: equipo/compañeros que colaboraron.


