# 🏎️ Formula 1 Data Pipeline Project

Hi there! 👋 Welcome to my Formula 1 Data Pipeline project. 

If you are a fan of Formula 1 or just interested in how data engineering works in the real world, you are in the right place! This project is all about taking raw racing data and transforming it into something we can use to answer fun questions (like who the best drivers and teams are).

## 🌟 What is this project?

In simple words, this project takes raw data (like CSV and JSON files containing race results, driver info, and lap times) and processes it using **Azure Databricks**. 

Think of it like a factory:
1. **Raw Material (Bronze Layer 🥉):** We bring in the raw, messy data exactly as it is. 
2. **Refining (Silver Layer 🥈):** We clean up the data, remove bad records, and connect different pieces of information together.
3. **Finished Product (Gold Layer 🥇):** We summarize the data so it's ready to be plugged into dashboards to show the final race results and standings.

## 📁 What's inside this repository?

I have organized the files to make it easy to navigate:
- **`formula1-project/`**: This folder contains the code for the first time we load all the historical data.
- **`formula1-project-incremental-load/`**: Formula 1 has new races all the time! This folder has the code that only processes the *new* data every race weekend, so we don't have to process the old data all over again.
- **`data/`**: The raw data files we use as our starting point.
- **`docs/`**: Check out the `images` folder here! It contains diagrams that show exactly how our data is connected at every step of the factory.

## 🚀 How to read the code

If you want to see how the magic happens, start by opening the `formula1-project` folder:
1. `01-setup`: How we get everything ready to run.
2. `02-bronze` ➡️ `03-silver` ➡️ `04-gold`: Follow the data as it gets cleaned up step-by-step!
3. `05-analytics`: Where we finally ask the data questions (like finding the most dominant drivers).
4. `06-orchestration`: How we automate this entire process to run on a schedule.

---
*Note: I built this project while learning Azure Databricks. It's a great showcase of building a real-world, automated data pipeline!*