# SQL Analysis of COVID-19 Death Data

## Project Description
This project involves analyzing COVID-19 death data using SQL. The dataset, sourced from [Our World in Data](https://ourworldindata.org/covid-deaths), contains global COVID-19 death statistics. The goal of the project is to perform various SQL queries to extract meaningful insights from the data, such as total deaths by country, death rates over time, and comparisons between different regions.

## Technologies Used
- SQL 
- Python

## Dataset Information
The dataset used in this project is from [Our World in Data](https://ourworldindata.org/covid-deaths) and contains global data on COVID-19 deaths. Some of the key columns include:
- `iso_code`: Country or region code
- `location`: Name of the country or region
- `date`: Date of the recorded data
- `total_deaths`: Cumulative number of deaths
- `new_deaths`: Number of new deaths on a given day

## Project Structure
- `sql_queries.sql`: Contains the SQL queries used to analyze the COVID-19 death data.
- `README.md`: Documentation of the project.

## SQL Queries
1. Total COVID-19 deaths by country:
   ```sql
   SELECT location, SUM(total_deaths) as total_deaths
   FROM covid_deaths
   GROUP BY location
   ORDER BY total_deaths DESC;


