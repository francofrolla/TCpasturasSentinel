# TCpasturasSentinel
App web desarrollada en Heroku apps para estimar la Tasa de crecimiento con datos satelitales de la misión Sentinel2

Este proyecto surgue del interes de un asesor agropecuario de la zona de Cnel. Suarez. El mismo realiza estimaciones de tasa de crecimiento usando datos de Sentinel 2 y metodologia desarrollada por tecnicos de la UBA. Especificamente en este repositorio se automatizo el trabajo que se realiza manualmente y se construyo una aplicación web para su uso.

Referencias de la metodoliga (con datos de MODIS):
http://www.agro.uba.ar/laboratorios/lart

Requerimientos:
Se debe identificar mediante poligonos las areas a estimar la Tasa de crecimiento, la misma puede hacer referencia a lotes, ambientes, zona.    
Para cada Poligono se debe identificar el cultivo presente mediante las siguientes etiquetas en un columna llamada **CULTIVOS**, se pueden agregar otras columnas sin que esto afecte el programa:

VERDEO INVIERNO  
CN+AGRO  
CN+FEST  
CAMPO NATURAL  
PASTURA ALFALFA  
PASTURA CONSOCIADA  
PASTURA AGROPIRO  
ALFALFA PURA  
PASTURA FESTUCA  
VERDEO SORGO  
VERDEO MAIZ  
  
Vista de una tabla de atributos lista para la carga del archivo en la app:

