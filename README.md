# Pollutants-As-A-Polynomial

## About this project
🔍 **Project Objective:** Analyze how nitrogen oxides (NOx) emissions have changed in the Guadalajara Metropolitan Area (AMG) over the past 20 years and what insights an intelligent model can provide about their evolution. 🚀  

🤖 **Methodology:** A machine learning model will be used to process and understand the evolution of these pollutants.  

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
- In winter, more pollutants remain suspended; in summer, rainfall washes them into the ground. 🌧️💨  

🛠️ **Tool Used:** Scikit-Learn, the selected machine learning library for fitting the regression.  

⏳ **Next Step:** Evaluate the model’s accuracy using the mean squared error. 🔍  



