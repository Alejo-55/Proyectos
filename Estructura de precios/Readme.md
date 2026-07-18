# Análisis de Precios y Rentabilidad — Simulación Tienda de Conveniencia

Proyecto de práctica de análisis de precios, construido con excel y Power BI. Aplicando conceptos de economía (elasticidad precio-demanda, margen de contribución). A un dataset simulado con productos de una tienda conveniencia en una gasolinera.


## Descripción del proyecto

Este proyecto simula las estryuctura de precios y rentabilidad de 15 productos (bebidas, snacks, tabaco, comida rápida, automotriz y combustible). Segmentadas en 8 categorías de producto. El objetivo fue construir de principio a fin, un flujo de análisis de precios: cálculo de márgenes, utilidades, elasticidades, clasificación de productos, simulación de escenarios ante cambio en los precios, fenómeno normal enn los mercados. Y también construir una visualización de resultados en un dashboard intercativo.


## Objetivo

Responder a una pregunta central de negocio: ¿Qué productos son realemente rentables para una empresa de esta categoría, y cómo respondería la utilidad total ante un cambio en los precios de mercado?


## Metodología
#### Datos:
Dataset simulado con 15 productos básicos en una tienda comveniencia, con precio, costo unitario, unidades vendidas y costo fijo asignado (prorroteado por renta, servicios públicos).
#### Herramientas:
Excel(Cálculos base, fórmulas, búsqueda, clasificación condicional) y Power BI (Modelado de datos, construcción de medidas DAX, visualizaciones).
#### Supuestos:
Se evaluó el efecto que un incremento del 10% en precio para todos(15) los productos de la tienda tiene sobre la utilidad neta de la empresa. Usando una elasticidad asumida por categoría de producto en base a teoría económica y lógica de negocio (no estimadas estadísticamente, véase la sección de limitaciones).


## Conceptos Aplicados

#### Margen vs Markup:
Porcentaje de ganancia obtenido sobre el precio de venta. Markup es el porcentaje que se agrega al costo para poder llegar al precio de venta.
#### Margen de contribución y punto de equilibrio:
El margen de contribución (Precio - Costo Unitario) indica cuanto aporta cada unidad vendida para cubrir los costos antes de generar la ganancia real. El punto de equilibrio (costo fijo/margen de contribución) indica cuántas unidades se necesitan vender para cubrir esos costos fijos.
#### Margen x Volumen:
Utilidad Total de un producto depende de dos factores, márgen por unidad y el volumen de ventas. Un margen alto, no garantiza utilidad alta si el volumen de unidades vendidas es bajo. Antaño, un margen bajo, no garantiza utilidad baja si el volumen de unidades vendidas es alto, y siempre, dependiendo del tipo de producto o servicios, qué tipo es y su elasticidad.

#### Productos de atracción:
En este caso, el conbustible funciona como producto de "enganche" para atraer a los clientes a la tienda conveniencia. El bajo mergen se ve compensado por el alto volumen de unidades vendidas y a que el producto es muy insensible a cambios en el precio DE MERCADO.

#### Elasticidad precio de la demanda: 
Mide qué tan sensible es la cantidad demandada de un bien o servicio entorno al precio de mercado.En la literatura existen tres conceptos que se clasfican su definición de la siguiente manera: Si es mayor a 1, se dice que es elástica (muy sensible al precio), si es igual a 1 (sensible al precio) o sensibilidad unitaria, si es menor a 1 es insensible al precio. Los coeficientes de la misma se asignaron por categoría y en base a la necesidad del bien, disponibilidad de sustititutos cercanos, frecuencia de compra, etc.




## Hallazgos principales


## Herramientas y técnicas aplicadas
[Excel: BUSCARX, SUMAR.SI... | Power BI: DAX, SUMX... | Conceptos económicos: elasticidad, margen ponderado...]

## Limitaciones
[Datos simulados, elasticidad asumida por categoría no por producto, etc.]

## Capturas del dashboard
[Imágenes]
