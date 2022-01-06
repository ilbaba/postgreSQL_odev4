# postgreSQL_odev4
PostgreSQL - Dördüncü ödev - Ilgar Babashli

# _Q1_ 
film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
# _Ans_
SELECT DISTINCT replacement_cost from film;

# _Q2_ 
film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
# _Ans_
SELECT COUNT (DISTINCT replacement_cost) from film;

Çıktı: 21

# _Q3_ 
film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
# _Ans_
SELECT COUNT(title) from film
WHERE title LIKE ('T%') AND rating = 'G';

Çıktı: 9

# _Q4_ 
country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
# _Ans_
SELECT COUNT (country) FROM country
WHERE country LIKE ('_____');

Çıktı: 13
# _Q5_
city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
# _Ans_
SELECT COUNT (city) FROM city
WHERE city ILIKE ('%r');

Çıktı: 33
