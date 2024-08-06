# Pivot Tables and Data Visualization

### Total Sales

- Create a new **Pivot Table** from the `orders` table.
- Drag the `Order Date` to the `Rows` area.
  - Change the grouping to `Years` and `Months`.

  <img width="346" alt="image" src="https://github.com/user-attachments/assets/e3fcfd71-b7ec-4077-9bb2-341878af574a">

- In the `Design` tab:
  - Change the **Report Layout** to a **Tabular Form**.
  - Turn **OFF** the **Grand Totals** for rows and columns.
  - Turn **OFF** the **Subtotals**.

- Drag `Coffee Type Names` into the `Columns` area.
- Drag `Sales` into the `Values` area.
  - Change the formating to use the 1000 separator.
  - Use 0 decimal places.

- The final pivot table will look like this:

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/32afc9a0-d448-4aff-ab3d-4d3ceb06abbf">

- From this pivot table, we can create a Line Chart.
  - Format the Line Chart so that the information that we want to show is clear.

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/90222b1c-f2bb-43f4-82ef-408469eaadde">
---

### Insert Time Line 

- This timeline is importat because we will use it to manipulate and filter all the charts in the dashboard.
- From the `PivotChart Analyse` tap, select the button `Insert Timeline` and check the `Order Date` box.

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/4b5de227-7035-473d-9533-c5204366b6ae">
---

### Insert Slicers 

- From the `PivotChart Analyse` tap, select the `Insert Slicer` option.
- The slicers to create are `Roast Type`, `Size` and `Loyalty Card`.

  <img width="330" alt="image" src="https://github.com/user-attachments/assets/890505e1-f712-4a32-a282-0d9a96cf59b4">
---

### Country Bar Chart

- Duplicate the worksheet with the Pivot Table from `Total Sales`.
- In the `PivotTable Fields` bring the `Country` field into the `Rows` area, and leave `Sales` in the `Values` area.
- Insert a **Bar Chart** and format.

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/16414daa-9b42-4b6b-89a4-e7ec7b0332d6">
---

### Top 5 Customers Bar Chart

- Duplicate the worksheet with the Pivot Table from `Total Sales`.
- In the `PivotTable Fields` bring the `Customer Name` field into the `Rows` area, and leave `Sales` in the `Values` area.
- Filter by the **Top 5** and sort the results based on the `Sum of Sales`.
- Insert a **Bar Chart** and format.

  <img width="500" alt="image" src="https://github.com/user-attachments/assets/3c312f0f-d223-45e4-996d-9cf9247f3441">
---






















