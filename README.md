# ☕️ Coffee Sales Project

The Coffee Sales Excel Project aims to develop a comprehensive and interactive Excel dashboard to efficiently manage and analyze coffee sales data. 
This project will enable tracking of:
- Total sales overtime.
- Sales by country.
- Top 5 customers.

All the information regarding the case study has been sourced from [here](https://github.com/mochen862/excel-project-coffee-sales)

## Steps

1. Gather customer data using **XLOOK UP**:

- From the `customers` page search the `Customer name`, `Email`, and `Country` information that matches the `Customer ID` in the `Orders` page.
  
  <img width="500" alt="image" src="https://github.com/user-attachments/assets/8ee1ce0b-6fff-401a-b3fa-83630b78d7e7">

- There are some `Customer ID` that do not have an `Email`. Only using the **XLOOK UP** formula will bring a '0' in those cases. To fix this, we can use thr **IF** fuction and if the returning value is equal to '0' then we are going to leave the cell empty.

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/e1b9c180-24cb-4d9e-bd84-f40320ab7bd9">

3. Use **INDEX MATCH** to gather product data.

- Using the **INDEX** function

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/cd906b8d-8f9b-4983-9421-3c4817205faf">



