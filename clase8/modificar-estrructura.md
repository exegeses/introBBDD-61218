# Modificar estructura de una tabla

## Cambiar nombre de una columna

    ALTER TABLE nombreTabla  
        CHANGE nombreViejo nombreNuevo tipoDato;  

    ALTER TABLE destinos  
        CHANGE destAsientos modificado tinyInt not null;

## Cambiar tipo de datos de una columna  

    ALTER TABLE nombreTabla  
        MODIFY nombreCampo tipoDato modificador;  

    ALTER table destinos  
        MODIFY destNombre varchar(60) not null;  

    ALTER table destinos  
        MODIFY destPrecio float(10,2) not null;  

## Agregar nueva columna (al final de la tabla)  

    ALTER TABLE nombreTabla  
        ADD nombreCampo tiporDato modifadores;  

    ALTER TABLE destinos  
        ADD descripcion varchar(500) not null;   

## Agregar nueva columna (después de una columna)  

    ALTER TABLE nombreTabla  
        ADD nombreCampo tiporDato modifadores AFTER columna; 

    ALTER TABLE destinos  
        ADD fechaAlta DATE not null AFTER destPrecio;  

    ALTER TABLE destinos    
        ADD fechaAlta DATE DEFAULT '2023-01-11' not null AFTER destPrecio;  

## Eliminar una columna de una tabla  

    ALTER TABLE nombreTabla  
        DROP nombreCampo;  

    ALTER TABLE destinos  
        DROP descripcion;  

