<h1 align="center"> Hi there, I'm Jean👋</h1>

<div align="center"> Welcome to my portfolio! I am a Data Analyst with specializing in data visualization, business intelligence, and creating actionable insights. My expertise includes tools like Power BI, SQL, and Python, which I use to transform complex data into clear, impactful narratives that drive business decisions.</div>

---


<h1 align="center"> About Me 🙎🏽‍♂️ </h1>

<div align="center"> I have worked on numerous impactful projects, including building predictive sales models, analyzing marketing data, and developing operational dashboards. My goal is to empower businesses with data-driven strategies and improve decision-making processes.</div>

---

<h1 align="center"> Projects 📈 </h1>

👉 [Ver apresentação incorporada](./SmartThingProject.html)

- ### Sales Forecasting Model
  - **Tools Used:** Power BI, SQL
  - **Highlights:** Built a predictive model to enhance sales strategies, reducing manual effort by 40%.

- ### Marketing Data Analysis
  - **Tools Used:** SQL, Power BI
  - **Highlights:** Improved email engagement by 20% and increased campaign sales by 15%.
 
 <p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Captura%20de%20tela%202025-01-26%20221207.png"></img>
  </kbd>
</p> 

- ### Operational Efficiency Dashboard
  - **Tools Used:** Power BI
  - **Highlights:** Developed a unified dashboard for the CEO, integrating data from multiple departments for real-time monitoring, this tool enhanced operational efficiency, aligned with OKR strategies, and improved overall performance visibility for leadership.

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/V%C3%ADdeo%20sem%20t%C3%ADtulo%20(1).gif"></img>
  </kbd>
</p>

DAX
```csharp
Principal Dax =
dbl_faturamento_juncao_probabilidade_BX =
var faturamento_lojinha = [dbl_faturamento_gerencial_lojinha]
var faturamento_car = [dbl_faturamento_bruto_car_probabilidade]
var faturamento_potencial =
    calculate (
        1100 * sum ( fato_Negocios_funil_last_date[quantidade_produtos] ),
        fato_Negocios_funil_last_date[fk_etapa_funil] > 4,
        fato_Negocios_funil_last_date[business_unit] = "GROWTH"
    )
var faturamento_potencial7k =
    calculate (
        1100 * sum ( fato_Negocios_funil_last_date[quantidade_produtos] ),
        dim_Organizacoes[Escolas_Trabalhar_7000.Carteira 2023] <> ""
    )
var faturamento_potencial_geral =
    calculate ( 1100 * sum ( dim_Organizacoes[alunos_TT] ) )
return
    switch (
        selectedvalue ( 'Tipo de dado'[Value] ),
        "Lojinha", faturamento_lojinha,
        "Contrato", faturamento_car,
        "Potencial Conversão", faturamento_potencial,
        "Potencial 7k", faturamento_potencial7k,
        faturamento_potencial_geral
    )


````
- ### Square Analysis, **[click here](https://app.powerbi.com/reportEmbed?reportId=fc7abf58-d2d1-4802-9bfc-ccd80abb21ad&autoAuth=true&ctid=30cb66b6-2919-4c93-b208-6b8e8cefdd39/)**.
  This project enables users to accurately determine the distance between a selected school and nearby schools. The information provided includes the number of pupils in each school, their locations, and the average ticket price. This allows for a comprehensive and effortless comparison of schools within a specific radius.

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Design%20sem%20nome.gif"></img>
  </kbd>
</p>

DAX
```csharp
Principal Dax = 
var Rad_lat1 =
    selectedvalue ( Origem[Latitude] ) / 57.2957795
var Rad_lat2 =
    selectedvalue ( Fat_Organization[Latitude] ) / 57.2957795
var Rad_long1 =
    selectedvalue ( Origem[Longitude] ) / 57.2957795
var Rad_long2 =
    selectedvalue ( Fat_Organization[Longitude] ) / 57.2957795
var x =
    round (
        sin ( Rad_lat1 ) * sin ( Rad_lat2 )
            + cos ( Rad_lat1 ) * cos ( Rad_lat2 )
                * cos ( Rad_long1 - Rad_long2 ),
        15
    )
var vTerra = 6371
return
    acos ( x ) * 6371

````
- ### Power Apps

  A Power Apps application has been developed for requesting promotional items and materials for events organized by consultants and distributed nationwide across Brazil. This application establishes a direct connection with the company's CRM and utilizes a standardized unified database, enabling the Commercial Operations team to efficiently process orders. This streamlined approach has resulted in a reduction of operational time by over 70%.

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Design%20sem%20nome%20(1).gif"></img>
  </kbd>
</p>


- LinkedIn: [@jean-rocha](https://linkedin.com/in/jean-rocha)

- ### SQL 
  - ### Challenge 1 

**[THE PADS] ( https://www.hackerrank.com/challenges/the-pads/problem)**  

### Result
```SQL 
SELECT CONCAT(NAME, '(', LEFT(OCCUPATION, 1), ')')
FROM OCCUPATIONS
ORDER BY NAME;


SELECT CONCAT('There are a total of ', COUNT(OCCUPATION), ' ', LOWER(OCCUPATION), 's.')
FROM OCCUPATIONS
GROUP BY OCCUPATION
ORDER BY COUNT(OCCUPATION), LOWER(OCCUPATION);
```

- ### Python, 

```Python 
### version

!python -V

# 1.3 arrays Numpy

import numpy as np

km = np.loadtxt('carros-km.txt')

km

anos = np.loadtxt('carros-anos.txt', dtype = int)

anos

### Obtaining the average mileage per year

km_media = km / (2022 - anos)

km_media

type(km_media)

```

### Variable declaration


```Python 
ano_atual = 2019
ano_fabricacao = 2003
km_total = 44410.0

Year_Now

manufacturing_year

km_total

# $$km_{averange} = \frac {km_{total}}{(Year_{now} - Year_{manufacturing})}$$

km_media = km_total // (ano_atual - ano_fabricacao)

km_media


### Multiple declaration

current_year = 2019
year_manufactured = 2003
km_total = 44410.0

current_year, manufacturing_year, km_total = 2020 , 2019 , 4888.0

current_year

km_total




```
---
Visit my repositories to explore more projects and code samples.
---
## Icons and Tools

- **Languages:** ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
- **Visualization Tools:** ![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
- **Other Skills:** ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

&copy; 2024 Jean Rocha Santos
