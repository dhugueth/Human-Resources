# Human Resources 

To access the report [click here](https://app.powerbi.com/view?r=eyJrIjoiYWQwODlkYTYtMDRmYi00ODg2LThmZjYtMzA3OGQ2NjcwZTQyIiwidCI6ImJhYjBiNjc5LWJkNWYtNGZlOC1iNTE2LWM2YjhiMzE3Yzc4MiIsImMiOjR9)

## What was used? 

The project was developed and published using Power BI, one of the top leader in business Intelligence.

### Data

_The data used was provided for educational purposes by Power BI - Data Analysis and Business Intelligence course on the Udemy platform._

- [Datos Empleados.xlsx](https://github.com/dhugueth/Recursos-Humanos/files/7570979/Datos%2BEmpleados.xlsx)

A free theme by the University of Melbourne and a pre-established background given in the course was used. 

### Data Preparation

Modifications were made to the original data using the Power Query editor to be able to use them appropriately. 

The modifications were: 

- The original data in "Género" column of the "Tabla Empleados" sheet was replaced from English to Spanish.
- The original data in "Departamento" column of the "Tabla Empleados" sheet was replaced from English to Spanish.
- The original data in "Posición" column of the "Tabla Empleados" sheet was replaced from English to Spanish.
- The column "Nombre Empleado" of the "Tabla Empleados" sheet is modified to change the order of last name and first name.
  - The option split column by delimiter is used to separate the name in one column and the last name in another column.
  - Once separated into two columns, both columns are selected with Ctrl.
  - Merge Columns option is used to return the information to a single column but now with the desired order 

## Data Modeling

It was required to relate common data between the files:

- The data named "ID Empleado" of the "Tabla Empleados" and "Tabla sueldo" sheet were related. 
- The data named "ID Empleado" of the "Tabla Empleados" and "Tabla Evaluación" sheet were related. 

**DAX - Data Analysis Expressions**

- A new measure was created using `COUNTROWS` function in "Tabla Empleados" sheet.
- A new measure was created using `AVERAGE` function in "Tabla Sueldo" sheet.
- A new measure was created using `AVERAGE` function in "Tabla Evaluación" sheet.
- A new column was created using `INT`, `YEARFRAC` and `TODAY` functions in "Tabla Empleados" sheet 
- A new measure was created using `AVERAGE` function in "Tabla Empleados" sheet.
- A new column was created using the conditional `IF` in "Tabla Empleados" sheet.
- A new column was created using the conditional `IF` in "Tabla Sueldo" sheet.
- A new column was created using the conditional `IF` in "Tabla Evaluación" sheet.

## Description

For the human resources report different visualizations such as map, card, buttons, donut chart, stacked bar chart, stacked column chart, table, and scatter chart were used to make the exposed analysis 


https://user-images.githubusercontent.com/93662295/142662794-b8b290f2-571a-456f-a8c3-8232da5b06d6.mp4

https://user-images.githubusercontent.com/93662295/142662814-939b17e2-500b-4c56-9192-62cf55985a0a.mp4

https://user-images.githubusercontent.com/93662295/142662959-2726e2a5-7319-4360-8b10-525efa017994.mp4
