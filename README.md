Embedding Sensor information into Generative Adversarial Networks to determine COVID-19 infection risks in enclosed spaces
=======================

## Independent Research Project (ACSE-9) </br>
#### MSc in Applied Computational Science and Engineering 
#### Jamesson Ipock (Github: acse-jsi18)
</br>
This repository contains the report, code and documentation which demonstrates the development and implementation of spatio-temporal predictive PredGAN and DA-PredGAN models. 

------------------------

The project entails predictive modelling with use of a Generative Adversarial Network (GAN) in a novel approach of Enhanced Training; seeing the direct implementation of pre-defined sensor locations in making spatio-temporal predictions of viral laden air fluid flow. 
</br> 

**Isosurface contour gif** comparisons between the CFD Fluidity (Top) and the predictive models, DA-PredGAN (Center) and PredGAN (Bottom) with the Fluidity CFD shown below. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#"><img src="https://github.com/acse-2020/acse2020-acse9-finalreport-acse-jsi18/blob/master/animations/animation.gif" width="600"></a>&nbsp;&nbsp;&nbsp;

</br>
The system is written in the programming language, Python3, maximising the advantages of Machine Learning libraries, use of Google Colab's GPU's, and for graphical post-processing.
</br></br>

Repository structure
--------------------------
Within the repository there exists seven jupyter notebooks, with an animation folder containing the isosurface gif.
Notebooks:
* Load_data.ipynb
* POD_Compression.ipynb
* Extract_Sensors.ipynb
* Enhanced_Train_GAN.ipynb
* PredGAN_Enhanced.ipynb
* DA-PredGAN_Enhanced.ipynb

The predictive model notebooks exist as *PredGAN_Enhanced.ipynb* and *DA-PredGAN_Enhanced.ipynb*, however the other notebooks are vital for to produce the saved variables (e.g. .pkl file of POD coefficients etc.) necessary for the models to run.

Additionally, *Results.ipynb* notebook exists within the repository, highlighting some of the most important plots produced and those found within the report.

The repository further includes a *license.txt*, *requirements.txt*. 

### Getting started / Pre-requisites
----------------------------------
Installation
Clone or download the [Research Project Repository](https://github.com/acse-2020/acse2020-acse9-finalreport-acse-jsi18.git) to your local machine

Requires having *vtktools.py* and *tools_io.py* within the local repository, from the open-source [Fluidity](https://github.com/FluidityProject/fluidity) Computation Fluid Dynamics software package. 

To execute the .ipynb scripts:
Open the scripts in a jupyter notebook instance and click:
    
    Run or Run all
Command line:
     
     $jupyter nbconvert --to notebook --execute <notebookfilename>.ipynb

''' NEED BELOW??

Requirements/dependencies</br>
To install the packages/requirements:

     $ conda env create -f environment.yml 
     $ conda activate py3ml
     $ python -m ipykernel install --user --name=python3

