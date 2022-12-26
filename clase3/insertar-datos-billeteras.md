# Insertar datos en una tabla

> Para insertar datos en una tabla  
> utilizamos el comando "INSERT"

> Sintáxis versión a (mencionando los campos)    

    INSERT INTO nombreTabla   
        ( nCampo2, nCampo3, nCampo4 )  
      VALUES  
        ( valor2, valor3, valor4 );  

> Ejemplo 
 
    INSERT INTO billeteras  
        ( nombre, precio, stock )  
      VALUES  
        ( 'Ledger Nano S', 16000, 30 );


> Sintáxis versión b (sin mencionar campos)

    INSERT INTO nombreTabla  
        VALUES  
          ( valor1, valor2, valor3, valor4 );  

> Ejemplo: 

    INSERT INTO billeteras  
        VALUES  
          ( DEFAULT, 'Trezor One', 19500, 30 );  


----

> También podemos insertar varios registros en un sólo comando  

    INSERT INTO billeteras    
        ( nombre, precio, stock )  
      VALUES  
        ( 'Trezor T', 78000, 20 ),  
        ( 'Ledger Nano X', 56000, 20 );  
