Ecoinformatics: methods in spatial and environmental biodiversity analysis
=====


##Course Description
___


Over the past few decades there has been an explosion of available data
for environmental and biodiversity research. This ‘big data’ now allows
us to address a number of old and new important questions with
unprecedented rigor and generality. Leveraging these new data streams
requires new tools and increasingly complex workflows.

The course will provide an overview of methods for addressing the
challenges of working in a Linux Environment, including command line and
scripting routines using open source software. Students will also learn
about multi-core computation on a local computer as well cluster
computation via remote servers. Scripting knowledge will be developed
step by step during the course, emphasising the concatenation process of
the different software. The course will have three sections: 1) Methods
and tools (Linux; command line scripting; GRASS; advanced R for
spatial/environmental data) 2) Example “big” datasets (environmental,
remote sensing, biodiversity) 3) Example questions, data integration and
modelling (data-model dichotomy, Bayesian approaches, addressing
uncertainty). At the end of the semester participants will have a basic
knowledge of the variety of open source tools that are available for
Geographic Information System (GIS), Remote Sensing (RS), and spatial
analysis and modelling. They will have worked through case studies from
forestry, species distribution modelling, biodiversity, conservation,
and remote sensing image processing.

Target audience of the course are students and postdocs with an interest
in advancing their data analysis and modelling skill-set and who have at
least basic understanding of statistics, remote sensing, and GIS (there
will be no emphasis on introductory concepts).

Course will be graded as pass/fail.

## History
This course was developed as Yale University (EEB 713) in the fall of 2013 as *Methods in spatial and environmental biodiversity analysis* by Adam M. Wilson, Walter Jetz, Giuseppe Amatulli & Petr Keil.  


##Tools
---

