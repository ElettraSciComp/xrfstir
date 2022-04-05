# XFR-STIR
![logo_image](https://github.com/ElettraSciComp/xrfstir/blob/main/images/logo_web_app.png)
X-Ray Fluorescence Sample Topography Inverse Reconstruction (XRF-STIR), is a novel [ray-tracing](https://en.wikipedia.org/wiki/Ray_tracing_(graphics)) based application developed in [Python](https://www.python.org/) and [Numba](https://numba.pydata.org/) for increased performance. The aim of the algorithm is to recover a 3D sample together with its correct topographical landscape, from 2D XRF count rate maps acquired on multi-detection systems of X-ray Fluorescence microscopy endstations. In particular, the presented demo application is designed on the LEXRF system present at the [TwinMic](https://www.elettra.trieste.it/elettra-beamlines/twinmic.html) beamline in Elettra Sincrotrone Trieste (Trieste, Italy). 
 
At present, the application is in its demonstration stage and only allows to load a predefined set of three datasets, allowing to edit all the parameters relevant for the acquisition setup geometry (i.e. the position of the detection system with respect to the examined sample) and the inverse reconstruction procedure. However, in the near future, it will be possible to upload the users' own datasets. Furthermore, upon contacting the authors (please address correspondence to: matteo.ippoliti@elettra.eu), it will also be possible to test different detection setups and geometries.
 
## Tutorial
Currently the demo application can be found [here](https://open-data.elettra.eu/scicomp/xrf-stir/) and can be accessed through the following credentials:
 * username: xrf
 * password: topography
 
![login_image](https://github.com/ElettraSciComp/xrfstir/blob/main/images/login.png)

After log-in it is possible to access a short usage manual in the "Appendix" section.
 
![appendix_image](https://github.com/ElettraSciComp/xrfstir/blob/main/images/appendix.png)

Secondly, the user can select an example dataset in the "Load Data" section, from three datasets that have been created artificially. Anyone of these datasets can be chosen and the respective experimental information will be loaded automatically in the following sections of the application. 

![load_data_image](https://github.com/ElettraSciComp/xrfstir/blob/main/images/load_data1.png)
 
Thirdly, the experimental information regarding the data acquisition needs to be input. As mentioned, this is automatically taken care of when loading any of the three example datasets, and parameters do not neet to be changed.

{Input Experimental Information IMAGE}

Inside the "Setup Geometry and XRF Lines" section one can setup all the experimental information relative to the acquisition geometry, i.e. how the multiple-detector system is arranged in space with respect to the sample being scanned. The current version of this application automatically loads the LEXRF acquisition setup present at the TwinMic beamline at Elettra Sinctrotrone, Trieste, when selecting one of the example datasets. As is, any setup recalling the basic geometry of LEXRF can be directly accessed in the application by simply changing the relative parameters (eg. detector's active area and distance to the sample). In the near future it will also be possible to test different acquisition geometries, by first contacting Matteo Ippoliti (matteo.ippoliti@elettra.eu) 
 

After having defined the acquisition geometry, the user needs to identify explicitly the XRF maps that have been provided at loadtime, by providing the element and fluorescence line for each found entry.

{select line image}

In the "Setup Inverse Reconstruction Parameters" section the user can change all the parameters linked to the reconstruction algorithm. For example it is possible to change the number of iteration required to extract thickness information from STXM data provided at loadtime, or change the XRF line to be used as a source for the inverse reconstruction.
