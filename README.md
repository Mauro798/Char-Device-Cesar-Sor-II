# Trabajo Práctico 0: Device Drivers

El objetivo de este trabajo práctico, es crear un Kerner Module para un Char Device. Este recibirá un String y lo encriptará con el método Cesar con un valor de 3, Esto quiere decir que si una letra del mensaje es una A, pasara a ser una D.


## Make del Modulo

Primero se compila el codigo con make

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2015-19-00.png)

Esto nos genera como resultado los siguientes archivos

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2015-19-39.png)

## Carga del modulo y creación del archivo asociado

Cargamos el modulo creado y revisamos la lista de modulos para ver que se haya cargado bien

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2018-16-26.png)

Vemos el log del kernel para saber que mayor number usar

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2018-18-01.png)

Creación del archivo asociado en el kernel con el mayor number indicado

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2018-20-17.png)

## Probando el char device

Ahora le cambiamos los permisos de lectura y escritura para poder trabajar. Despues de eso le pasamos un mensaje y luego leemos el mensaje que le pasamos y nos lo devuelve encriptado.

![](/Imagenes%20TP0/Captura%20de%20pantalla%20de%202020-10-05%2018-32-32.png)

