# GeoVisualizacion
A través de esta práctica vas a lograr:  Identificar información geoespacial de utilidad para resolver un problema. Integrar los conocimientos adquiridos para visualizar información sobre un mapa. Manipular y realizar operaciones sobre los datos para tener una mejor visualización y apoyar en la tomar decisiones.
Introducción:



Durante este reto vas a utilizar información sobre los Estados de la República Mexicana, incluyendo los Polígonos que los componen, así como información sobre la ubicación de las sucursales de Costco en México. Supongamos que Bertha es una empresaria mexicana que tiene una cadena de restaurantes de comida rápida, en particular hamburguesas y desea abrir una nueva sucursal que se encuentre dentro del rango de entregas a domicilio de la cadena Costco ya que ahí compra la materia prima para preparar los alimentos. Para ello te han contratado para que indiques en qué región (o regiones) del país NO sería conveniente poner otra sucursal debido a la falta de cobertura de entregas a domicilio. 

 

Los datos de los estados se encuentran en algunos archivos llamados mexican-states con diferentes extensiones, que fueron creados para Los Angeles Times con datos de OpenStreetMap. La información de la ubicación de las sucursales fue recuperada de la página oficial de Costco, depurada y procesada a mano para poder utilizarla para la visualización. Puedes revisar las referencias al final del documento si deseas más información al respecto. 

 

En resumen: 

Vas a utilizar información oficial sobre los Estados de la República Mexicana y la localización de las sucursales de Costco en el país
Descargar los archivos de mexican-states y tiendasCostco_.csv
Procesar los datos usando Python para responder la siguiente pregunta:
¿En qué regiones del país (centro, centro oeste, noreste, noroeste, sureste) NO es conveniente abrir una nueva sucursal debido a la falta de cobertura de entregas a domicilio?
 

Instrucciones:

 

Es necesario cumplir con todos los pasos descritos a continuación para que puedas resolver el reto exitosamente: 

 

Descarga todos los archivos mexican-states con sus diferentes extensiones.
Descarga el archivo tiendasCostco_.csv. 
Crea una nueva libreta de Google Colab para programar tu script en Python.
Carga los datos de los Estados de la República Mexicana en un GeoDataFrame.
Carga los datos de la localización de las sucursales de Costco en un DataFrame.
Convierte los datos de la localización de las sucursales de Costco en un GeoDataFrame, creando Puntos a partir de la longitud y latitud de cada sucursal. 
Agrega una columna a los estados que indique la región a la que pertenecen y separa el GeoDataFrame por regiones en lugar de por estados:
Centro: Tlaxcala, Puebla, CDMX, Morelos, Estado de México e Hidalgo;
Centro Oeste: Jalisco, Michoacán, Colima, Aguascalientes, Nayarit, Zacatecas, San Luis Potosí, Guanajuato y Querétaro;
Noreste: Chihuahua, Coahuila, Nuevo León, Tamaulipas y Durango;
Noroeste: Baja California Norte, Baja California Sur, Sonora y Sinaloa;
Sureste: Guerrero, Veracruz, Oaxaca, Tabasco, Chiapas, Campeche, Yucatán y Quintana Roo.
Asegura que ambos GeoDataFrames utilicen el CRS epsg=3395 que usa metros como medida de distancia.
Crea un buffer de 120 km alrededor de los puntos de localización de cada sucursal. 
Grafica la intersección de las regiones con los círculos creados a partir de la localización de las sucursales. 
Identifica las regiones en dónde se requiere más cobertura y responde la pregunta: 
 ¿En qué regiones del país (centro, centro oeste, noreste, noroeste, sureste) NO es conveniente abrir una nueva sucursal debido a la falta de cobertura de entregas a domicilio?
