# Relaciones entra tablas

> Cuando queremos traer información de más de una tablas ( dos o más ) debemos relacionar las tablas.  
> La técnica ***"table relation"*** se logra igualando la columna en común a ambas tablas (la columna de relación). 

    SELECT prdNombre, prdPrecio, mkNombre  
        FROM productos, marcas  
        WHERE productos.idMarca = marcas.idMarca; 

    SELECT prdNombre, prdPrecio, mkNombre  
        FROM productos, marcas  
        WHERE productos.idMarca = marcas.idMarca  
        AND productos.idCategoria = categorias.idCategoria;

> La técnica JOIN también puede trear datos de varias tablas. 

    SELECT prdNombre, prdPrecio, mkNombre  
        FROM productos  
        JOIN marcas  
        ON productos.idMarca = marcas.idMarca;

    SELECT prdNombre, prdPrecio, mkNombre, catNombre  
        FROM productos  
        JOIN marcas  
        ON productos.idMarca = marcas.idMarca  
        JOIN categorias  
        ON productos.idCategoria = categorias.idCategoria;



