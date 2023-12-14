- Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
```SQL
SELECT AVG(rental_rate) from film;
```
- Film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
```SQL
SELECT COUNT(*) from film
WHERE title LIKE 'C%';
```
- Film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
```SQL
SELECT MAX(length) from film
WHERE rental_rate = 0.99;
```
- Film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
```SQL
SELECT COUNT(DISTINCT replacement_cost) from film
WHERE length > 150;
```
