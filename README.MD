# PV Systems Diffusion Forecasting
## _Dataset and ML Algorithms Benchmark_
[![DOI](https://zenodo.org/badge/677429901.svg)](https://zenodo.org/doi/10.5281/zenodo.10415226)
<a target="_blank" href="https://colab.research.google.com/github/gmlunardi/on-grid-pv-systems-difusion-forecasting/blob/main/Analysis_per_Quarter.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>


This repository contains a Python code file written in a Jupyter notebook. It includes all the experiments conducted with the support of the PyCaret 3.0.4 library in a temporal regression task to predict the diffusion of photovoltaic energy systems in Brazil.

## Dataset

We developed the dataset `dataset_temporalQUARTER.csv` with a set of predictors from different datasources. Then, we used it to train the algorithms we used in the experiments. Therefore, you will need the following predictors to forecast `Installed Power`, our target attribute for estimating diffusion, for a new quarter:

| Predictor | Unit |
| ------ | ------ |
Installed Power	| kW
Quarter	        | Date
Electricity Tariff	Currency | (R$) 
Irradiance	| Wh/m²
Fleet	| N/A
Education HDI	| %
Longevity HDI	| %
Income HDI	| %
Population	| N/A
Territorial area |	Km²
Population density	| People/area
College education	| %
Number of households	| N/A
Cities verticalization	| %
Households in rural area	| %
Number of own households	| N/A
Number of rented households	| N/A
Residents per household	| People/house
Households with three or more residents |	N/A
Gross Domestic Product (GDP) per capita	Currency | (R$)/people
Average minimum wage in the city	| Currency (R$)
Number of companies in the city | 	N/A
Number of employees in the city	| N/A


## How to Load Trained Models
If you only wish to make predictions, download the `lightgbm` and `randomForest` models and load them into a blank Jupyter notebook using the following command:

```python
load_model()
```

This way, you won't need to train the algorithms again. For more details, you can find them at this link: https://pycaret.gitbook.io/docs/get-started/tutorials

## How to cite this repo and data
Cite the paper as following LaTeX bib:

```latex
@misc{tobedefined,
      title={How explain on-grid PV systems diffusion? Review and Application in Brazil}, 
      author={authors},
      year={tobepublished},
}
```

Please, cite the following too:
[![DOI](https://zenodo.org/badge/677429901.svg)](https://zenodo.org/doi/10.5281/zenodo.10415226)

