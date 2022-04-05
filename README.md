# XFR-STIR
## Description
X-Ray Fluorescence Sample Topography Inverse Reconstruction (XRF-STIR), is a ray-tracing based application developed to recover a 3D sample together with its correct topographical landscape, from 2D XRF count rate maps acquired on multi-detection systems. A demo application can be found here, and upon clicking, can be accessed through the following credentials:
 * username: xrf
 * password: topography
 
 {LOGIN IMAGE}
 
After log-in it is possible to access a short usage manual in the "Appendix" section.
 
 {Appendix Image}
 
Secondly, the user can select an example dataset in the "Load Data" section, from three datasets that have been created artificially. Anyone of these datasets can be chosen and the respective experimental information will be loaded automatically in the following sections of the application. Further developments of the current application will allow users to load their own XRF datasets for analysis. For clarifications/information in this regard, please contact Matteo Ippoliti (matteo.ippoliti@elettra.eu).
 
 {LOAD DATA IMAGE}
 
Thirdly, the experimental information regarding the data acquisition needs to be input. As mentioned, this is automatically taken care of when loading any of the three example datasets, and parameters do not neet to be changed.

{Input Experimental Information IMAGE}

Inside the "Setup Geometry and XRF Lines" section one can setup all the experimental information relative to the acquisition geometry, i.e. how the multiple-detector system is arranged in space with respect to the sample being scanned. The current version of this application automatically loads the LEXRF acquisition setup present at the TwinMic beamline at Elettra Sinctrotrone, Trieste, when selecting one of the example datasets. As is, any setup recalling the basic geometry of LEXRF can be directly accessed in the application by simply changing the relative parameters (eg. detector's active area and distance to the sample). In the near future it will also be possible to test different acquisition geometries, by first contacting Matteo Ippoliti (matteo.ippoliti@elettra.eu) 
 

After having defined the acquisition geometry, the user needs to identify explicitly the XRF maps that have been provided at loadtime, by providing the element and fluorescence line for each found entry.

{select line image}

In the "Setup Inverse Reconstruction Parameters" section the user can change all the parameters linked to the reconstruction algorithm. For example it is possible to change the number of iteration required to extract thickness information from STXM data provided at loadtime, or change the XRF line to be used as a source for the inverse reconstruction.
