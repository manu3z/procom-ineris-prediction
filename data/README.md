<br />
<div align="center">

  <h1 align="center">Prediction of air pollutant emissions based on learning methods</h1>

  <h2 align="center">
    Output files :
  </h2>
</div>

The following list state the 7 data files we need to run the algorithms:

```
EMISRefFRAProxyNO2.csv
FRA_CLC-2018_G.csv
FRA_OTM-FirstClass_G.csv
FRA_OTM-SecondClass_G.csv
FRA_OTM-MainRoad_G.csv
FRA_Population_G.csv
FRA_Proxy_G.csv
```

All of this data files are originally at high resolution but they all have columns to also match them at a lower resolution space (8km) for the prediction process. The most important of them all is the column: **```Id_G```**. This column was created by using the graphical interface from **qGIS** and is used to join all the data in one single dataframe for further exportation as '.csv'.

### ```EMISRefFRAProxyNO2.csv```
This are the emissions' data given by Ineris. They contain the data of the emissions of NO2:
* in Kg
* thoughout a given year
* for France
* at a resolution of 800m

### ```FRA_CLC-2018_G.csv```
This file contains the Corine Land Cover data for 2018 in France. This data is split in 3 classes of type of soil:
* Class 0: Artificial surfaces (Urban areas) 
* Class 1: Agricultural areas
* Class 2: Forest, Semi natural areas, Wetlands and Water bodies

### ```FRA_OTM-FirstClass_G.csv```
### ```FRA_OTM-SecondClass_G.csv```
### ```FRA_OTM-MainRoad_G.csv```

This 3 files correspond to the Open Transport Map data, separated in categories of roads: First Class roads, Second Class roads and Main Roads. The attribute that interests us the most is the traffic volume at each data point. 

### ```FRA_Population_G.csv```
This data file contains France's population given by Ineris.

### ```FRA_Proxy_G.csv```
This data file contains a grid of France at a high resolution, joined with a low resolution grid. This is used to predict all the values in France and to adapt every other data files to have both resolutions.
