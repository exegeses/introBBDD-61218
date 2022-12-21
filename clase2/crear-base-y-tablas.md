# Creación de bases de datos y de tablas

## Creaci´´on de una base de datos  

> Para crear una base de datos usamos el comando   
> "CREATE DATABASE"

    CREATE DATABASE introDB;  

> Si queremos interactuar con una base de datos,
> debemos activarla.  
> Para activar una base, utilizamos el comando "USE"  

    USE introDB;  

### Borrado de una base 

    DROP DATABASE introDB;



## Creación de tablas  

> Para crear una tabla utilizamos el comando  
> "CREATE TABLE"

> Sintáxis  

    CREATE TABLE nombreTabla
        (
            campo1 tipoDato características,
            campo2 tipoDato características,
            campo3 tipoDato características
        );


    CREATE TABLE billeteras  
    (
        id tinyint primary key auto_increment not null,
        nombre varchar(30) not null,
        precio float(9,2) not null,
        stock tinyint not null
    );