<h1 align="center"> Hi there, I'm Jean 👋</h1>

<div align="center"> Welcome to my data space! I am Jean Rocha Santos, a Data Analyst and Analytics Engineer who loves turning complex, chaotic data into clear, actionable stories. I believe that a great data infrastructure isn't just about writing code—it's about empowering people to make better decisions without the headache.</div>

---

<h1 align="center"> About Me 🙎🏽‍♂️ </h1>

<div align="center"> My journey into data is a bit unique. I started with a strong foundation in Business and Finance, and later dived deep into technology with a Postgraduate degree covering foundational computer science topics in Ireland. Because of this hybrid background, I don't just build data pipelines or write SQL queries—I actually understand the business impact behind the numbers. Whether I'm building an Executive Cockpit for a CEO or orchestrating a complex data architecture, my goal is always the same: to bridge the gap between raw data and real-world strategy.</div>

---

<h1 align="center"> Technical Projects & Architecture 📈 </h1>

## 📊 Presentation — PowerApps & Dataverse: Enterprise Ticketing System

Here is a look behind the scenes of an enterprise ticketing system I built. This presentation showcases the backend architecture, relational database design, and automated workflows that make the system tick.
<img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Captura de tela 2026-01-28 200346.png"></img>
[![PowerApps - Ticketing System Presentation]](https://www.canva.com/design/DAG_u5GstUY/PJO_gJiPljeSZlkG3JqSyg/view?utm_content=DAG_u5GstUY&utm_campaign=designshare&utm_medium=embeds&utm_source=link)

---

### 🗺️ Geospatial Optimization: The Square Analysis 
👉 **[Live Power BI Report Here](https://app.powerbi.com/reportEmbed?reportId=fc7abf58-d2d1-4802-9bfc-ccd80abb21ad&autoAuth=true&ctid=30cb66b6-2919-4c93-b208-6b8e8cefdd39/)**

Have you ever needed to calculate the exact distance between hundreds of locations dynamically? I tackled this logistical challenge by implementing the **Haversine Formula** natively in DAX. It processes geographical coordinates (Latitude/Longitude) on the fly, allowing users to effortlessly compare student density and average ticket prices within a specific radius.

<p align="center">
  <kbd>
    <img src="https://github.com/jean-rocha1/MyPortfolio/blob/main/Design%20sem%20nome.gif"></img>
  </kbd>
</p>

*A peek at the core DAX logic:*
```csharp
Principal Dax = 
var Rad_lat1 = selectedvalue ( Origem[Latitude] ) / 57.2957795
var Rad_lat2 = selectedvalue ( Fat_Organization[Latitude] ) / 57.2957795
var Rad_long1 = selectedvalue ( Origem[Longitude] ) / 57.2957795
var Rad_long2 = selectedvalue ( Fat_Organization[Longitude] ) / 57.2957795
var x = round (
        sin ( Rad_lat1 ) * sin ( Rad_lat2 )
        + cos ( Rad_lat1 ) * cos ( Rad_lat2 )
            * cos ( Rad_long1 - Rad_long2 ),
        15
    )
var vTerra = 6371
return acos ( x ) * 6371

````
### 👔 Executive Cockpit & Financial Modeling
This is one of the projects I am most proud of. I developed a mission-critical financial and operational data pipeline for C-level leadership.

* **The Challenge:** The company's data was fragmented across different departments.
* **The Solution:** I consolidated complex pipelines (Growth, Finance, HR) into a single, unified "source of truth."
* **The Impact:** It significantly enhanced strategic planning and financial transparency, aligning company goals with core OKR methodologies.

*Handling conditional financial metrics (DAX):*
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
### ⚙️ Supply Chain Integration Pipeline
I built this enterprise-grade application to solve a real-world headache: distributing operational materials efficiently across a massive nationwide network.

* By connecting a centralized CRM with a unified SQL database infrastructure, the Commercial Operations team was able to process orders seamlessly, resulting in a **70% reduction in operational time**.

---

### 📈 Predictive Sales Modeling & Marketing ROI
* **Sales Forecasting:** Designed an automated predictive data model using SQL and Power BI to optimize sales strategies, reducing manual forecasting effort by 40%.
* **Marketing Analytics:** Built targeted SQL reporting layers that helped the team improve email engagement by 20% and boost campaign sales by 15%.

---
🌱 **Currently exploring & learning:** Advanced Data Engineering pipelines (dbt, Apache Airflow) and Cloud Infrastructure (GCP).

---

## 🛠️ My Tooling & Languages

* **Languages:** ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
* **Databases & Environments:** ![Dataverse](https://img.shields.io/badge/Microsoft_Dataverse-0066B3?style=for-the-badge&logo=microsoft) ![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
* **BI & Devops:** ![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

📬 **Let's Connect:** 
* LinkedIn: [@jean-rocha](https://linkedin.com/in/jean-rocha)

Feel free to explore my repositories to see more projects and code samples!

---
&copy; 2026 Jean Rocha Santos
