# tarea de la semana 8.
## 1. Cuantos productos no tiene registro el país de origen:
 - Sentencia:
```
SELECT COUNT (*) - COUNT(country_of_origin) AS products_without_country
FROM product;
````
-Captura.
<imag![Imagen de WhatsApp 2024-05-30 a las 15 49 59_a8446549](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/6fff2b57-79ff-4e65-b739-31574407d987)
## 2. Numero de clientes por ciudad.
- Sentencia:
```
SELECT DISTINCT city, COUNT(city)
FROM client
GROUP BY (city)
````
-Captura.
<img![Imagen de WhatsApp 2024-05-30 a las 15 55 10_d7259422](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/d36aaa45-83dc-4b41-ad9f-338c5c162572)
