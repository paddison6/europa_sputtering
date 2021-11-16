Compressed data files for manuscript by Addison et al., 2022.

Title: "Effect of the Magnetospheric Plasma Interaction and 
Solar Illumination on Ion Sputtering of Europa's Surface Ice"
Authors: Peter Addison*, Lucas Liuzzo, Sven Simon

*Corresponding author Peter Addison (paddison6@gatech.edu)

--------------------------------------------------------------
-------------------------- Description------------------------
--------------------------------------------------------------

There are two .zip files in this data archive. The first, 
"AIKEF.zip" contains the outptut of the AIKEF hybrid plasma 
simulation code for our publication, as described in section 
2.1 of the manuscript. The output is in the form of a binary 
.dat file, which can be converted into nine text files 
(denoting the three components of the magnetic field, 
electric field, and the grid locations). The conversion can 
be completed via use of the two .cpp filesprovided 
("readhybrid.cpp" and "main.cpp"). Specifying the path to the 
file in readhybrid.cpp, compiling the two scripts 
simultaneously, and running the subsequent executable will 
produce the nine .txt files. The second .zip file 
("GENTOo.zip") contains the results of the GENTOo GEN-2 particle 
tracing codefor fluxes and sputtering rates of H2O and O2 
from ion impacts.

--------------------------------------------------------------
------------------- Organization of these Files --------------
--------------------------------------------------------------

1. AIKEF.zip
   This directory contains a single .dat file, containing the 
   output of the AIKEF hybrid code for the configuration 
   described in section 2.1 of the manuscript. The two conversion
   files are also included. Data is in the EPhiO coordinate system 
   as described in the manuscript.
2. GENTOo.zip
   This directory is divided into H2O and O2 directories, 
   containing the relevant particle-tracing and sputtering
   quantities for each respective case and sputtered species. 
   The H2O directory contains subdirectories for the case of
   perturbed fields ("perturbed"), and for the case of 
   uniform fields ("uniform"). Each of these directories is
   in turn populated with subdirectories denoting ion species
   and energy. The O2 directory features an additional tier
   of subdirectories, denoting the different local times used
   to calculate the surface temperature profile, along with
   a directory for the diurnally-averaged case ("di_avg").
   Within each ion species directory is a number of energy
   directories, reflecting the ion energy (e.g., "10MeV").
   Within each of these directories is a "data" directory,
   which contains the respective data files. Ion fluxes 
   are contained in files named "cassidyflux.txt", 
   H2O sputtering rates are in files named
   "sputtering_yields.txt" (for modeled incidence angle)
   or "sputtering_yields_normal.txt" for constant, normal
   incidence angles. In addition, the O2 directories 
   contain data files denoted "o2_sputtering_rate.txt" and
   "o2_sputtering_rate_normal.txt", denoting the respective
   sputtering rates of O2, calculated with the model of 
   Teolis et al., (2017a), see text.
   All quantities are in units as defined in the 
   manuscript. Rows reflect a fixed latitude, while 
   columns reflect a fixed longitude.
   NOTE: The particle data is in the STANDARD POLAR 
   COORDINATE LONGITUDE SYSTEM, NOT THE WEST LONGITUDE 
   SYSTEM USED IN THE MANUSCRIPT. The first column, therefore,
   is at 0 degrees Polar, which corresponds to 90 degrees in 
   the West Longitude system. Longitude then increases 
   counterclockwise when viewed from above, i.e., towards
   90 degrees polar (0 degrees W), then 180 degrees polar 
   (270 W), then 270 polar (90 W), and finally back to 360
   Polar (90 W). The latitude step is 2 degrees, while the 
   longitude step is 4 degrees. The coordinate singularity at 
   Europa's poles is avoided.

For further information or with any inquiries about this data,
please contact the corresponding author. 
