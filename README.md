<h1 align="center"> Hi there, I'm Jean👋</h1>

## Data Analyst Portfolio

Welcome to my portfolio! I am a Data Analyst with specializing in data visualization, business intelligence, and creating actionable insights. My expertise includes tools like Power BI, SQL, and Python, which I use to transform complex data into clear, impactful narratives that drive business decisions.

---

## About Me

I have worked on numerous impactful projects, including building predictive sales models, analyzing marketing data, and developing operational dashboards. My goal is to empower businesses with data-driven strategies and improve decision-making processes.

---

## Contact

Feel free to reach out via email at [jean.rsantos1@gmail.com](mailto:jean.rsantos1@gmail.com).

Or connect with me on [LinkedIn](https://linkedin.com/in/jean-rocha).

---

## Projects

### Sales Forecasting Model
- **Tools Used:** Power BI, SQL
- **Highlights:** Built a predictive model to enhance sales strategies, reducing manual effort by 40%.

### Marketing Data Analysis
- **Tools Used:** SQL, Power BI
- **Highlights:** Improved email engagement by 20% and increased campaign sales by 15%.

### Operational Efficiency Dashboard
- **Tools Used:** Power BI
- **Highlights:** Developed a unified dashboard for the CEO, integrating data from multiple departments for real-time monitoring.



## Square Analysis, **[click here](https://app.powerbi.com/reportEmbed?reportId=fc7abf58-d2d1-4802-9bfc-ccd80abb21ad&autoAuth=true&ctid=30cb66b6-2919-4c93-b208-6b8e8cefdd39/)**.
This project enables users to accurately determine the distance between a selected school and nearby schools. The information provided includes the number of pupils in each school, their locations, and the average ticket price. This allows for a comprehensive and effortless comparison of schools within a specific radius. 

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Design%20sem%20nome.gif"></img>
  </kbd>
</p>

```DAX
Principal Dax = 
VAR Rad_lat1 =
    SELECTEDVALUE ( Origem[Latitude] ) / 57.2957795
VAR Rad_lat2 =
    SELECTEDVALUE ( Fat_Organization[Latitude] ) / 57.2957795
VAR Rad_long1 =
    SELECTEDVALUE ( Origem[Longitude] ) / 57.2957795
VAR Rad_long2 =
    SELECTEDVALUE ( Fat_Organization[Longitude] ) / 57.2957795
VAR x =
    ROUND (
        SIN ( Rad_lat1 ) * SIN ( Rad_lat2 )
            + COS ( Rad_lat1 ) * COS ( Rad_lat2 )
                * COS ( Rad_long1 - Rad_long2 ),
        15
    )
VAR vTerra = 6371
RETURN
    ACOS ( x ) * 6371

````
## Power Apps


A Power Apps application has been developed for requesting promotional items and materials for events organized by consultants and distributed nationwide across Brazil. This application establishes a direct connection with the company's CRM and utilizes a standardized unified database, enabling the Commercial Operations team to efficiently process orders. This streamlined approach has resulted in a reduction of operational time by over 70%.

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Design%20sem%20nome%20(1).gif"></img>
  </kbd>
</p>


- LinkedIn: [@jean-rocha](https://linkedin.com/in/jean-rocha)

## SQL 
# Challenge 1 

**[THE PADS] ( https://www.hackerrank.com/challenges/the-pads/problem)**  

# Result
```SQL 
SELECT CONCAT(NAME, '(', LEFT(OCCUPATION, 1), ')')
FROM OCCUPATIONS
ORDER BY NAME;


SELECT CONCAT('There are a total of ', COUNT(OCCUPATION), ' ', LOWER(OCCUPATION), 's.')
FROM OCCUPATIONS
GROUP BY OCCUPATION
ORDER BY COUNT(OCCUPATION), LOWER(OCCUPATION);
```

## Python, 

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


Visit my repositories to explore more projects and code samples.


---

## Icons and Tools

- **Languages:** ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
- **Visualization Tools:** ![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
- **Other Skills:** ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

&copy; 2024 Jean Rocha Santos
