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

![Figura1](https://github.com/francofrolla/TCpasturasSentinel/blob/e8eaaf70015d27d2ef5e805f2b15d5b9904195e0/imagenes/figura1.png)

Salvar el acrivo en formato **GeoJSON**  
En **QGIS > Exportar > Guadar objeto como.. > Formato (GEOJson)**

Abrir la app https://tcpasturassentinel2.herokuapp.com/

a) Cargar el GeoJson generado    
b) Agregar Lote  
c) Buscar Imagenes  
d) Seleccionar la mejor imagen presente en los ultimos 25 dias de la fecha presente  
e) Calcular TC (tasa de crecimiento)  
f) Descargar archivo con tasa de crecimiento por poligono (Formato GEOJson)  
e) Abir en QGIS   

### Descargo de responsabilidad: 
El autor no se hace responsable por el uso de los datos generados por la aplicación creada. La misma utiliza servicios gratuitos para fines no comerciales los cuales possen sus limitaciones para su uso en ambitos que no sean de testeo o desarrollo. 

### Video en Youtube
https://www.youtube.com/watch?v=OqIvd163nVU
