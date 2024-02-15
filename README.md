Directory contains Matlab code for generation of dielectric properties (dielectric permittivity and conductivity) 
for images from ISIC dataset.

The data for testing are copied from
https://challenge2020.isic-archive.com/

Download DICOM Corrected* (6.7GB)
10,982 DICOM images with embedded metadata.


Some of dicom-files (15 files) are  located  in  ISIC15dcm.zip, see their description below.

All files  named  ISIC*.dcm  can be can be analyzed in MATLAB, for example:


info = dicominfo('ISIC_0740997.dcm');

Y = dicomread(info);
figure

imshow(Y,[]);

We have analyzed following dicom files (all of them are in ISIC15dcm.zip):


ISIC_0171865.dcm 

ISIC_0585534.dcm 

ISIC_2406681.dcm  

ISIC_2479848.dcm

ISIC_0206261.dcm 

ISIC_0740997.dcm 

ISIC_2417982.dcm

ISIC_2493881.dcm

ISIC_0460023.dcm  

ISIC_2382043.dcm

ISIC_2423944.dcm 

ISIC_2518681.dcm

ISIC_0520611.dcm

ISIC_2401138.dcm

ISIC_2455226.dcm

Then these files were renamed   ( see archive ISIC15dcm.zip ) as 

ISIC1.m-ISIC15.m in the following order:

ISIC_0171865.dcm  --- ISIC1.dcm

ISIC_0206261.dcm  ... ISIC2.dcm

ISIC_0460023.dcm  

ISIC_0520611.dcm   .... ISIC4.dcm

ISIC_0585534.dcm

ISIC_0740997.dcm

ISIC_2382043.dcm

ISIC_2401138.dcm

ISIC_2406681.dcm

ISIC_2417982.dcm

ISIC_2423944.dcm

ISIC_2455226.dcm

ISIC_2479848.dcm

ISIC_2493881.dcm

ISIC_2518681.dcm  --- ISIC15.dcm

********************************************************************


Types of materials and values for epsilon and sigma are produced by matlab programs type_of_mat*.m


