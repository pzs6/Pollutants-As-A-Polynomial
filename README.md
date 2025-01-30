# Pollutants-As-A-Polynomial
## Table of Contents
1. [About this project](#about-this-project)
2. [Source of data](#source-of-data)
3. [Data cleaning and formatting](#data-cleaning-and-formatting)
4. [Data Modeling, Evaluation and Visualization](#data-modeling-evaluation-and-visualization)
5. [Results](#results)



## About this project
🔍 **Project Objective:** Analyze how nitrogen oxides (NOx) emissions have changed in the Guadalajara Metropolitan Area (AMG) over the past 20 years and what insights an intelligent model can provide about their evolution. A machine learning model will be used to process and understand the evolution of these pollutants.  🚀

🔥 **Why NOx?**  
- They mainly come from the burning of fossil fuels. ⛽🚗  
- They have a significant environmental impact (acid rain, smog, etc.). 🌍💨  
- They affect human health (respiratory issues, lung inflammation). ⚠️ 

## Source of data
 
- Historical data from the **Secretaría de Medio Ambiente y Desarrollo Territorial de Jalisco (SEMADET)**.  
- **Public** and **free** access.  

📥 **Data Format:**  
- Available in **Excel**, divided by year.  
- Contains **hourly and daily** measurements of pollutants and **meteorological variables**.  
- Measurements come from various **meteorological stations** in the city of Guadalajara.  

## Data cleaning and formatting
Python was used, with NumPy and Pandas as the main tools.  

📍 **Data Selection:**  
- Only NOx measurements were used.  
- Data was filtered from the most central meteorological station: *"Estación Vallarta."*  

🔄 **Handling of Null Values:**  
- Replaced with 0, as a null value indicated the absence of measurement, not invalid data.  

📏 **Normalization:**  
- Ensured that data was within expected ranges to avoid errors in the analysis.  

Resulting in clean, structured data, ready for the model to work its magic. 🚀

## Data Modeling, Evaluation and Visualization
📊 **Chosen Model:** Polynomial regression to capture the trend of NOx emissions over the analyzed years.  

📈 **Why Polynomial?**  
- NOx emissions follow a parabolic pattern 📉📈 (approximately quadratic).  
- In winter, more pollutants remain suspended; in summer, rainfall washes them into the ground.  

🛠️ **Tool Used:** Scikit-Learn, the selected machine learning library for fitting the regression.  

The model’s accuracy was evaluated using the mean squared error.  

## Results
In the next visualizations we can observe:

📅 **Pollution Peaks (October-January):**  
- Increased emissions due to fireworks and bonfires during celebrations like Christmas and New Year. 🎆🔥  

🌧️ **Decrease in the Middle of the Year:**  
- Rainfall temporarily reduces pollutants in the air, as they combine with water vapor and form acid rain.  
- Festivities increase pollution, and rain redistributes it to the soil, but in both cases, it remains an environmental issue.

🦠 **2020 - An Unusual Year:**  

- Missing measurements in certain months, likely due to failures in the measuring devices or restrictions caused by the Coronavirus pandemic.   
- The pandemic and lockdowns may have affected both the operation of stations and the behavior of emissions.

<p align="center">
  <img src="https://github.com/user-attachments/assets/208e18e9-f51d-4f23-97cc-2717efef2b20" width="300" style="margin-right: 25px;" />
  <img src="https://github.com/user-attachments/assets/1611a564-ebff-43f9-8921-a20ab747af8d" width="300" style="margin-right: 25px;" />
  <img src="https://github.com/user-attachments/assets/0af41487-46c9-4428-ab8b-67f0a0f049c3" width="300" />
</p>

⚖️ **Average Pollution by Year:**  
- Highest pollution: 2000.  
- Lowest pollution: 2020.

<p align="center">
  <img src="https://github.com/user-attachments/assets/517dfaa6-0304-453e-b48c-d35691a4b191" width="500" />
</p>

📈 **Best Polynomial Fits by Year:**  

- 2000: 5th-degree polynomial.  
- 2010: 3rd-degree polynomial.  
- 2020: 2nd-degree polynomial.

🔮 **Can We Predict the Future?**  
- No, polynomials are not suitable for making direct future predictions.  
- However, with more complex machine learning models, patterns can be used to make predictions.  

🌱 **Future Applications:**  
This analysis could help control emissions and make decisions to reduce pollution and raise awareness about the environmental impact in the Guadalajara Metropolitan Area (AMG). 🌍💨  
