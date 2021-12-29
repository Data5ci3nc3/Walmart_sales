## Walmart sales project
Build a machine learning model able to predict the weekly sales in Walmart stores with the best possible precision.

## Goal to be achieved
Create an application that will recommend where people should plan their next holidays. The application should be based on real data about weather and hotels in the area.
Furthermore, the application should be able to recommend the best destinations and hotels based on the above variables at any given time.

## Methodology applied to reach the goal
- Scrape data from destinations
- Get weather data from each destination
- Get hotels' info about each destination
- Store all the information above in a data lake
- Extract, transform and load cleaned data from your datalake to a data warehouse

## Scope of the project
Focus on the Top 35 cities/destinations to visit in France:
Mont-Saint-Michel, Saint-Malo, Bayeux, Le Havre, Rouen, Paris, Amiens, Lille, Strasbourg, Chateau du Haut-Koenigsbourg, Colmar, Eguisheim, Besançon, Dijon, Annecy, Grenoble, Lyon, Gorges du Verdon, Bormes-les-Mimosas, Cassis, #Marseille, Aix-en-Provence, Avignon, Uzès, Nîmes, Aigues-Mortes, Saintes-Maries-de-la-Mer, Collioure, Carcassonne, Ariège, Toulouse, Montauban, Biarritz, Bayonne and La Rochelle.

## Data collection (extraction#)
cleaning, data - and data U minatim. e https:org/ to get the gps coordinates of all the cities/destinations
- Use https://openweathermap.org/appid to collect information about the weather for the 35 cities/destinations

## For this project, average temperature determines nice weather
The average temperature collected for the coming week has been calculated to determine the list of cities where the weather will be the nicest.

## Data cleaning, data manipulation and data storage (transform and load)
- All results were saved in the kayak.csv file and uploaded programatically on an Amazon Simple Storage Service bucket.
- A (extraction) postgresql database instance was created on AWS Relational Database Service (RDS) using PG Admin. The data sent to the S3 datalake was also uploaded to the RDS through the SQL language. Thereby, the data analysis team can extract cleaned data from the data warehouse.
- Tests have been conducted on the Jupyter notebook to verify that the data has been corretly uploaded to the database instance on Amazon RDS.

## Data visualization
- After determining t#he Top 5 cities, the Top 5 French cities with the highest average temperatures for the next 7 days have been plotted on a map.
- Top hotels in the Top 5 cities have been plotted on a map so that the customers can have information aggregated by Kayak rather than having to find it elsewhere on the Web.age (transform and load)
