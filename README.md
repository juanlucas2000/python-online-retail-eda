Online Retail II — Exploratory Data Analysis (EDA)

Análisis exploratorio de datos transaccionales de un mayorista de artículos de regalo con sede en el Reino Unido, con el objetivo de identificar patrones de ventas, productos top y mercados internacionales relevantes.

Dataset:  Online Retail II (UCI Machine Learning Repository, también disponible en Kaggle)
Tamaño: 1,067,371 transacciones, 8 columnas
Columnas: Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country


Proceso de limpieza
Cancelaciones: 19,494 No son ventas reales

Cantidad ≤ 0 (no marcadas como cancelación): 3,456

Precio ≤ 0 :6,207 Productos promocionales o muestras gratuitas, sin ingreso real

Duplicados exactos: 34,335 repetidos sin información nueva.

Filas finales: 1,007,913


Decisión documentada: se conservaron las filas sin Customer ID, ya que no afectan el análisis de ingresos y ventas generales.


Insights principales

Ingreso total: £20,476,260.45

Estacionalidad atípica: el pico de ventas ocurre en octubre, no en diciembre. Este es un patrón característico de un negocio B2B: los clientes (muchos revendedores) hacen sus pedidos grandes con anticipación para tener stock antes de la temporada navideña, en lugar de comprar durante la temporada misma.

Productos top: liderados por artículos de decoración para el hogar y temporada navideña — Regency Cakestand 3 Tier, White Hanging Heart T-Light Holder, Paper Chain Kit 50's Christmas, Rotating Silver Angels T-Light Holder — consistente con el perfil de mayorista de regalos y decoración.

Mercados internacionales top (excluyendo UK): EIRE (Irlanda), Países Bajos y Alemania — mercados geográficamente cercanos al Reino Unido con fuerte actividad de comercio B2B.


Herramientas


Python (pandas, matplotlib)
Jupyter / VS Code
