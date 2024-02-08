
--------------------------------------------TSQL-----------------------------------
    
	------------------------------DISTINCT COUNT OF SALES YEARS-------------------------------
                        SELECT  DISTINCT 
                        YEAR( Order_Date)
                       FROM [Sales Data.xls - Orders]
-----------------------------------------------------------------------------------------------------------
    -----------------IN YEAR 2019 THE TOTAL  SALES ARE 494.040.211559594.........................               
					   SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2019'
-----------------------------------------------------------------------------------------------------------------
     ---------------IN THE YEAR 2020 TOTAL SALES ARE 472.2993.031299055------------------------------------               
					SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2020'
--------------------------------------------------------------------------------------------------------------------------
  ------------------IN THE YEAR 2021 TOTAL SALES ARE 613.933.578229964-----------------------------------------                  
					SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2021'
-------------------------------------------------------------------------------------------------------------------
   ---------------------IN THE YEAR 2022 TOTAL SALES ARE 745.567.528743744------------------------                 
					SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2022'
------------------------------------------------------------------------------------------------------------------------------
 ----------YEAR 2019 THE HIGHEST SALE MONTH IS SEPMTEMBER WITH THE SALES OF 82K PLUS----------------------------------			
				     SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2019' AND MONTH(Order_Date)='9'
-------------------------------------------------------------------------------------------------------------------------------
  -----------YEAR 2020 THE HIGEHST SALES MONTH IS NOVEMBER WITH THE SALES OF 75K PLUS---------------------                    
					  SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2020' AND MONTH(Order_Date)='11'
-----------------------------------------------------------------------------------------------------------------------------
  -------------YEAR 2021 THE HIGEHST SALES MONTH IS DECEMBER WITH THE SALES OF 97K PLUS----------------------                 
				   SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2021' AND MONTH(Order_Date)='12'
------------------------------------------------------------------------------------------------------------------------------
 -------------YEAR 2022 THE HIGEHST SALE MONTH IS SEMPTE  MBER WITH THE SALES OF 88K PLUS--------------------               
				  SELECT SUM(SALES)
					   FROM [Sales Data.xls - Orders]
					   WHERE  YEAR(Order_Date) = '2022' AND MONTH(Order_Date)='9'
-------------------------------------------------------------------------------------------------------------------------------
  -----------------------THE TOTAL REVENUE FOR THE WHOLE YEARS 2.6M PLUS---------------------------
                                          SELECT SUM(Sales)
                                                 + 
										 SUM(Profit ) AS TOTALREVENUE

                                         FROM [Sales Data.xls - Orders]
----------------------------------------------------------------------------------------------------------------------------
  ---------------------------------------TOTAL SALES FOR THE WHOLE YEAR-- 2.3M PLUS--------------------------------                       
						 SELECT SUM(Sales)
							 FROM [Sales Data.xls - Orders]
--------------------------------------------------------------------------------------------------------------------------------
------------TOTAL PROFIT FOR TH WHOLE YEAR-- 292K PLUS------------------------------------
                           SELECT SUM( Profit)
				         FROM [Sales Data.xls - Orders]
