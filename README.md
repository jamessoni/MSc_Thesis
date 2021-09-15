## Embedding Sensor information into Generative Adversarial Networks to determine COVID-19 infection risks in enclosed spaces
---------------------------

#### Independent Research Project (ACSE-9) </br>
#### MSc in Applied Computational Science and Engineering 
#### Jamesson Ipock (Github: acse-jsi18)
</br>
This repository contains the report, code and documentation for the development of predictive models, PredGAN and DA-PredGAN, used to determine the spread of viral infection in enclosed spaces. 

------------------------

The project entails predictive modelling with use of a Generative Adversarial Network (GAN) in a novel approach of Enhanced Training; seeing the direct implementation of pre-defined sensor locations in making spatio-temporal predictions of viral laden air fluid flow. 
</br> 

**Isosurface contour gif** comparisons between the CFD Fluidity (Top) and the predictive models, DA-PredGAN (Center) and PredGAN (Bottom) with the Fluidity CFD shown below. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="#"><img src="https://github.com/jamessoni/MSc_Thesis/blob/master/animations/animation.gif" width="600"></a>&nbsp;&nbsp;&nbsp;

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

The predictive model notebooks exist as *PredGAN_Enhanced.ipynb* and *DA-PredGAN_Enhanced.ipynb*, however the other notebooks are vital to produce the saved variables (e.g. POD coefficients etc.) necessary.

Additionally, *Results.ipynb* notebook exists within the repository, highlighting some of the most important plots produced and those found within the report.

Functionality of the system requires calling functions from *vtktools.py* and *tools_io.py*, python scripts from the open-source [Fluidity](https://github.com/FluidityProject/fluidity) Computation Fluid Dynamics software package. This is therefore placed within the repository for ease of availability.

The repository further includes a *license.txt* and *requirements.txt* files. 

For further reading please refer to the [documentation](https://github.com/jamessoni/MSc_Thesis/blob/master/documentation.md).

### Getting started / Pre-requisites
----------------------------------
Although the notebooks can be run locally it is the recommendation to use the Google Colab platform, as use of the GPU's can significant reduce run time.

#### Installation
Clone or download the [Research Project Repository](https://github.com/jamessoni/MSc_Thesis.git) to your local machine


Change to the cloned directory.

    pip install -r requirements.txt

Ensure to *execute* the scripts in the order at which they are presented in the section above. This is due to dependency variables being defined and saved by each notebook.

To execute the .ipynb scripts:
Open the scripts in a jupyter notebook instance and click:
    
    Run / Run all

Note: The first two cells are commented and should remain as such unless using the Google Colab (recommended) platform.

License: GNU General Public License v3.0