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

### Dashboard

- Now that we have all the charts and information that is going to be added to the Dashboard, is time to build it.
- Create a new worksheet and bring all the charts, slicers and timeline.
- Bring them together in a way that the information that we want to present is clear and the slicers and timeline can be use without taking away from the data.
- One last thin to do is for the slicers and timeline to have a connection with the `Sales By Country` and `Top 5 Customers` charts.
  - To do this we can click in the timeline or slicer, then click in the corresponding tab, and then `Report Connections`.
  - Here select the other two charts.
    
    <img width="419" alt="image" src="https://github.com/user-attachments/assets/3e5bac9a-dc62-46a0-8e91-cdadd70537b7">

- All is left to do is add formating and color to the Dashboard so it has an appealing look but without taking away from the data which is the most important.

<img width="1233" alt="image" src="https://github.com/user-attachments/assets/8fec9464-9b12-4f57-ba2a-2504e7f1acfb">

















