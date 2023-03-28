<br />
<div align="center">

  <h1 align="center">Prediction of air pollutant emissions based on learning methods</h1>

  <h2 align="center">
    Output files :
  </h2>
</div>

The following list state the 3 output files we worked on:

```
france_NO2_all.csv
predictions_70203.csv
predictions_all.csv
```

### ```france_NO2_{}.csv```
The first of them all, is the output of the ```load_data``` notebook. This corresponds to the data from:
* Emissions (from Ineris)
* Traffic Volume (from Open Transport Map)
* Population (also from Ineris)
* Soil Type (from Corine Land Cover)

### ```predicions_{}.csv```
This files contain the outputs from the ```models``` notebooks. They are ready to use, compare, and create visualizations.