<h1 align='center'>
 <b>PROYECTO INDIVIDUAL Nº2</b>
</h1>
 
## **Descripción del problema (Contexto y rol a desarrollar)**

### **Contexto**

La pandemia del **COVID-19** tuvo un gran impacto en los mercados financieros internacionales, que llevaban años de relativa tranquilidad después de la **crisis financiera del 2008**, causada por la burbuja de la deuda inmobiliaria estadounidense. La pandemia, considerada por muchos analistas como un evento "cisne negro", tuvo implicaciones no solo en la salud de las personas, sino también en otros ámbitos, como la producción global de bienes y servicios y la forma en que trabajamos.

Los confinamientos cortaron por períodos más o menos extendidos casi todas las líneas de suministros, perjudicando la producción global de bienes y servicios. Al mismo tiempo, la generación de nuevas tendencias "remote first" llevó al crecimiento exponencial de empresas de consumo masivo online o de herramientas que permitieran tal filosofía de trabajo, como Zoom.

Este cambio se tradujo en el mercado en un movimiento muy marcado de inversiones hacia **empresas tecnológicas**, mientras que las consideradas tradicionales se vieron más o menos desfavorecidas. Sin embargo, muchas personas que dependen de la presencialidad vieron reducidos sus ingresos al punto de ver comprometida su subsistencia, por lo que la mayoría de los gobiernos adoptó medidas de asistencia, recurriendo a la emisión monetaria para tales fines.

Esto llevó a una hiperliquidez a nivel global, cuyos efectos se ven aún hoy. La Reserva Federal ha estado realizando aumentos de las tasas de interés que paga por sus bonos a un ritmo no visto desde hace décadas, en un intento por bajar la aún creciente inflación. La incertidumbre con respecto a la situación económica mundial y el impacto de otros eventos como la guerra Ucrania-Rusia han despertado una migración al dólar estadounidense, en busca de refugio.

La subida de tasas por parte de la FED y la migración al dólar causaron su fortalecimiento, generando que muchos países en vías de desarrollo vieran encarecidas sus deudas en dólares, y empezaran a notarse indicios de una recesión inminente. Sin embargo, los mercados financieros son el espacio en donde se encuentran la oferta y la demanda de activos financieros, como bonos y acciones. De esta forma, a través del mercado, los gobiernos y las empresas pueden obtener financiamiento, mientras que las personas pueden invertir sus ahorros y obtener ganancias.

En líneas generales, en el corto/mediano plazo se observan muchas variaciones en los precios de los activos, pero a largo plazo se suelen observar tendencias alcistas (también llamadas bullish) o tendencias bajistas (bearish). Una herramienta utilizada para el correcto análisis y visualización de los precios, minimizando el “ruido” generado por la volatilidad inherente, son las medias móviles, que muestran el valor medio del precio de un mercado/activo durante un determinado período de tiempo y en función del cambio del precio, su valor medio va aumentando o disminuyendo.

Si por ejemplo tomamos una media móvil de periodo 200 (es decir, 200 sesiones) tenemos la media aritmética del precio durante las anteriores 200 sesiones y lo que se hace es que se suman los 200 precios de cierre y posteriormente los dividimos entre 200.

 
### Rol a desarrollar

Considerando que la empresa no conoce esta área financiera, le solicita una explicación de qué ha sucedido en este mercado en los últimos años (considerando impactos positivos y negativos a partir del año 2000), recomendaciones de inversión (ya sea enfocada en empresas o rubros de éstas) y otra información complementaria que, usted como experto en datos, está en capacidad de brindar. 

El foco del análisis es variado y amplio, siendo posible incorporar focos como la variación de precios en el tiempo, la comparación entre distintas acciones, cálculo de estadísticas bursátiles (volatilidad, promedios móviles, entre otras), recomendaciones basadas en el retorno y riesgo de inversión e incluso la creación de KPIs útiles para la toma de decisiones de inversión. La empresa deja a su disposición el o los focos que desee analizar, el resto de las exigencias se indicarán más adelante.

Limitaremos el análisis a las empresas pertenecientes al índice SP500 ([Standard & Poor's 500 Index](https://www.google.com/url?q=https://en.wikipedia.org/wiki/List_of_S%2526P_500_companies&sa=D&source=docs&ust=1676566032938438&usg=AOvVaw3J6gZYtEH8xJABTCf0pYqO)).

Considerando lo anterior, el principal objetivo es poder conocer la situación del mercado bursátil en los últimos 23 años según los focos mencionados anteriormente, permitiendo que usted, como Analista de Datos, sea capaz de dar un contexto de la situación y generar recomendaciones de inversión, como mínimo se espera que pueda recomendar en qué compañías invertir y qué día de la semana es recomendable hacerlo.


## **Arbol del proyecto:**
 
│   
├───**datasets:** Contiene los datasets utilizados en nuestros dashboards.  
│       ├───companies.csv   
│       └───GSPC.csv       
├───**EDA.ipynb:** Analisis exploratorio de los datos de los datasets.    
├───**PI02.pbix:** Dashboards del proyecto, requiere PowerBI para ser ejecutados.   
└───**README.md:** Es el archivo que usted se encuentra leyendo en este momento.    
   

## **Consideraciones, calculos y metricas utilizadas**

Es importante destacar que en nuestro proyecto utilizaremos el **cierre ajustado** para la mayoria de los calculos ¿Por qué? Por que el cierre ajustado es el precio de cierre después de los ajustes para todas las distribuciones de splits y dividendos aplicables. Algunas acciones corporativas toman en cuenta temas como divisiones de acciones, dividendos, distribuciones y ofertas de derechos, las cuales  afectan el precio de una acción y se necesitan ajustes para llegar a un reflejo técnicamente exacto del verdadero valor de esa acción.

### **Calculos y metricas realizadas**


**Daily Return:** Se calcula sacando el cambio porcentual entre un cierre ajustado y su anterior.

**Media movil:** Es un promedio del cierre ajustado a lo largo de un periodo particular.

**Tasa de retorno promedio diaria:** Es un promedio del Daily return o retorno diario calculado con anterioridad.

**Rentabilidad Acumulada:** Hace referencia al primer precio de las acciones frente a su último precio en un periodo de tiempo determinado.

**Rendimiento Total:** Es la suma del Daily Return en un determinado periodo de tiempo. Como Daily Return puede ser negativo, resulta una medida interesante a tener en cuenta.

**Volatilidad:** Es una medida de la frecuencia e intensidad de los cambios del precio de un activo o de un tipo definido como la desviación estándar de dicho cambio en un horizonte temporal específico.
