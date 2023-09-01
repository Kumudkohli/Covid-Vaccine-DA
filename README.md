# COVID-19 Data Analysis SQL Queries
This repository contains a set of SQL queries designed to extract insightful information from COVID-19 datasets. The queries focus on analyzing various aspects of the pandemic, including infection rates, death percentages, vaccination progress, and more. By leveraging SQL, this repository offers a comprehensive understanding of the global COVID-19 situation, shedding light on key statistics and trends.

## Introduction
The SQL queries provided in this repository are intended to be executed on relevant COVID-19 datasets. These queries cover a wide range of analyses, from identifying infection rates to examining vaccination trends. By running these queries, you can gain valuable insights into the impact of the pandemic on different regions, countries, and continents.

## Data Sources
The analysis is performed on two main datasets:

- `coviddeaths$`: This dataset contains information related to COVID-19 cases, deaths, and population statistics for various locations around the world.

- `covidVaccines$`: This dataset provides data about COVID-19 vaccinations, including the number of new vaccinations administered per day for different locations.

## Query Highlights

1. Extract Data from Excel Files to SQL:

  - Retrieve COVID-19 data from the provided Excel files and load it into SQL.
  - Select relevant columns such as location, date, total cases, new cases, total deaths, and population.
  - Order the results by location and date.
2. Chances of Dying from COVID-19 in India:

  - Calculate the percentage chance of dying if contracted COVID-19 in India.
  - Display total cases, total deaths, and the calculated death percentage.
  - Filter the results for the location containing "India."
    
3. Percentage of Population Infected with COVID-19:

  - Calculate the percentage of the population that has been infected with COVID-19.
  - Display the location, maximum total cases, and the calculated population infection rate.
  - Group the results by location.
    
4. Death Count in Various Countries:

  - Calculate the total death count for each location (country).
  - Display the location and the maximum total deaths.
  - Exclude records with missing continent information.
  - Group the results by location and order them by total death count in descending order.
    
5. Continents with Highest Number of Deaths:

  -  Calculate the total death count for each continent.
  -  Display the continent and the maximum total deaths.
  -  Group the results by continent and order them by total death count in descending order.
    
6. Cases Count Per Day Since First Reported Case:

  - Calculate the total cases and total deaths per day since the very first COVID-19 case was reported.
  - Exclude records without continent information and where new cases are zero.
  - Group the results by date and order them by date.

7. Joining Two Tables:

  - Perform an inner join between the coviddeaths$ and covidVaccines$ tables using location and date as common columns.
  - Display all columns from both tables in the join result.

8.  Percentage of Population Vaccinated Daily:

  -  Calculate the percentage of the population that received vaccinations on a daily basis.
  -  Utilize a common table expression (CTE) to calculate rolling vaccination totals.
  -  Display continent, location, date, population, new vaccinations, rolling vaccination total, and the percentage of the population vaccinated.

9. Creating and Using Views:

  -  Create a view named rollingpopvac to encapsulate the calculation of rolling vaccination totals.
  -  Utilize this view to retrieve data, eliminating the need to rewrite the calculation each time.

## Getting Started
1. Clone this repository to your local machine using:
```
git clone https://github.com/your-username/covid-analysis-sql.git
```
2. Import the provided datasets (coviddeaths.xlsx and covidVaccines.xlsx) into your SQL database.

3. Execute the SQL queries provided in the repository in your SQL environment to explore COVID-19 data insights.

## Contributors
 Kumud Kohli - [GitHub Profile](https://github.com/kumudkohli)

Feel free to contribute to this project by opening issues or pull requests! Your contributions are highly appreciated in advancing our understanding of the COVID-19 pandemic through data analysis.





