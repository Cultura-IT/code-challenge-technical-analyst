# Cultura IT - Code Challenge

Bienvenidos!

Estamos buscando desarrolladores analistas técnicos para incorporar a nuestro equipo de trabajo. 
Con el fin de validar tus conocimientos, quién mejor que el código para comprobarlo. Por lo cual te proponemos que nos ayudes a resolver el siguiente problema; por favor tomate un tiempo para pensarlo y resolverlo.

## Empresa de logística

Se trata de una diversa cantidad de empresas de logística, donde cada una de ellas cuenta con "n" centros de distribuciones.
Cada centro de distribución cuenta con un depósito en el cual se puede almacenar una cantidad limitada de paquetes. Una vez que recibe sus paquetes y llena su depósito no deberá volver a recibir entregas.
Las empresas no distingue entre diferentes paquetes, es decir, cada paquete equivale lo mismo en cuanto a tamaño y peso. 
Las empresas nos piden diseñar un algoritmo que permita determinar cuantos días tardarán en entregar todos los paquetes en los centros de distribuciones con la siguiente particularidad, el camión debe entregar por día la misma cantidad de paquetes en todos los centros de distribuciones, y esta cantidad está determinada por el centro de distribución que menor espacio en su depósito tenga. Por ejemplo:
* Centro de distribución 1: espacio en depósito 5
* Centro de distribución 2: espacio en depósito 2
* Centro de distribución 3: espacio en depósito 10
Para este ejemplo se podrá entregar el primer día solo 2 paquetes. Mientras que el segundo día 3 paquetes.

Se requiere que la aplicación pueda:
1. Determinar la cantidad de días que se tardará en entregar los paquetes.
2. Poder visualizar un paso a paso de la fluctuación de las cantidades de paquetes en el transcurso de los días.
3. Loggear en la consola de desarrollador el tiempo que tarda el algoritmo en resolver el problema.

###### Restricciones:
El algoritmo no deberá tardar más de 20 segundos en procesar la información para ninguna de las empresas.

###### NOTAS:
El frontend de la apliación se deberá desarrollar en cualquier tecnología.  
El backend se consumirá de https://logicproblemapi.herokuapp.com/.  
Las rutas posibles para obtener datos llevan la siguiente estructura:
- GET	/getEmpresas -- https://logicproblemapi.herokuapp.com/getEmpresas -- obtener todas las empresas
- GET	/getCentrosDistribucion?empresa=1 -- https://logicproblemapi.herokuapp.com/getCentrosDistribucion?empresa=1 -- obtener las cantidades de almacenamiento de los depositos de los centros de distribución filtrando por empresa
- GET	/checkDias?empresa=1&dias=100 -- https://logicproblemapi.herokuapp.com/checkDias?empresa=1&dias=100 -- checkear que la cantidad de días son correctas

###### EJEMPLO:
request - /getCentrosDistribucion?empresa=1
response - [5,2,10]
Luego de procesar la información la cantidad de días es 3

###### AYUDAS:
https://www.youtube.com/watch?v=g2o22C3CRfU

Evitar estructuras repetitivas anidadas

### Cómo presentar la solución
Cuando consideres que el problema está resuelto, debes subirlo a un repositorio de tu elección y enviarnos un mail a fsare@culturait.com.ar con el link del repositorio adjunto, además podes agregar cualquier comentario que creas correspondiente.


**Happy hacking!**
