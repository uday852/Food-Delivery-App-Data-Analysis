🍽️ Zomato Data Analysis using Python

📌 Overview



This project analyzes restaurant data from Zomato to understand customer dining preferences, online ordering trends, pricing patterns, and restaurant ratings. The analysis was performed using Python and popular data analytics libraries to extract meaningful insights and visualize key patterns in the dataset.



The goal of this project is to demonstrate how data analytics can help businesses understand consumer behavior and make data-driven decisions.



📂 Dataset



The dataset contains information about restaurants listed on the Zomato platform.



* Dataset Features



* Restaurant Name



* Online Order Availability



* Table Booking Option



* Customer Rating



* Number of Votes



* Approximate Cost for Two People



* Restaurant Category (Dining / Cafe / Others)



Dataset Size



* Rows: 148



* Columns: 7



🛠 Tools \& Technologies



* 🐍 Python



* 📊 Pandas



* 🔢 NumPy



* 📉 Matplotlib



* 🎨 Seaborn



* 📓 Jupyter Notebook / Google Colab



⚙️ Project Workflow



1️⃣ Data Loading



The dataset was imported into Python using Pandas for initial analysis.



import pandas as pd

dataframe = pd.read\_csv("Zomato data.csv")



2️⃣ Data Cleaning



* Converted the rating column into numeric format



* Checked for missing values



* Verified dataset structure and data types



Example transformation:



def handleRate(value):

&#x20;   value = str(value).split('/')

&#x20;   return float(value\[0])



dataframe\['rate'] = dataframe\['rate'].apply(handleRate)



3️⃣ Exploratory Data Analysis (EDA)



* Key analyses performed:



* Restaurant category distribution



* Most popular restaurant based on votes



* Online vs offline ordering trends



* Restaurant rating distribution



* Cost preferences for couples



* Customer engagement based on restaurant type



📊 Visualizations



The project includes several visualizations:



* 📉 Countplots to analyze restaurant categories and online ordering trends



* 📊 Histograms to understand rating distribution



* 📦 Boxplots to compare ratings for online vs offline orders



* 🔥 Heatmaps to visualize relationships between restaurant types and online orders



These visualizations help identify patterns and trends in the dataset.



🔍 Key Insights



* Most restaurants fall under the Dining category.



* The restaurant with the highest votes is Empire Restaurant.



* A majority of restaurants do not support online ordering.



* Most restaurant ratings fall between 3.5 and 4.0.



* Couples prefer restaurants with an approximate cost of ₹300 for two people.



* Cafes tend to receive more online orders, while dining restaurants rely more on offline visits.



🚀 Project Outcome



This project demonstrates how Python can be used to perform data cleaning, exploratory data analysis, and visualization to uncover insights about customer behavior and restaurant performance.



The insights generated from this analysis can help restaurants and food delivery platforms optimize pricing strategies, improve customer experience, and understand market trends.



▶️ How to Run the Project



1️⃣ Clone the Repository



git clone https://github.com/yourusername/zomato-data-analysis.git

2️⃣ Install Required Libraries



pip install pandas numpy matplotlib seaborn



3️⃣ Run the Notebook



Open the project in Jupyter Notebook or Google Colab and execute the cells to reproduce the analysis.



📁 Project Structure

Zomato-Data-Analysis

│

├── dataset

│   └── zomato\_data.csv

│

├── notebook

│   └── zomato\_analysis.ipynb

│

├── images

│   └── visualizations

│

└── README.md



⭐ Goal of this project: Demonstrate practical skills in Python-based data analysis, data visualization, and exploratory data analysis (EDA).