Linux shell-bash scripting, [GRASS](http://grass.osgeo.org/) and
[QGIS](http://www.qgis.org/) geographic information systems, [R
language](http://cran.us.r-project.org/) and
[JAGS](http://mcmc-jags.sourceforge.net/) and environment for
statistical computing and graphics, [GDAL/OGR](http://www.gdal.org/),
[Orfeo Toolbox](http://www.orfeo-toolbox.org/otb/),
[pktools](http://savannah.nongnu.org/projects/pktools), and [Open Foris
Geospatial Toolkit
(OFGT)](http://www.fao.org/forestry/fma/openforis/en/) for the
manipulation of (raster and vector) geospatial data. More information on
the tools and related exercises is stored at
[www.spatial-ecology.net](http://www.spatial-ecology.net) and on
[https://github.com/adammwilson/SpatialAnalysisTutorials](https://github.com/adammwilson/SpatialAnalysisTutorials).

##Computer requirements
---

The course will include class exercises on student laptops (under any
operating system).  We will provide a Linux Virtual Machine (LVM) with
GIS/RS open source software and all documents, exercises and data useful
for the course to be run on the participant's laptop using
[VirtualBox](https://www.virtualbox.org/).  Participants will be
encouraged to install the Virtual Machine on other computers to
facilitate continuation of their self-learning after the course. The LVM
can be installed as it is in any pc or can be used to create a USB
bootable version for a full installation.

##Data & Scripts
---

As discussed, we have consolidated the course material for easy download
and storage for future reference. The full material (the ost4sem folder
and Dropbox folder) can be download here
ftp://130.132.32.117/ost4sem.zip (1.5 GB). Please consider that in case
you want re-run the scripts it is necessary to set up the directory
where the data are stored.

We deleted some of the data that are also available online
 (e.g.[ ](http://www.worldclim.org/)[worldclim](http://www.worldclim.org/))
to reduce folder size. You can download them again using the wget
command.

For instructions on how to share a folder between your operating system
and the Linux Virtual Machine see here:  [Folder sharing option
VirtualBox](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:installvm)
____

#Schedule


The course content and schedule is designed to be flexible and
accommodate student preferences and abilities.

##Section 1: Methods and Tools

### Week 1

#### Introduction to the course

1.  Course Motivation & Objectives (see also ppt in ClassesV2)
1.  Era of big data in large scale spatial biodiversity analysis
2.  Existence of ‘big data’ requires specialized tools
3.  Toolbox of practical tools
4.  Workflow & repeatable research
2.  Overview of course components
3.  Student introductions

### Week 2

#### Linux OS

1.  [Introduction and installation of the Linux Virtual
    Machine](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:installvm)
2.  [Linux environment, why and what to
    use](http://www.spatial-ecology.net/ost4sem/lecture/hands_on_Linux_OS.pdf)
3.  [Why to use Unix/Linux and command line for solving complex research
    questions](http://www.spatial-ecology.net/ost4sem/lecture/hands_on_Linux_OS.pdf)
4.  The use of kate as an editor

#### [UNIX/LINUX Bash programming](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:bash)

1.  Command syntax and basic commands
2.  Redirection of the input/output
3.  [Read and explore a text
    file](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:basicbash)
4.  Concatenate process (pipe)
5.  The use of variable
6.  Iteration and conditional statements (for loop, if else)
7.  [AWK/GNUPLOT for text
    manipulation](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:awk) (if
    there is time/interest)
8.  [Exercise](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:advancebash)

### Week 3

#### Command-line tools for geospatial data

1.  [GDAL](http://www.gdal.org/)/[OGR](http://www.gdal.org/ogr_utilities.html) 

1.  Introduction to GDAL/OGR for raster and vector analysis
2.  Command syntax, raster/vector and data manipulation

2.  [pktools](http://savannah.nongnu.org/projects/pktools) and
    [oft-tools](http://km.fao.org/OFwiki/index.php/Open_Foris_Geospatial_Toolkit/Sandbox) for
    image processing
3.  [Exercise](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:gdalbasic)         

#### [GRASS](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:grass)
1.  [Introduction
    to](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:basicgrass2)[GRASS](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:basicgrass2)
2.  Data structure in GRASS
3.  Command syntax and general commands of data handling raster/vector.
4.  GRASS/Quantum GIS interface
5.  Scripting in GRASS: combine BASH with GRASS commands
6.  [Setting GRASS variables for GRASS bash
    job](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:grassvariables)
7.  [GRASS Create Location by bash
    script](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:grasscreatelocation) 
8.  QGIS
9.  Exercise

### Week 4

#### R programming for spatial analysis

1.  [Introduction to
    R](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:basicr)
2.  Raster library, performance and limitations
3.  Exercise

#### Introduction to pktools & oft-tools

1.  [Exercise](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:langintergartiongr) -
    Calculate mean and standard deviation  inside a polygon.
2.  [Exercise](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:openforis_burned) -
    Burned area classification 

### Week 5

#### [Language/software integration through scripting language](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:langintergartionptot)

1.  Combine multiple languages in a scripting-process (can use
    Bash/R/python/etc)
2.  Brief overview of wget as a tool to download MODIS data
3.  Import and export variables from different languages
4.  Integrate GRASS and R in a Bash script
5.  The use of EOF and the “Redirect         standard input”
6.  The use of arguments  in  bash R and  python
7.  Exercise


##Section 2: Example Datasets 
---------------------------

### Week 6

#### [Working with climate data](https://github.com/adammwilson/SpatialAnalysisTutorials/blob/master/climate/presentation/ClimateData.pdf)

1.  Climate Data

1.  Models, scenarios, etc.
2.  Historical vs. ‘Observed’
3.  Introduction to NetCDF/HDF (30 minutes)
4.  Earth System Grid data portal

#### Generating biologically relevant climate metrics (Adam, Walter)

1.  Climate Data Operators (CDO) / NetCDF Operators (NCO) / NCL
2.  Use daily data to generate metrics of interest using CDO

Exercise:  [Download, process, and visualize GCM and RCM data for New
England.](https://github.com/adammwilson/SpatialAnalysisTutorials/tree/master/climate/code)

### Week 7

#### Environmental and remote sensing data

        An overview of key environmental datasets with continental to
global extent

        An evaluation of their uses and limitations

#### Biodiversity data and informatics

        An overview of key biodiversity datasets with continental to
global extent

Models and Methods for integrating the dimensions of biodiversity


### Week 8 

In this class we will demonstrate important species occurrence data from
several sources, doing some data cleaning, and overlaying with
environmental data to ‘annotate’ the species observations with the
environmental data at that location.  We will then build a simple
species distribution model and predict the probability of occurrence
across the landscape.  [Data and code available
here.](https://github.com/adammwilson/SpatialAnalysisTutorials/tree/master/climate/code)

##Section 3: Statistical Models
=============================

All codes and data for this section are archived on GitHub at [https://github.com/adammwilson/SpatialAnalysisTutorials](https://github.com/adammwilson/SpatialAnalysisTutorials)
All teaching and exercises are done from within [R
studio](http://www.rstudio.com/), or from GitHub, using the
[Markdown](http://daringfireball.net/projects/markdown/)structuring of
the code; the codes are available in.rmd, .md and .html formats.

### Week 9 

#### [The duality of data and models; probability models for data](https://github.com/adammwilson/SpatialAnalysisTutorials/tree/master/statistics_intro)  (Petr) {.c5}

1.  Demonstration of several published cases (PowerPoint presentation)
2.  The deterministic and the stochastic parts of models
3.  Simple normally-, poisson- and binomially- distributed data in
    spatial context (on a raster grid). Normal, poisson and binomial
    regression as the baseline models
4.  Introducing the concept of Likelihood
5.  Spatial gradients and their influence on frequency distributions of
    data

### Week 10

#### [Statistical models in spatial context](https://github.com/adammwilson/SpatialAnalysisTutorials/tree/master/logistic_regression)

1.  Introduction to spatial autocorrelation
2.  Fitting logistic regression with and without a spatial component
    (GAM splines)
3.  Comparison of spatial and non-spatial models, and the inference on
    that
4.  Spatial autocorrelation in residuals; Moran’s correlograms

### Week 11

#### [Three ways of fitting models: glm(), maximum likelihood and MCMC](https://github.com/adammwilson/SpatialAnalysisTutorials/blob/master/poisson_regression/poisson_regression.md)

1.  The advantages of data centering and standardization
2.  The advantages of expressing statistical models by equations
3.  Introducing the Poisson log-linear model, exploring the role of its
    parameters
4.  Fitting the model using glm()
5.  Fitting the model by maximum likelihood; in-depth explanation of the
    concept of likelihood
6.  Fitting the model by MCMC in JAGS; brief intro to Bayesian inference

### Week 12
Yale last day of classes December 6

In this session we will perform a simple species distribution model
workflow for the Solitary Tinamou (Tinamus solitarius).   In this
session we will:

1.  Download and process some raster environmental data
2.  Process occurrence data from various sources
3.  Fit a Bayesian species distribution model using the observations and
    environmental data
4.  Predict across the landscape and write the results to disk as a
    geotif (for use in GIS, etc.)

[Exercise](https://rawgithub.com/adammwilson/SpatialAnalysisTutorials/master/workflow/Solitary_Tinamou/Tinamou.html)