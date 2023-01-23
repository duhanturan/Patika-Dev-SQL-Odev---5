# Patika-Dev-SQL-Odev---5
## SQL Odev - 5

### 1 - film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
````sql
SELECT * FROM FILM
WHERE TITLE LIKE "%n"
ORDER BY LENGTH DESC
LIMIT 5;
````

### 2 - film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
````sql
SELECT * FROM FILM
WHERE TITLE LIKE "%n"
ORDER BY LENGTH ASC
OFFSET 5
LIMIT 5;
````

### 3- customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.
````sql
SELECT * FROM CUSTOMER
WHERE STORE_ID = 1
ORDER BY LAST_NAME DESC
LIMIT 4;
````
