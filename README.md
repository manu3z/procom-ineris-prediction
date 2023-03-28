<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/manu3z/procom-ineris-prediction">
    <img src="images/logo.png" alt="Logo" width="100" height="100">
  </a>

  <h1 align="center">Prediction of air pollutant emissions based on learning methods</h1>

  <h3 align="center">
    Collaboration between IMT Atlantique students and INERIS
    <br />
    <a href="https://www.imt-atlantique.fr/en">
    <img src="images/imta.jpg" alt="Logo IMTA" width="80" height="60">
    </a>
    <a href="https://www.ineris.fr/en">
    <img src="images/ineris.png" alt="Logo INERIS" width="80" height="80">
    </a>
  </h3>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a>
    <li>
      <a href="#usage">Usage</a></li>
      <ul>
        <li><a href="#prerequisites">load_data</a></li>
        <li><a href="#installation">models</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Proportion Original][proportion-original]] [![Proportion Original][proportion-predicted]]

This project has the objective to train a machine learning algorithm with high resolution data from France, in order to be able to use this model as a super-resolution prediction tool applied in other countries with lower resolution data.

Our method consisted in taking the high resolution data: a grid of data points every 800m, and summing the values in a bigger grid of 100 values: a grid of points every 8km. Then, we trained the algorithms to have an input of values every 8km and as output, values every 800m.

The data used to train the model was used for:
* State monitoring of ambient air quality in France
* Modelling of pollutant concentrations via chemistry-transport models.

More information on the data:
* Using spatial data, quantity of pollutants emitted, meteorological data.
* Preliminary work conducted by INERIS using a multilinear regression model

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Built With

To build this project we used the following languages, libraries and programs:

* [![Python][Python.org]][Python-url]
* [![Jupyter][Jupyter.org]][Jupyter-url]
* [![qGIS][qGIS.org]][qGIS-url]
* [![scikit-learn][scikit-learn.org]][scikit-learn-url]
* [![PyTorch][PyTorch.org]][PyTorch-url]

We used Jupyter Notebooks to run all our codes and be able to extract outputs as the code was running.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To begin with, we need to download the data shared by Ineris. The downlaoded files should be put in the ```/data``` folder, as specified in the README file inside said folder.

If the user wants to use directly the prediction algorithms, they can also downlaod the output files and put them in the ```/output``` folder, as specified in the README file inside said folder.

<!-- USAGE EXAMPLES -->
## Usage

In order to use our codes, we have created two Jupyter notebooks to separate the two main functionalities we worked on: data treatment and machine learning prediction. Each of those notebooks are specified below.

### ```load_data```

This Jupyter notebook has all the steps that necessary to load, in one single ".csv" file, all the data that will be used to train the ```models``` later.

We used the Pandas and Numpy libraries to do this.

### ```models```

This Jupyter notebook uses the output of ```load_data``` and performs the training, testing and validation of different machine learning regression algorithms, such as: Linear Regression, Random Forest, Gradient Boosting and MLP.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Manuel SANCHEZ-LAGUARDIA : [Mail](mailto:manuel.sanchez-laguardia@imt-atlantique.net) - [LinkedIn](https://www.linkedin.com/in/manuel-sanchez-laguardia/)

Jonny Alexander TORRES ROBLES : [Mail](mailto:jonnyy-alexander.torres-robles@imt-atlantique.net) - [LinkedIn](https://www.linkedin.com/in/jonnyytorres/)

Marianne BELLERY : [Mail](mailto:marianne.bellery@imt-atlantique.net@imt-atlantique.net)

Joel IRIE : [Mail](mailto:bi-doubi-armel-joel.irie@imt-atlantique.net)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- IMAGES and LINKS-->
[proportion-original]: images/70203_ORIG.png
[proportion-predicted]: images/70203_RF_Final.png

[Python.org]: https://img.shields.io/badge/-Python-yellow?logo=python&style=flat&logoWidth=30
[Python-url]: https://www.python.org/
[Jupyter.org]: https://img.shields.io/badge/-Jupyter-orange?logo=jupyter&logoColor=white&style=flat&logoWidth=30
[Jupyter-url]: https://jupyter.org/
[qGIS.org]: https://img.shields.io/badge/-qGIS-green?logo=qgis&logoColor=white&style=flat&logoWidth=30
[qGIS-url]: https://www.qgis.org/en/site/
[scikit-learn.org]: https://img.shields.io/badge/-scikit_learn-blue?logo=scikit-learn&logoColor=white&style=flat&logoWidth=30
[scikit-learn-url]: https://scikit-learn.org/stable/index.html
[PyTorch.org]: https://img.shields.io/badge/-PyTorch-orange?logo=pytorch&logoColor=white&style=flat&logoWidth=30
[PyTorch-url]: https://pytorch.org/
