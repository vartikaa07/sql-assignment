# sql-assignment

1)
select unique_key from `bigquery-public-data.austin_incidents.incidents_2008` where descript = 'DWI' LIMIT 10;

https://drive.google.com/file/d/1t3WCdwOOQRN13KhPM8brI-7nkLMPciEQ/view

2)
select address from `bigquery-public-data.austin_incidents.incidents_2008` LIMIT 10;
https://drive.google.com/file/d/1bs0CJB0QEx69CwTjWzXO2CsmK_XVbaTB/view

3)
select distinct descript from `bigquery-public-data.austin_incidents.incidents_2008` LIMIT 10;
https://drive.google.com/file/d/107dZA8L0wXLw7BIhwrispiN_7StDtp77/view

4)
select count(*) from `bigquery-public-data.austin_incidents.incidents_2008` where longitude is not null and latitude is not null and location is not null LIMIT 10;
https://drive.google.com/file/d/141B9_wZe9YRU-USeksKQciaxP4iSmnIV/view

5)
select date, time from `bigquery-public-data.austin_incidents.incidents_2008` where address like '5100%'LIMIT 10;
https://drive.google.com/file/d/1GjESiC64AEicsCiErTAiZBBKBhN19lSX/view

6)
select max(time) from `bigquery-public-data.austin_incidents.incidents_2008` LIMIT 10;
https://drive.google.com/file/d/1JuaOUICQYHpdEmLa1zUnYllcSYe7YWKx/view

7)select * from `bigquery-public-data.austin_incidents.incidents_2008` where descript = 'THEFT' and unique_key > 20082021744 LIMIT 10;
https://drive.google.com/file/d/1DOjH7Oyz5XiHNaTR0F3VbGhLIMrP4zg9/view

8)
select address from `bigquery-public-data.austin_incidents.incidents_2008` order by time desc limit 10;
https://drive.google.com/file/d/1W2Dnj3EcYL4q0nGrIQ_WHWE5o63Qqb2i/view


9)
#Joint Query
select * from `bigquery-public-data.austin_incidents.incidents_2008` t1 left join `bigquery-public-data.austin_incidents.incidents_2010` t2 on t1.time = t2.time where t1.time > '11:00:00' limit 10;

https://drive.google.com/file/d/1xM5s09BIhn3ccZ0fgfz_m8lkVMTziEtU/view?

10)
select t1.descript from `bigquery-public-data.austin_incidents.incidents_2008` t1, `bigquery-public-data.austin_incidents.incidents_2009` t2 where t1.latitude = t2.latitude and t1.longitude = t2.longitude limit 10;

https://drive.google.com/file/d/1iASQU3iVS0QXZiN6tzUpIDhR1isoBFJQ/view

