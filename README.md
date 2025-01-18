## INTRODUCCIÓN
*SpaceX*, es una empresa estadounidense de fabricación aeroespacial y de servicios de transporte espacial con sede en Hawthorne (California). Fue fundada en 2002 por *Elon Musk* con el objetivo de reducir los costes de viajar al espacio para facilitar la colonización de Marte.
Los logros de *SpaceX* incluyen:

-Enviar naves espaciales a la Estación Espacial Internacional.
-*Starlink*, una constelación de Internet por satélite que proporciona acceso a Internet por satélite.
-Envío de misiones tripuladas al espacio.

Una de las razones por las que *SpaceX* puede hacer esto es porque los lanzamientos de cohetes son relativamente económicos.
*SpaceX* anuncia los lanzamientos de cohetes Falcon 9 en su sitio web con un coste de 62 millones de dólares, otros proveedores cuestan más de 165 millones de dólares cada uno. Gran parte del ahorro se debe a que SpaceX puede reutilizar la primera etapa.
Por lo tanto, si podemos determinar si la primera etapa aterrizará, podemos determinar el costo de un lanzamiento.
La segunda etapa, ayuda a poner la carga útil en órbita, pero la mayor parte del trabajo se realiza en la primera etapa, que es bastante grande y cara.
A diferencia de otros proveedores de cohetes, el Falcon 9 de SpaceX, puede recuperar la primera etapa.
A veces, la primera etapa no aterriza, a veces se bloquea, otras veces, Space X sacrifica la primera etapa debido a los parámetros de la misión, como 
la carga útil, la órbita y el cliente.
En esta fase final, asumiré el papel de una científica de datos que trabaja para una nueva empresa de cohetes espaciales, Space Y, que quiere competir con SpaceX. 
Mi trabajo consistirá en determinar si Falcon 9 reutilizará la primera etapa y así predecir el coste de cada lanzamiento.
Para ello, recopilaré información pública sobre SpaceX acerca de los lanzamientos de Falcon 9, y crearé paneles para mi equipo de Space Y.
Crearé y entrenaré un modelo de aprendizaje automático, que usaré para hacer predicciones sobre el éxito del lanzamiento.

Que comience la acción!!

## DATA COLLECTION

* Import Libraries and Define Auxiliary Functions
* Solicitud a la API de SpaceX.
* Filter the dataframe to only include Falcon 9 launches.
* Dealing with Missing Values.

## WEBSCRAPING

* Web-scraping to collect Falcon 9 historical launch records from a Wikipedia page titled [List of Falcon 9 and Falcon Heavy launches](https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches).

![falcon9-launches-wiki](https://github.com/user-attachments/assets/af0df148-3f39-409b-9199-55213969a221)

* Import Libraries and Define Auxiliary Functions.
* Request the Falcon9 Launch Wiki page from its URL.
* Extract all column/variable names from the HTML table header.
* Create a data frame by parsing the launch HTML tables.

## EXPLORATORY DATA ANALYSIS (EDA)

* Import Libraries and Define Auxiliary Functions.
* Calculate the number of launches on each site.
* Calculate the number and occurrence of each orbit.
* Calculate the number and occurence of mission outcome of the orbits.
* Create a landing outcome label from Outcome column.

## VISUALIZATION

* Import Libraries and Define Auxiliary Functions.
* Visualize the relationship between Flight Number and Launch Site.
* Visualize the relationship between Payload and Launch Site.
* Visualize the relationship between success rate of each orbit type.
* Visualize the relationship between FlightNumber and Orbit type.
* Visualize the relationship between Payload and Orbit type.
* Visualize the launch success yearly trend.
* Create dummy variables to categorical columns.
* Cast all numeric columns to float64.





