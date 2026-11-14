                     
### TP-Final-analisis-de-datos 📒

Curso: Herramientas básicas para Análisis de Datos - Centro UTN E-Learning
                                       
### Descripción general: Evolución del mercado argentino de peróxido de hidrógeno (2021-2026) 

Siendo Solvay Peróxidos uno de los mayores fabricantes de este insumo, es primordial monitorear nuestra posición en el mercado analizando periódicamente las importaciones de la posición arancelaria correspondiente, así como incluir con la mayor precisión posible las cantidades fabricadas en el país.  

📂DATASET: (https://app.penta-transaction.com/home/detalle/AR/importDetalladas) se requiere contraseña pero ya se descargaron los datos en el archivo H2O2 2021 Sep 2026_sucio.xlsx presente en este repositorio.
Se descargan por año las importaciones de la posición arancelaria del peróxido de hidrógeno (código 2847) y se arma el archivo, que unifica todos los despachos de importaciones en el período 2021 - Sep 2026.
Se compone de casi 6000 filas y 36 columnas. Contiene información sobre toneladas importadas, precios y costos logisticos.

### Estructura de datos

              
              ├── IMAGES                                    : Contiene gráficos varios
              
              ├── H2O2 2021-Sep 2026_sucio(1).xlsx          : dataset estructurado obtenido de servicios aduaneros

              ├── MercadoPeroxlimpio(5).xlsx                : dataset limpio de filas nulas y anómalas luego de tratamiento en Colab con Python

              ├── README.md                                 : Resumen de los puntos más importantes y acciones para mejorar

              ├── TP Final Dashboard.pbix                   : Principales KPIs respondiendo a los objetivos 

              ├── TP final.ipynb                            : Notebook en plataforma Colab utilizando Python para clasificar y extraer datos útiles para analizar las estadísticas de mercado

              ├── requirements.txt                          : Librerías para correr este modelado de datos con Python


### 🎯Objetivos principales: Hacer el seguimiento a lo largo de los últimos 5 años de los siguientes indicadores

#### 1) Monitorear la evolución del tamaño del mercado en toneladas y participación de cada empresa y conocer en cualquier año si cumplimos con la meta del 15%



<img src="https://github.com/PADelucchi/herramientas-basicas-analisis-de-datos-Delucchi-Pablo/blob/main/images/Mkt%20perox%20Ene-Sep%20comparaci%C3%B3n.png" alt="Descripción del gráfico" width="700">

Se observa que el mercado ha disminuido desde el cambio de modelo económico implementado por el actual gobierno, debido a la caída del consumo que afecta a la industria textil y papelera, así como la apertura de importaciones.
 
Y en el siguiente se aprecia la evolución del mkt share

<img src="https://github.com/PADelucchi/herramientas-basicas-analisis-de-datos-Delucchi-Pablo/blob/d067cb408a9180a11a1435acb5cfad9ed6ae1f64/images/Evol%20Mkt%20Share%20a%C3%B1o.png" alt="Descripción del gráfico" width="700">

Nuestro market share se ha mantenido cercano a la meta del 15% durante la actual gestión económica y descendido fuertemente desde el año 2022. Esto es debido también a la caída en los precios finales a los clientes. Nuestra estructura de costos y fletes no ha mejorado lo que nos resta competitividad.


#### 2) Seguir la evolución de los precios y comparación frente a la competencia

<img src="https://github.com/PADelucchi/herramientas-basicas-analisis-de-datos-Delucchi-Pablo/blob/main/images/Precios%20y%20fletes%20competidores%20directos.png" alt="Descripción del gráfico" width="700">

En la gráfica se excluyen los usuarios directos, haciendo foco en los competidores directos, es decir el sector de reventa. Se evidencian nuestros costos mayores frente al competidor Dalgar sobretodo en los últimos 2 años, pero bien posicionados frente a Febel.

#### 3) Medir la incidencia del costo logístico en el precio del producto, que no sea mayor a 150 usd/tn y su comparación frente a competidores directos.

Del mismo gráfico se pueden ver los precios de los fletes por tonelada, y también debemos mejorar frente a Dalgar. Las columnas azules, que representan el costo de producción + flete, para Solvay Peróxidos marcan que nuestro margen de rentabilidad está bajo presión porque los precios para los clientes, lejos de mantenerse estables, están yendo a la baja para la poca demanda agua oxigenada.

### Instrucciones de uso

Para ver criterios de clasificación y limpieza del dataset, junto con gráficas correr el siguiente enlace
* [Analisis Python via Colab](https://github.com/PADelucchi/herramientas-basicas-analisis-de-datos-Delucchi-Pablo/blob/main/TP%20final%20.ipynb)

Para ver KPIs que describen el cumplimiento de metas, se accede al siguiente dashboard donde se puede filtrar por año, mes y por empresa.

 * [PowerBI Dashboard](https://app.powerbi.com/groups/me/reports/98037350-6f8a-49dd-a79e-037e0111255c/9684fd06026c94b4c3b1?experience=power-bi)


### 🔍Resultados  

El mercado argentino de agua oxigenada viene cayendo sin pausa desde 2023, lo que muestra una relación directa con la caída del consumo y la actividad industrial.
La incidencia de los fletes ha aumentado dado que los precios bajaron mientras nuestros transportes (Solvay Peróxidos) se mantuvieron casi constantes desde 2021 en USD/tn.
Frente a este contexto se buscará importar producto desde Chile por la menor distancia respecto a Brasil.

Es prioritario renegociar nuestros servicios logísticos, logrando una reducción mínima del 10%, así como también nuestros costos de producción, para ser más competitivos y adaptarnos a la realidad del mercado actual. Con estas medidas, volveremos al nivel mínimo de un Mkt Share del 15%

La tendencia es que se mantendrá un mercado recesivo y sin cambios hasta después de las elecciones del año próximo, en caso que aumente el consumo de la población, y no dependerá tanto de que se restrinjan las importaciones de producto terminado.


#### Clonar repositorio

git clone https://github.com/usuario/proyecto.git 

#### Instalación librerías

```pip install -r requirements.txt```

### 🛠️Herramientas utilizadas: entorno Google Colab, Python, pandas, matplotlib, plotly, Power BI

### Autor: Pablo Delucchi
