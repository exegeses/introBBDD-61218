# Consultas en SQL

## Consultas a server 

> Para generar consultas a un server de BDD 
> utilizamos la sentencia ***"SELECT"***  

## Consultas a tablas 

> Para generar consultas a tablas de una BBDD
> también utilizamos la sentencia ***"SELECT"***,  
> pero además debemos especificar las/s tablas  
> con la palabra ***FROM***  

    SELECT * FROM destinos;  

> Si queremos traer sólo datos de algunos campos de la tablas la sintáxis es la siguiente  

    SELECT nCampo2, nCampo4, nCampo5  
        FROM nombreTabla;

> Ejemplo práctico:  

    SELECT destNombre, destPrecio  
        FROM destinos;  

## Ordenando registros 

> Para ordenar registros, utilizamos la palabra
> ***ORDER BY***  
> Sint´´axis:  

    SELECT nCampo2, nCampo4, nCampo5    
        FROM nombreTabla  
        ORDER BY nCampo3;
    
> Ejemplo práctico 

    SELECT destNombre, destPrecio    
        FROM destinos  
        ORDER BY destPrecio;  

## Filtrado de registros

> Filtrar registros significa traer sólamente los registros que cumplan alguna condicion dada  

> Para especificar condiciones de filtrado usamos la palabra ***WHERE***  

> Traer nombre y precio de destinos  
> con un precio que no supere 8000

    SELECT destNombre, destPrecio  
        FROM destinos  
        WHERE destPrecio <= 8000;

> Traer nombre y precio de destinos  
> con un precio que no supere 8000  
> y además ordenar los resultados por precio.  

    SELECT destNombre, destPrecio  
        FROM destinos  
        WHERE destPrecio <= 8000  
        ORDER BY destPrecio;  

> Traer nombre y precio de los destinos  
> donde el precio esté entre los valores 6600 y 8000  

    SELECT destNombre, destPrecio
        FROM destinos
        WHERE destPrecio >= 6600 
         AND destPrecio <= 8000
         ORDER BY destPrecio;

> Ahora misma consulta con la palabra ***BETWEEN*** 

    SELECT destNombre, destPrecio  
        FROM destinos  
        WHERE destPrecio BETWEEN 6600   
        AND 8000;  

> Traer nombre y precio de los destinos de la región 5

    SELECT destNombre, destPrecio   
		FROM destinos  
        WHERE idRegion = 5;  

> Traer nombre y precio de los destinos 
> de la región 5 y también de la región 3  

    SELECT destNombre, destPrecio   
		FROM destinos  
        WHERE idRegion = 5  
          OR idRegion = 3;  

        

