# Proptech Application
## Housing Rental Analysis for San Francisco

Proptech is an innovative field that joins the real estate market and technology. This proptech application is an instant, one-click service for people looking to buy properties to rent. Our goal is to help these buyers find the best deals around San Francisco's neighborhoods. 

---

## Technologies

In order for this program to run, this application must be used in Jupyter Notebook, as it uses the Pandas/Python language. To run the program, it is essential to have JupyterLab installed. To ensure the code works, please open the file in a dev environment using python. It is also necessary to install Pandas in order to read/run the code.

The operating systems and program versions are mentioned below and are highly recommended when running the program.

**Systems**

[conda 4.10.3](https://docs.anaconda.com/anaconda/install/index.html) - Package manager, Environment Manager

python 3.7 - included in Anaconda

JupyterLab - included in Python 

Pandas - included in Python

**Other Installations**

[PyViz](https://pyviz.org/) - Tools for data visualizations


---

## Installation Guide

As mentioned above, to ensure that there are no errors when running this application, the user or programmer must use Jupyter Notebook to access the application file. 

Additional installs are needed before running the program. Please install in terminal, in a dev environment:

```JupyterLab
conda active dev
python -m ipykernel install --user --name dev
conda install -c conda-forge nodejs
conda deactivate

```
Once installed you should be able to open Jupyter Notebook by the following code:

```
conda activate dev
jupyter notebook
```

To exit out of Jupyter Notebook hit: Ctrl + C

It is important to also install Pandas as the majority of code used is using language from Pandas.

```Pandas
conda activate dev
conda install pandas -y
conda deactive
```

PyViz will help build interactive visual modules that will showcase our data.

```
conda install -c plotly plotly=4.13.
conda install -c pyviz hvplot
conda install -c conda-forge nodejs=12
```

The code below will install Jupyterlab dependencies.

```
conda install -c conda-forge jupyterlab=2
jupyter labextension install jupyterlab-plotly@4.13.0 --no-build
jupyter labextension install @jupyter-widgets/jupyterlab-manager plotlywidget@4.13.0 --no-build
jupyter labextension install @pyviz/jupyterlab_pyviz --no-build
jupyter lab build
```

As we are using Mapbox API to pull current data, you will need to use your MapBox API key to pull in the information. Be sure to have your *.env* file around to use this application.

```
!pip install python-dotenv
```



---

## Usage and Examples

To use the proptech application, the repository will need to be cloned from GitHub and into a local repository.

Please open the 'san_francisco_housing.ipynb' file. Enter into the dev environment by commanding: 

```
 conda activate dev
```
Next, use the code:

```
jupyter notebook
```
to run the file.

When using the file, each line of code must be individually ran to capture the data. This ensures any data that needs to be pulled gets included in future calculations as we start to build out formulas for analysis. It is important that we do not miss a line of code.

To quickly execute the code, use the keyboard shortcut: Shift + Enter.

The most important piece of code we need to run is the imports. Without these, information may not get pulled correctly.

In order to enable Mapbox API we need to use our Mapbox API key.

First we pull the information for San Francisco's gross rent, sales price per square foot, and housing units between 2010 and 2016.
We then evaluate the housing trends, looking to see how many units were sold in the year.

Next, we evaluate the trends for gross rent, sales price per square foot to see how the market functions. We analyze by time periods and by neighborhood.

Lastly, an interactive map that 




---

## Contributors

[Julia Guanzon](www.linkedin.com/in/julia-guanzon)

## License

GPL-3.0 License
