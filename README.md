# **SAIVT Soft Biometric Database**

## **Overview**
The SAIVT-SoftBio database contains a collection of multi-camera sequences of 152 pedestrians captured from a set of 8 surveillance cameras. This database provides a challenging and realistic test-bed for person redetection tasks, and is freely available for download. Contact Dr Simon Denman (s dot denman at qut dot edu dot au) for more information.

## **Licensing**
The SAIVT-SOFTBIO database is © 2012 QUT and is licensed under the [Creative Commons Attribution-ShareAlike 3.0 Australia License] (http://creativecommons.org/licenses/by-sa/3.0/).

## **Attribution**
To attribute this database, use the citation provided on our publication at [eprints] (http://eprints.qut.edu.au/53437/).

## **Acknowledgement in publications**
In addition to citing our paper, we request the following text be included in your publications:
'We would like to thank the SAIVT Research Labs at Queensland University of Technology (QUT) for freely supplying us with the SAIVT-SoftBio database for our research'.

## **Installing the SAIVT-SoftBio Database**
[Download and unzip this archive] (https://Q0102-RO:Vieyae3G@q0102-webdav.qcloud.qcif.edu.au/SAIVT-SoftBio.tar.gz)

At this point, you should have the following data structure and the SAIVT-SoftBio database is installed:
```
SAIVT-SoftBio 
 +-- Calibration 
   +-- C1--U1-17 
   +-- C2--U18-48 
   ... 
   +-- C10--U140-152 
 +-- Uncontrolled 
   +-- Subject001 
   +-- Subject002 
   +-- Subject003 
   ... 
   +-- Subject152 
 +-- Bialkowski2012 - A database for person re-identification in multi-camera surveillance networks.pdf 
 +-- LICENSE.txt 
 +-- README.txt 
 +-- SAIVTSoftBioDatabase.xml
```
The 'Calibration' directory contains a camera calibration and background images (one image per camera) for the dataset. It is arranged into groups of subjects (i.e. C1--U1-17 contains camera calibration and background images valid for subjects 1 to 17). All camera calibration has been calculated using Tsai's method.
The 'Uncontrolled' directory contains the image sequences for each subject, arranged by camera view.

The 'SAIVTSoftBioDatabase.xml' file defines the database. This file specifies the number of cameras used and number of calibrations present, the regions of interest for each camera (<camera> tags), the location of the calibration information (<calibration> tags), and the subjects themselves (<uncontrolledsubject> tags). Note that for each subject, a camera calibration is specified.

[Motion segmentation masks for the entire database] (https://Q0102-RO:Vieyae3G@q0102-webdav.qcloud.qcif.edu.au/SAIVT-SoftBio-Segmentation.tar.gz)

More information on the SAIVT-SOFTBIO database in our paper at [QUT eprints] (http://eprints.qut.edu.au/53437/)