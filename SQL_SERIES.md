**1.**

SELECT \* from customers where country='Brazil' or country='Italy';



**or**



SELECT \* from customers where country in ('Brazil', 'Italy');





**2.**



SELECT \* from customers where customername like '%son%';



**3.**

SELECT \* from Orders where Orderdate between '1996-10-01' and '1996-10-31' order by orderdate ASC;



**or**



SELECT \* from Orders where orderdate>='1996-10-01' and orderdate<='1996-10-31' order by orderdate ASC;



**or**



SELECT \* from Orders where month(OrderDate)=10 and year(Orderdate)=1996 order by orderdate ASC;



**or**



SELECT \* from Orders where orderdate like '1996-10-%' order by orderdate ASC;



**4.**

Select shipperid, count(\*) as total\_orders from orders group by Shipperid;



**5.**

SELECT \* from products where price>25;



**6.**

SELECT top 1 SupplierID, count(\*) as total\_supplies from products group by SupplierID ORDER BY count(\*) desc;

