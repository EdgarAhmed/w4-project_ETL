# w4-project_ETL

Proyecto semana 4

El proyecto de la semana 5 consiste en la extracción, limpieza y carga de datos sobre un tema de libre elección. 

Los parámetros a seguir han sido los siguientes.

1.	Se debe de obtener la información de 3 fuentes distintas.
2.	Los métodos de extracción deben de ser al menos, 2. Descarga directa de ficheros, “strapeo” de páginas webs/base de datos, uso de “apis/rss”, entre otros.
3.	Limpieza y homogeneización de los datos.
4.	Subida a la base de datos a elección (Mongo/SQL).

En este caso en particular escojo ver la incidencia que tiene el cáncer (en general, sin hacer ninguna diferenciación) en 4 países, España, Francia, Reino Unido y Estados Unidos. En un inicio también había la determinación de realizar dicho trabajo añadiendo los datos de China e India, para ver si el resto de indicadores socioeconómicos arrojaban algún tipo de diferencia. Sin embargo, ni en la web de la OMS, ni en la web de la OCDE aparecían datos de estos dos países sobre la incidencia de cáncer en su población. 

A su vez, se extrajeron datos de la cantidad de emisiones de CO2 y la renta per cápita para ver si estos dos indicadores socioeconómicos tenían algún tipo de relación de cara a la aparición de cáncer.

Estos datos son extremadamente generales y no se pueden inferir ni sacar conclusiones directas todavía. La idea es usar este ejercicio de cara a un proyecto final e ir afinando cada semana más con indicadores más precisos y más 


1.	Extracción de datos. 

Se extraen datos de las siguientes webs. 

De la OCDE se obtiene datos de la renta per cápita de los países seleccionados y las emisiones de CO2 per cápita. Esta extracción se hace con “selenium” y descarga directa respectivamente (ejemplo en el siguiente gif).

![](https://github.com/EdgarAhmed/w4-project_ETL/blob/main/pics/ejemplo.gif)


De “OurWorldInData” se extraen datos de incidencia poblacional del cancer en España, supervivencia de cáncer a 5 años en todo el mundo y distribución de tumores en toda la población y estandarizados en toda la población. 

2.	Limpieza de datos.

Una vez obtenidos los CSVs, se cargan a Jupyter. Se eliminan columnas, se homogenizan los distintos valores que pueden aparecer.

3.	Subida a base de datos. 
En este caso, se suben a sql.

![](https://github.com/EdgarAhmed/w4-project_ETL/blob/main/pics/Screenshot%202023-11-06%20at%2018.13.28.png)

Fuentes: 

https://www.oecd.org/ 

https://ourworldindata.org/

https://www.who.int


Bibliotecas usadas para Python.

https://pandas.pydata.org/

https://www.selenium.dev/documentation/webdriver/

https://tqdm.github.io/docs/notebook/

