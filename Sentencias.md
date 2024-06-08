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

## 3. Contar el número de productos de una categoría específica.
- Sentencia:
```
SELECT SUM(price)
FROM product
WHERE category = 'Audio';
````
-Captura.
<img!![Ima](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/cbf6d1f3-cdac-42c1-bb35-f12d467de00b)

## 4.Contar el número de clientes en una ciudad específica.
 - Sentencia:
```
 ## 5.Contar el número de productos cuyo precio está dentro de un rango específico.
- Sentencia:
```
````
-Captura.
 ## 6. Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico,
- Sentencia:
```
````
-Captura.
 ## 7. Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico
- Sentencia:
```
````
-Captura.
 ## 8. Seleccionar productos que fueron producidos en un año específico y en un país de origen específico
- Sentencia:
```
````
-Captura.
 ## 9. Seleccionar clientes cuyo nombre completo comience con 'J'.
- Sentencia:
```
````
-Captura.
  ## 10. Seleccionar clientes cuya ciudad contenga la letra 'a'
- Sentencia:
```
````
-Captura.
