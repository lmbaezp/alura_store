# README - Análisis de AluraStore

## Descripción del Proyecto
Este proyecto consiste en un análisis detallado del desempeño de las cuatro tiendas de AluraStore. El objetivo principal es evaluar métricas clave como facturación, ventas por categoría de productos, productos más y menos vendidos, calificaciones de los clientes y costos promedio de envíos. El análisis busca identificar la tienda con menor rendimiento para considerar su posible cierre, con el fin de optimizar las finanzas de la empresa.

## Estructura del Repositorio
- **Informe_AluraStore.pdf**: Documento detallado que contiene el análisis completo, gráficos y conclusiones.
- **Notebooks/**: 
  - `AluraStoreLatam.ipynb`: Notebook de Google Colab con el código utilizado para el análisis.
- **Data/**: 
  - Archivos de datos de las cuatro tiendas (si están disponibles en el repositorio).

## Métricas Analizadas
1. **Facturación**:
   - Porcentaje de recaudo por ventas por tienda.
   - Número de ventas anuales y trimestrales.
   - Ganancias por ventas discriminadas por año y trimestre.

2. **Ventas por Categoría de Productos**:
   - Mapa de calor de ventas por categoría y tienda.
   - Recaudo por categoría de productos.

3. **Productos Más y Menos Vendidos**:
   - Productos con mayor y menor volumen de ventas.
   - Productos con mayor y menor recaudo por tienda.

4. **Calificaciones de las Tiendas**:
   - Promedio de calificaciones por tienda.
   - Evolución de las calificaciones a lo largo del tiempo.

5. **Costo Promedio de Envíos**:
   - Promedio del costo de envío por tienda.
   - Porcentaje del recaudo total que representa el costo de envíos.

### Metodología de Análisis
- **Limpieza y preparación de datos**:
  - Exclusión del año 2023 para análisis anuales (debido a datos incompletos).
  - Validación de registros faltantes (ej: Tienda 4 tenía 1 venta menos que las demás).
  - Normalización de formatos (fechas, categorías, métodos de pago).

- **Enfoque temporal**:
  - Análisis anual (2020–2022) para tendencias a largo plazo.
  - Análisis trimestral (incluyendo Q1-2023) para patrones estacionales.

- **Métricas clave calculadas**:
  - **Facturación**: Recaudo total, margen bruto (precio - costo de envío).
  - **Desempeño por categoría**: Ventas unitarias vs. ingresos generados.
  - **Eficiencia logística**: Costo de envío como porcentaje del recaudo (5.33% para todas las tiendas).

## Hallazgos Principales
#### ¡Recuerda que todo el análisis se encuentra en el docuemnto Informe_AluraStore.pdf!
- **Tienda 4**: Presenta el menor recaudo total, una disminución constante en ventas y calificaciones, y un bajo desempeño en productos más vendidos.
- **Tienda 3**: Aunque inicialmente tuvo un declive en 2021, mostró una recuperación significativa en 2022, mejorando en ventas y calificaciones.
- **Tienda 1**: Destaca por su alto recaudo y estacionalidad en ventas, aunque con una caída en 2022.
- **Tienda 2**: Muestra un comportamiento estable, con crecimiento en ganancias a pesar de una disminución en ventas en 2022.

## Conclusiones y Recomendaciones
Basado en el análisis, **la Tienda 4 es la candidata principal para ser cerrada**, debido a su bajo recaudo, disminución constante en ventas y calificaciones, y bajo desempeño en productos clave. Las demás tiendas muestran tendencias positivas o estables que justifican su continuidad.

## Limitaciones
- **Datos incompletos**: El año 2023 solo incluye Q1, lo que limita el análisis anual.
- **Variables no consideradas**:
  - No se analizó el impacto del "método de pago" en las ventas.
  - Falta información externa (ej: campañas publicitarias por tienda).

## Instrucciones para Ejecutar el Código
1. **Requisitos**:
   - Python 3.x
   - Bibliotecas: Pandas, Matplotlib, Seaborn, NumPy.
   - Google Colab (opcional, si se desea ejecutar en la nube).

2. **Pasos**:
   - Abrir el notebook `AluraStoreLatam.ipynb` en Google Colab o en un entorno local con Jupyter.
   - Ejecutar las celdas en orden secuencial para evitar errores.
   - Asegurarse de que los archivos de datos estén en la ruta correcta (especificada en el notebook).
