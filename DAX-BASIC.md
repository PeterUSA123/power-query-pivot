# Tìm hiểu về hàm trong DAX

> Hàm FILTER (lọc dữ liệu từ bảng với điều kiện)
`FILTER(<table>,<filter>)`
>Count of sales orders over 100 = COUNTROWS(FILTER('Sales', 'Sales'[Sales] > 100))

> Hàm ALL
`ALL(<table> or <column>)`
`Count of all sales orders = COUNTROWS(ALL('Sales'))`

> Hàm RELATED
`RELATED(<column>)`
Count of sales orders in the `US = COUNTROWS(FILTER(ALL('Sales'), RELATED('SalesGeography'[Countries]) = "United States"))`

> TOTALYTD / TOTALQTD / TOTALMTD
`TOTALYTD(<expression>,<dates>[,<filter>][,<year_end_date>])`
`Total sales this year = TOTALYTD(SUM('Sales'[Sales]), 'Dates'[Dates])`

> CALCULATE 
`CALCULATE(<expression>, <filter1>,<filter2>…)`
Sum of sales all countries = CALCULATE(SUM('Sales'[Sales]),ALL('SalesGeography'))

Để viết biểu thức ta dùng cấu trúc
Tên_cột:=<biểu thức>
