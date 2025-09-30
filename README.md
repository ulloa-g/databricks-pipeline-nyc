# databricks-pipeline-nyc

### 1. Crea una cuenta en [databricks](https://www.databricks.com/).

![](img/01_create_acc.png)

### 2. Crea una carpeta y un notebook nuevo en python

![](img/02_create_notebook.png)

### 3. Datos

Vamos a trabajar con un documento gubernamentales de la comisión de taxis y limusinas de la ciudad de Nueva York - Estados Unidos. 

Vamos a aprovechar que **Databricks** nos brinda una tabla alojada en Amazon S3 con estos datos. 
![](img/03_data.png)
Si quieres puedes descargar la información localmente y conocer más [aquí](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page).

Adicional a esta información, vamos a trabajar con un archivo **.csv** que tenemos alojado en este repositorio ```/databricks-pipeline-nyc/input_data/nyc_zip_borough_neighborhoods_pop.csv```. Este archivo contiene columnas para codigo postal y los nombres de los barrios que corresponden. Esta información nos servirá para cruzar información con la tabla alojada en *Databricks*.

Para cargar esta información y convertirla en una tabla sigue los siguientes pasos:

![](img/04_local_data.png)

Arrastra el archivo **nyc_zip_borough_neighborhoods_pop.csv**
![](img/05_local_data2.png)

Cambia el nombre de la tabla a: **nyc_zip_codes**. Luego click en **Create table**. Más tarde haremos uso de esta información.
![](img/06_local_csv_to_table.png)

### 4. ETL + EDA
Importa el archivo ```/notebook/databricks-pipeline-nyc.ipynb```

![](img/07_import_notebook.png)
