# Diagnóstico Estratégico Integral para RappiPlus
Análisis para RappiPlus, un servicio del ecosistema Rappi diseñado para aumentar la frecuencia de compra y el valor generado por usuario.

## Datos: 
- Tres datasets con datos crudos trabajados con Python, dos tablas para análisis de la retención de cohortes trabajadas con SQL y un dataset para poder hacer un test estadístico con Python;

1. rappiplus_orders_raw.csv. Incluye los datos de las compras de los usuarios en 12 columnas que incluyen: id_pedido, id_usuario, fecha_hora_pedido, pais, dispositivo, fuente_referencia, nombre_producto, categoria_producto, cantidad, precio_unitario, monto_descuento y monto_total.
   
2. rappiplus_catalog.csv. Incluye el catálogo de productos que ofrece el servicio, sus respectivos proveedores y el costo que ofrece el proveedor sobre cada producto dividido en 4 columnas: nombre_producto, categoria_producto, costo_unitario y proveedor.

3. rappiplus_marketing_spend.csv. Incluye informacion sobre las campañas de marketing en cada país y sus costos para evaluar el impacto que tiene en las ventas y poder calcular la rentabilidad. Distribuido en 5 columnas: fecha, pais, id_campaña, canal y gasto.

4. users. Tabla con información de los usuarios para su posterior distinción por cohortes.
  
5. user_activity. Tabla para evaluar la actividad de los usuarios y calcular la retención de acuerdo a los que se mantienen activos con el tiempo.
  
6. experiment_checkout_ui.csv. Incluye la modificación en la UI para evaluar el impacto en la conversión de compra y  llevar a cabo el test estadístico.

## 📂 Contenido del repositorio

Diego-Sarinana/Diagnostico-Estrategico-Integral-RappiPlus - Para éste análisis se llevo a cabo el siguiente proceso: 
1. Carga de datos y vista rápida.
2. Revisión y calidad de datos.
3. Análisis de rentabilidad.
4. Creacion de funnel de conversión.
5. Cálculo de retención por cohortes.
6. Aplicación de test estadístico.
7. Comunicación de resultados.


## ▶ Cómo abrir el archivo en Google Sheets/Excel

1. Descarga el archivo dando clic al botón de 'Download raw file' tras haber abierto la sección del proyecto (Diego-Sarinana/Resumen-Ejecutivo-Ventas-Walmart)
2. En la herramienta de tu elección (Excel/Sheets) abra el archivo

O: Abre el siguiente enlace;
https://docs.google.com/spreadsheets/d/1te4De0QvxfNt20P3EwFDVfv6Tlh4OsLuODCQkebbqD8/edit?usp=sharing
  
## 📘 Cómo reproducir el análisis:
1. Tras abrir el archivo en la herramienta elegida puedes dar clic en las hojas de la barra inferior para revisar las modificaciones y resultados obtenidos
   
## 🧠 Objetivo del análisis:
1. Revelar si el servicio de RappiPlus está generando más ganancias. 
2. Identificar si los usuarios compran más
3. Encontrar oportunidades perdidas en el proceso de compra

## 🗣️Recomendación de negocio:
- Revisar los posibles outliers en los que ciertos clientes compraron 10,000 y 20,000 unidades ya que se están reflejando pérdidas probables de hasta 2,072,000.00 y ganancias probables de hasta 5,122,200.00 lo que pudiera significar una gran alerta o un gran éxito en el negocio.
- Enfocar la inversión a las "Laptop-Gaming-16GB" ya que es el producto con la mayor cantidad de ventas y de mayor margen de ganancia.
