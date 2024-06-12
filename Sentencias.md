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
SELECT COUNT(*) AS numero_de_client
FROM client
WHERE city = 'Quito';
SELEC 
````
-Captura.
<img!![Captura de pantalla 2024-06-08 175207](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/9eaa2277-0f6a-42f6-ae1e-1755fac6cb47)

 ## 5.Contar el número de productos cuyo precio está dentro de un rango específico.
- Sentencia:
```
SELECT COUNT(*) AS numero_de_productos
FROM product
WHERE price >= 10 AND price <= 20;
````
-Captura.
<img!![Captura de pantalla 2024-06-08 180216](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/44b840c2-c64f-466c-8d01-5ffc5014534e)

 ## 6. Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico,
- Sentencia:
```
SELECT id_client, nombre, ciudad, tipo_client
FROM client
WHERE ciudad = 'Quito' AND tipo_cliente = 'Premium';
````
-Captura.
<img!![Captura de pantalla 2024-06-08 180759](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/b2cc8114-5113-4288-b2cc-2910e44d19f7)

 ## 7. Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico
- Sentencia:
```
SELECT name, category, price
FROM product
WHERE category = 'Clothes'
  AND price > 100;
````
-Captura.
<img!![image](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/6c8dbe58-f358-41c3-8fa4-845456be8164)

 ## 8. Seleccionar productos que fueron producidos en un año específico y en un país de origen específico
- Sentencia:
```
SELECT id, year_of_production, country_of_origin
FROM product
WHERE year_of_production = 2022 AND country_of_origin = 'USA';

````
-Captura.
<img!![Captura de pantalla 2024-06-08 182522](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/d7caf713-879b-4128-9300-b7025f642ebd)

 ## 9. Seleccionar clientes cuyo nombre completo comience con 'J'.
- Sentencia:
```
SELECT id, full_name
FROM client
WHERE full_name LIKE 'J%';
````
-Captura.
<img!![Captura de pantalla 2024-06-08 182912](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/6be38323-d58b-4c60-805e-8d41a4bb79c5)

  ## 10. Seleccionar clientes cuya ciudad contenga la letra 'a'
- Sentencia:
```
SELECT id, city
FROM client
WHERE city LIKE '%a%';
````
-Captura.
<imag!![Captura de pantalla 2024-06-08 183118](https://github.com/micaelabar/tarea_deberes_gsetiondebasededatos/assets/148156209/ca554608-6e07-4583-9512-b155eacd122b)

