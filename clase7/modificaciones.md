# Modificación de datos  

> Para modificar datos en un registro utilizamos
> el comando ***"UPDATE"***  

    UPDATE nombreTabla  
        SET campo = valor  
      WHERE campoID = valorID;  

    UPDATE destinos  
        SET destPrecio = 8470  
      WHERE idDestino = 6;  

    UPDATE nombreTabla  
        SET campo = valor,  
            campo2 = valor2,  
            campo3 = valor3  
      WHERE campoID = valorID;  