# 🌐 AWS COVID Analysis Project 

## Project Description
Explore and visualize COVID-19 data insights using Amazon Web Services (AWS) and QuickSight. This repository contains a data analytics dashboard leveraging AWS services to analyze and visualize key trends related to COVID-19.

## Features
- Interactive visualizations showcasing pandemic metrics.
- Utilization of AWS services: RDS, S3, EC2, and QuickSight.
- Data storage, processing, and dashboard creation.
  
## Objectives
Familiarization with Data Storage: This project aimed to provide a hands-on learning experience in managing data storage using AWS services like Amazon RDS (Relational Database Service) and S3 (Simple Storage Service). It involved understanding how to create databases, store datasets, and manage data within the AWS ecosystem.

Understanding Data Processing: The project sought to gain knowledge about processing data effectively using tools such as MySQL and AWS services like EC2 (Elastic Compute Cloud). It involved tasks like data importation, data transformation, and running MySQL queries to process and manage the COVID-19 dataset.

Exploration of Cloud Computing: The primary objective was to gain familiarity with cloud computing principles, particularly within the AWS environment. It involved understanding how to leverage cloud-based resources (such as instances, storage, and services) to perform data-related tasks, including analysis and visualization.

## Getting Started

## 1. Data Collection Details:
Obtained the COVID-19 dataset from [Our World in Data](https://ourworldindata.org/covid-cases), a scientific online publication addressing global challenges like poverty, disease, hunger, climate change, war, existential risks, and inequality.

## 2. Creating Table on Amazon RDS (MySQL):
1. Log into EC2 instance on Amazon Linux and install MySQL
2. Create a new database: `CREATE DATABASE covid_data;`
3. Select the database: `USE covid_data;`
4. Create a table named `covid_cases` to store the dataset. 

```sql
CREATE TABLE covid_cases (
    iso_code VARCHAR(10),
    continent VARCHAR(50),
    location VARCHAR(100),
    date DATE,
    total_cases INT,
    new_cases INT,
    ...
);
