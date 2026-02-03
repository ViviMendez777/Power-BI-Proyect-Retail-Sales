# Power-BI-Proyect-Retail-Sales
📊 Power BI Retail Sales Dashboard

📌 Resumen
Este proyecto transforma y visualiza las ventas de los últimos 3 años a partir de una planilla de Excel.
Se realiza un proceso de ETL básico (extracción, transformación y carga), modelado de datos en un esquema estrella y la construcción de un dashboard interactivo en Power BI

📑 Contenido
Descripción del origen
Estructura de datos y flujo de transformación
Modelo de datos (Esquema estrella)
Visualización y uso del dashboard
Archivos y enlaces
DAX
Créditos
Descripción del origen
Estructura de datos y flujo de transformación
Modelo de datos (Esquema estrella)
Visualización y uso del dashboard
Archivos y enlaces
Cómo contribuir
Créditos
1️⃣ Descripción del origen
Fuente: Planilla Excel de ventas (Sample - Superstore.xlsx).
Propósito: Analizar ventas de los últimos 3 años por producto, tienda, tiempo y cliente.
Herramientas:
Excel → archivo fuente.
Power BI → transformación, modelado y visualización.



2️⃣ Estructura de datos y flujo de transformación
Extracción:
Se toma la data directamente desde el archivo Excel fuente.
Transformación:
Limpieza de valores nulos e inconsistencias.
Normalización de formatos de fecha y unidades.
Enriquecimiento de datos con atributos derivados.
Carga y modelado:
Tablas cargadas en Power BI y organizadas en un modelo dimensional.
Flujo conceptual
Datos brutos (Excel) → Transformaciones → Modelo dimensional (estrella) → Dashboards



3️⃣ Modelo de datos (Esquema estrella)
Tabla de hechos:
Hechos_Ventas: métricas de ventas (importe, cantidad, descuento, costo, margen, fecha_id, producto_id, tienda_id, cliente_id, etc.).
Tablas dimensionales:
Dim_Tiempo: fecha_id, año, trimestre, mes, día.
Dim_Producto: producto_id, nombre_producto, categoría, precio_unitario, marca.
Dim_Tienda: tienda_id, nombre_tienda, ciudad, región, canal, formato.
Dim_Cliente: cliente_id, nombre_cliente, segmento, edad, sexo, comunidad.


4️⃣ Visualización y uso del dashboard
Descripción general:
Dashboard interactivo con filtros por año, trimestre, producto y tienda.
Visualizaciones típicas:
Ventas por periodo.
Ventas por producto.
Ventas por tienda.
Margen y tendencias.
Interacciones clave:
Filtros globales para periodo (3 años), producto, tienda y cliente.
Drill-down por mes o trimestre en la dimensión tiempo.


5️⃣ Archivos y enlaces
Archivo Excel fuente: Sample - Superstore.xlsx
Archivo Power BI PBIX): Descargar aquí
6️⃣ DAX
Calendario = CALENDAR(DATE(2014,01,03), DATE(2017,12,30))

MargenDeGanancia% = DIVIDE(SUM([Profit]), SUM([Sales]))

CantidadOrdenes = COUNT(Hechos[Order ID])

7️⃣ Créditos
Autor/a: Viviana Méndez
Fuente y recursos:
Planilla Excel de ventas original.
Power BI para ETL y visualización.
Contacto:
📧 Email: viviana.mendez2606@gmail.com 
🔗 LinkedIn: www.linkedin.com/in/viviana-mendez2606





