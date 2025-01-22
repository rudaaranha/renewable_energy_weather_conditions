# Rewable Energy and Weather Conditions
*Exploring the impact of climate on renewable energy generation.*

This dataset contains information about energy consumption and various climatic parameters such as solar radiation, temperature, pressure, humidity, wind speed, and precipitation. 
The "Energy delta[Wh]" column represents the change in energy consumption over a specific period, while the "GHI" measures Global Horizontal Irradiance, which is the amount of solar radiation received by a horizontal surface. 
The dataset also includes information about the presence of sunlight ("isSun"), the duration of daylight ("dayLength"), and the amount of time during which sunlight is available ("sunlightTime").
The "weather_type" column provides information about general weather conditions such as clear, cloudy, or rainy. The dataset is organized by hour and month, making it ideal for studying the relationship 
between renewable energy generation and climatic patterns over time.

| Column | Description |  
|----------|----------|  
| Time | The timestamp of the recorded data in the format YYYY-MM-DD HH:MM:SS |  
| Energy delta[Wh] | The difference in energy consumption in Watt-hours (Wh) from the previous timestamp to the current timestamp |  
| GHI | Global Horizontal Irradiance in watts per square meter (W/m²) measured by a pyranometer, which represents the amount of solar radiation received by a horizontal surface |  
| temp | Temperature in degrees Celsius (°C) measured at the same height as the pyranometer |  
| pressure | Atmospheric pressure in hectopascals (hPa) measured at the same height as the pyranometer |  
| humidity | Relative humidity in percentage (%) measured at the same height as the pyranometer |  
| wind_speed | Wind speed in meters per second (m/s) measured at the same height as the pyranometer |  
| rain_1h | Precipitation amount in millimeters (mm) measured in the last hour |  
| snow_1h | Snowfall amount in millimeters (mm) |  
| clouds_all | Cloud condition |  
| isSun | Whether there was sun during the day |  
| sunlightTime | Duration of sunlight |  
| dayLength | Number of hours of energy collection |  
| SunlightTime/daylength | Ratio of sunlight duration to energy collection hours during the day |  
| weather_type | Weather condition of the day |  
| hour | Hour of the day |  
| month | Month of the year |  

#### *Glossary*  

| Term | Meaning |  
|----------|----------|  
| Pyranometer | A pyranometer is an instrument used to measure solar irradiance, which is the amount of solar radiation received per unit area over a specific time period. This measurement is typically expressed in watts per square meter (W/m²). Pyranometers are essential in solar energy studies, meteorology, and climatology as they help quantify sunlight intensity under various conditions and locations. |  
| Watt-hour (Wh) | Watt-hour (Wh) is a unit of electrical energy measurement that quantifies the amount of energy consumed or generated over time. One watt-hour represents the energy equivalent of one watt of power used for one hour. **Calculation:** Energy (Wh) = Power (W) × Time (h) |  
| Irradiance | Irradiance is a measure of the power of solar radiation received per unit area at a specific moment. It is expressed in watts per square meter (W/m²) and represents the intensity of radiation incident on a surface. |  
| Celsius (°C) | Celsius (°C) is a widely used temperature measurement unit in many countries worldwide. It is part of the International System of Units (SI) and is based on two fixed reference points: **1. Freezing point of water:** 0 °C, the temperature at which water turns from liquid to solid (ice) under normal pressure. **2. Boiling point of water:** 100 °C, the temperature at which water turns from liquid to vapor also under normal pressure. |  
| Hectopascal (hPa) | Hectopascal (hPa) is a unit of pressure measurement commonly used in meteorology to express atmospheric pressure. One hectopascal equals 100 pascals (Pa), the International System of Units (SI) measurement for pressure. Atmospheric pressure is the force exerted by the air column above a specific point and is a critical parameter for understanding weather conditions. The conversion is as follows: 1 hPa = 100 Pa. |  
| Relative Humidity | Relative humidity is a measure expressing the amount of water vapor present in the air relative to the maximum amount the air can hold at a given temperature. It indicates the moisture level in the environment and is expressed as a percentage (%). Relative humidity (RH) is calculated using the formula: RH = (Current vapor pressure / Saturation vapor pressure) × 100. |  
| Precipitation | Precipitation is any form of water that falls from the atmosphere to the Earth's surface, including rain, snow, hail, and dew. It is a fundamental component of the water cycle and plays a critical role in ecosystems, agriculture, and water resource management. **Types of Precipitation:** Rain, snow, hail, and dew. | 


# Case

Amid the water crisis affecting countries like Brazil, governments face growing challenges in ensuring a reliable water supply to the population without overly depending on hydroelectric plants, whose production is directly linked to water availability. In search of sustainable alternatives, these companies have been investing in renewable energy sources, such as solar and wind energy, to diversify the energy matrix and reduce pressure on reservoirs. However, renewable energy production is highly influenced by climatic conditions, which vary daily and across seasons. These natural factors create the need for tools capable of predicting energy consumption variations based on climatic data.

This project aims to build a predictive model to help companies responsible for energy production and distribution anticipate the effects of climate changes on energy generation over time. To achieve this, we utilize a dataset containing detailed information on climatic variables such as solar irradiance (the amount of radiation reaching the surface), temperature, humidity, wind speed, and sunlight duration. The goal is to understand how these variables impact energy consumption and use this knowledge to forecast future consumption, represented by the variable "Energy delta[Wh]."

This predictive model will enable companies to adjust their operations and allocate energy resources more efficiently, maximizing the use of available renewable sources based on the climatic conditions of each day and season. For example, during periods of lower hydroelectric production, the company can optimize the distribution of renewable energy to reduce reliance on emergency sources, which are often more expensive and less sustainable. This approach not only reduces costs and increases efficiency but also contributes to the sustainability of the energy matrix, ensuring reliable and resilient energy supply even in times of water crisis.

This project offers an opportunity to apply data science to solve a real and urgent problem, helping the company address the challenges of an uncertain climate scenario and make smarter use of renewable energy sources.

Sources to understand the use of renewable energy and its environmental impact.
- https://www.sciencedirect.com/science/article/pii/S0360544221021757
- https://g1.globo.com/economia/noticia/2024/09/27/aneel-aciona-bandeira-tarifaria-vermelha-2-para-outubro-conta-de-luz-fica-mais-cara.ghtml
- https://aepet.org.br/artigo/impactos-socioambientais-no-maior-parque-solar-da-america-do-sul/
- https://www.uol.com.br/ecoa/ultimas-noticias/2024/07/18/impactos-parque-solar-piaui.html
- https://climainfo.org.br/2023/04/11/afetados-por-parques-eolicos-relatam-impactos-na-saude-e-no-meio-ambiente/
- https://brasil.mongabay.com/2023/10/comunidades-rurais-do-nordeste-enfrentam-desafios-causados-por-parques-eolicos/
