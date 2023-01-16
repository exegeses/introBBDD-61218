## Consultas usando LIKE

> traer nombre, precio y descripción 
> de la tabla productos, dónde en el nombre
> contenga 'Marshall'

    SELECT prdNombre, prdPrecio, prdDescripcion  
    FROM productos  
    WHERE prdNombre LIKE '%MarshalL%';  

> Traer nombre, precio y descripción 
> de la tabla productos, dónde en el nombre
> contenga 'Bluetooth'

    SELECT prdNombre, prdPrecio, prdDescripcion  
    FROM productos  
    WHERE prdDescripcion LIKE '%Bluetooh%';

> Ahora con más tablas
> Traer nombre, marca, precio y descripción
> de la tabla productos, dónde en la descripcion
> contenga 'Altavoz' 

    SELECT prdNombre, mkNombre, prdPrecio, prdDescripcion
    FROM productos, marcas
    WHERE productos.idMarca = marcas.idMarca
	 AND  prdDescripcion LIKE '%Altavoz%';

> La misma consulta utilizando JOIN

    SELECT prdNombre, mkNombre, prdPrecio, prdDescripcion
    FROM productos
     JOIN marcas
       ON productos.idMarca = marcas.idMarca
     WHERE prdDescripcion LIKE '%altavoz%';

