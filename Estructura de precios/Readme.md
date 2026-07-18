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

#### 1. Margen alto no garantiza utilidad alta
Café pequeño tiene margen alto pero utilidad baja (poca influencia en la utilidad total). Combustible tiene margen bajo pero genera bastante utilidad (alta incidencia en la utilidad total).

#### 2. El combustible cumple un rol estratégico, no solo financiero
Actúa como producto de atracción de tráfico de clientes hacia la tienda.

#### 3. Un aumento de precio, genera un incremento de utilidad, incluso perdiendo volumen de unidades totales vendidas en toda la tienda.
Al simular un incremento del 10% del precio en todo el portafolio de la tienda. Al simular el incremento de precios, la utilidad total neta subió de aprox L129,340 a L199,640, incrementándose en L70,300. A pesar de una pérdida estimada de 723 unidades del total de productos en venta. Esto ocurre porque el margen porque el precio incrementa el margen por unidad en todos los productos, y en productos inelásticos como combustible, casi no se pierden unidades, en relación a otros productos.

### 4. Matiz estratégico de la matemática: 
Aunque el modelo sugiere que subir precios en productos inelásticos genera mayor utilidad. El combustible, al ser un bien necesario o escencial en sociedades tradicionales, es un bien o producto muy comparado entre los compradores ya que existe alta competencia en su distribución. Subir su precio de manera agresiva podría reducir el volumen de ventas si los demás oferentes no suben el precio, cediendo mayor cuotas a las otras empresas del mercado. afectando también las ventas de la tienda conveniencia. Riesgo que la elasticidad asumida no captura completamente.



## Herramientas y técnicas aplicadas
#### Excel
Margen, markup, utilidad neta, margen de contribución, puntoos de equilibrio calculados por producto.
BUSCARX/INDICE + COINCIDIR: Identificación de productos con mayor/menor marge/utilidad.
SUMAR.SI: Utilidad total por categoría.
SI anidado: Clasificación automática de productos por nivel de margen (ALTO, MEDIO, BAJO).
Formato Condicional: Visualización tipo de semáforo por nivel de clasificación de margen.

#### POWER BI:
Importación y limpieza de datos, revisión del tipo de dato.
Medidas DAX: SUM, SUMX.
Margen ponderado por ingreso (no promedio simple) para reflejar rentabilidad real del negocio.
Elasticidad ponderada por volumen de ventas.
Simulación de utilidad total bajo escenario de incremento de precios, recalculando margen y volumen de ventas.
Dashboard con tarjetas KPI's, gráfico de dispersión (margen vs utilidad por producto) y gráfico de barras (utilidad y elasticidad por categoría).


## Limitaciones
Los datos son simulados, no provienen de una operación real.
Las elasticidades son supuestos razonados en base a teoría económica (productos sustitutos, necesidad, frecuencia de compra). No son estimaciones estadísticas provenientes de datos históricos de precios y cantidades.
Se asumió elasticidad uniforme por categoría. El la práctica, es casi probablemente que la elasticidad varíe por producto, según posicionamiento de marca y fidelidad de clientes (nivel de demanda). Una extensión de este análisis sería estimar las elasticidades con datos históricos reales.
La simulación de aumento de precios, no incorpora reacción de la competencia, ni efectos de imagen de marca, que en la práctica afectan las decisiones de pricing.

## Capturas del dashboard

![Dashboard estructura de precios](Estructura de precios/Estructura de precios.png)

**Autor:** Alejandro Sevilla Mejía — Economista (UNAH)
[GitHub](https://github.com/Alejo-55) | [LinkedIn](https://www.linkedin.com/in/alejandro-sevilla-a23a6b224/)
