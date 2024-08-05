# ☕️ Coffee Sales Project

The Coffee Sales Excel Project aims to develop a comprehensive and interactive Excel dashboard to efficiently manage and analyze coffee sales data. 
This project will enable tracking of:
- Total sales overtime.
- Sales by country.
- Top 5 customers.

All the information regarding the case study has been sourced from [here](https://github.com/mochen862/excel-project-coffee-sales)

## Steps

### 1. Gather customer data using **XLOOK UP**

- From the `customers` page search the `Customer name`, `Email`, and `Country` information that matches the `Customer ID` in the `Orders` page.

```excel
=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,,0)
```

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/8ee1ce0b-6fff-401a-b3fa-83630b78d7e7">

- There are some `Customer ID` that do not have an `Email`. Only using the **XLOOK UP** formula will bring a '0' in those cases. To fix this, we can use thr **IF** fuction and if the returning value is equal to '0' then we are going to leave the cell empty.

```excel
=IF(XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0)=0,"",XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0))
```

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/e1b9c180-24cb-4d9e-bd84-f40320ab7bd9">
---

### 2. Use **INDEX** and **MATCH** to gather product data

- This way the search will be dynamic and we will have to write only one formula and then drag for the other columns.

- Use the **INDEX** function to select all `products` table as the range of cells to look into. Then to match the **row number** and **column number** use the **MATCH** formula.
- For the **row number** use a `Product ID` in the `orders` table as the 'lookup_value' and the entire `Product ID` column in the `products` page as the 'lookup_array'.
- For the **column number** use the headers for the columns `Coffee Type`, `Roast Type`, `Size`, and `Unit Price` in the `orders` table as the 'lookup_value' and the entire row of headers in the `products` page as the 'lookup_array'.

```excel
=INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!I$1,products!$A$1:$G$1,0))
```

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/cd906b8d-8f9b-4983-9421-3c4817205faf">
---

### 3. Calculate `Sales` column

- With a simple formula, calculate the `sale` column for all rows. The `sale` value is equal to `Unit Price` * `Quantity`.

```excel
=L2*E2
```

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/d09a38e3-8168-49fe-a635-286066b6af2b">
---

### 4. Create a new `Coffee Type Name` column using **IF** function

- Based on the `Coffee Type` column values, we will create a new `Coffee Type Name` column with the complete coffee type.
  - Rob = Robusta
  - Exc = Excelsa
  - Ara = Arabica
  - Lib = Liberica

```excel
=IF(I2="Rob","Robusta",IF(I2="Exc","Excelsa",IF(I2="Ara","Arabica",IF(I2="Lib","Liberica",""))))
```

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/a34593d0-a247-4ec1-b056-19ec2decaa79">
---


