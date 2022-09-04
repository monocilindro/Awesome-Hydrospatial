

# **Awesome Hydrospatial**

An awesome and curated list of applications, tools, and documentation aimed to "map" the publicly available resources for the Ocean Mapping community.

Contributions are welcome. Add links through pull requests or create an issue to start a discussion.

<img src="./images/Hydrospatial.jpg" alt="Getting started" />



 
  - [**Free and Open Software for Ocean Mapping (FOSSOM)**](#free-and-open-software-for-ocean-mapping-fossom)
    - [Survey planning and preparations](#survey-planning-and-preparations)
    - [Data acquisition](#data-acquisition)
    - [Hydrographic data processing](#hydrographic-data-processing)
      - [**Specialized tools for multibeam backscatter processing**](#specialized-tools-for-multibeam-backscatter-processing)
    - [Quality Control / Quality Assurance](#quality-control--quality-assurance)
    - [Data management and visualization](#data-management-and-visualization)
    - [Tools for geospatial analysis and generation of derived products](#tools-for-geospatial-analysis-and-generation-of-derived-products)
    - [Python libraries, modules and other scripts](#python-libraries-modules-and-other-scripts)
  - [Python decoders](#python-decoders)
  - [Scripts](#scripts)
  - [Cartographic applications](#cartographic-applications)
  - [Other licenced but free tools](#other-licenced-but-free-tools)
  - [Visualization](#visualization)
  - [License and commercial hydrographic software](#license-and-commercial-hydrographic-software)
  - [Other interesting links](#other-interesting-links)
    - [Reference documentation](#reference-documentation)
    - [Conferences](#conferences)
    - [Hydrographic Offices / Mapping Agencies](#hydrographic-offices--mapping-agencies)
    - [Web sites](#web-sites)
    - [Youtube channels](#youtube-channels)
    - [Vimeo channels](#vimeo-channels)



## **Free and Open Software for Ocean Mapping (FOSSOM)** 
FOSSOM may be used to optimize survey design, troubleshoot and resolve multibeam system performance issues, derive products, and enhance data visualization and dissemination. 


### Survey planning and preparations
- [CruiseTools](https://github.com/simondreutter/cruisetools). A QGIS plugin aimed to simplify and automate common tasks in multibeam surveys

- [MBES Planning Tool](https://github.com/capt-clay10/MBES-Planning-Tool) is simplified GUI based tool to calculate line spacing, coverage and time taken.

- [BathyGlobe GapFiller](https://ccom.unh.edu/vislab/tools/gapfiller/) is a Windows tool designed to support planning for transit and area mapping, providing the latest versions of GEBCO bathymetry as context for planning. Gapfiller complements the online [Bathyglobe](https://bathyglobe.ccom.unh.edu/), an interactive globe to highlight the ocean mapping activities within the Seabed 2030 project.
- [AMUST](https://www.rijkswaterstaat.nl/formulieren/aanvraagformulier-software-hydrografische-normen), A-priori Multibeam Uncertainty Simulation Tool, is a Windows desktop software to compute the vertical and horizontal uncertainties in different operational circumstances. It is based on the error analysis of Hare et al (*Accuracy estimation of Canadian swath  and sweep sounding system, Canadian Hydrographic Service, 1995*)
- [SmartMap](https://www.hydroffice.org/smartmap/main), Sea Mapper's Acoustic Ray Tracing Monitor and Planning, is an online app within the [Hydroffice](https://www.hydroffice.org/) framework that provides tools to evaluate the impact of oceanographic temporal and spatial variability on hydrographic surveys.  
- [VDatum](https://vdatum.noaa.gov/) is a free Java tool designed to vertically transform geospatial data among a variety of tidal, orthometric and ellipsoidal vertical datums, allowing users to convert their data from different horizontal/vertical references into a common system and enabling the fusion of diverse geospatial data in desired reference levels. VDatum covers U.S. coastal areas out to 25 nautical miles from land.
### Data acquisition
- [Sound Speed Manager](https://www.hydroffice.org/soundspeed/) is a Python-based tool within the [Hydroffice](https://www.hydroffice.org/) framework that presents an intuitive, but feature-rich interface to guide the user through the processing steps required to deliver an enhanced sound speed profile to the acquisition system. 

### Hydrographic data processing

- [MB-system ](https://github.com/dwcaress/MB-System), is an open source software consisting of a set of programs to manipulate, process, list, or display bathymetry and backscatter imagery data derived from multibeam, interferometry, and sidescan sonars. MB-System is written in the C and C++ programming languages, and is delivered in packaged distributions for Linux and MacOS, as well as in the form of Docker containers. It can be run on Windows 10/11 machines by using the Windows Subsystem for Linux feature. 
- [NEANIAS Bathymetry Mapping from Acoustic Data service](https://www.neanias.eu/index.php/discover-the-neanias-services/underwater/26-services/493-u1-bat-service-2) (UW-BAT) is an online platform delivering an advanced user-friendly, cloud-based version of MB-System through Jupyter notebooks with additional functionalities.
- [GLOBE](https://www.seanoe.org/data/00592/70460/), GLobal Oceanographic Bathymetry Explorer,  is a Java application for processing and displaying raw multibeam and oceanographic data within a 3D environment represented as a globe. Kongsberg "all" and "kmall" formats as well as Teledyne "sk7" can be processed in GLOBE, along with IFREMER/SHOM raw multibeam format. Processed data come into [SONAR-netCDF4](https://github.com/ices-publications/SONAR-netCDF4) open format.   

- [OpenSideScan](https://opensidescan.cidco.ca/) is a Windows software to visualize and manipulate sidescan sonar imagery files, investigate seabed features, and create underwater inventories. OpenSideScan is free and open source, with community support on GitHub, but also is commercialized in custom versions with extra features and commercial support.

- [Kluster](https://github.com/noaa-ocs-hydrography/kluster) is a Python-based software that provides a fully open source hydrographic processing package to produce accessible bathymetry and backscatter products in support of ocean mapping. Kluster runs either on a GUI and through command line.
- [Sonar2MAT](https://cmst.curtin.edu.au/products/sonar2mat-software/) is a program that converts selected sonar files to MATLAB (.mat) data format to allow advanced data analysis and algorithm development. The convertor supports Reson (s7k), Kongsberg (.all, .wcd), Odom/Imagenex (.837, .83b and .83p), Generic Sensor Format (.gsf), Geoswath swamp and raw files (.swp, .rdf), MSTIFF (.mst) and eXtended Triton Format (.xtf).
- [CloudCompare](https://www.danielgm.net/cc/), is a 3D point cloud processing software. It can also handle triangular meshes and calibrated images. Although is commonly used in laser scanner and LIDAR data processing and photogrammetry, it is being utilized used for high definition 3D structure reconstruction from multibeam data.   


#### **Specialized tools for multibeam backscatter processing**
  - [SonarScope](https://www.seanoe.org/data/00766/87777/) is a Matlab-based software providing a high-performance environment for the analysis of multibeam echosounders and side scan sonars. In addition SonarScope is a reference tool for the treatment of bottom reflectivity by Ifremer and other marine resarch organizations.
  - [Stormix ](https://www.hydroffice.org/stormfix/) is a set of tools within [Hydroffice](https://www.hydroffice.org/) to reduce artifacts in acoustic backscatter data. It also allows displaying raw multibeam data. Currently Kongsberg "all" and "wcd" formats are supported.
  - [Iskaffe](https://github.com/alexschimel/Iskaffe) is an app to help assess the quality of the seafloor backscatter data acquired by multibeam echosounders. Iskaffe uses the CoFFee multibeam data processing toolbox. It is coded in MATLAB, but is also available as a standalone application that does not require a MATLAB licence. Currently Iskaffe support Kongsberg "all" and "kmall" formats.
  
  
### Quality Control / Quality Assurance

- [QC Tools](https://www.hydroffice.org/qctools/), found within  [Hydroffice](https://www.hydroffice.org/), assist in the review of various types of data occurring all throughout the ping-to-public process. Accepted data inputs are bathymetric grids, feature files, sounding selections, and directory structures. The output is GIS-layers that alert to the user various parts of their data that might require more attention. 
- [CA Tools](https://www.hydroffice.org/catools/main), another component of the [Hydroffice](https://www.hydroffice.org/) framework, assist in the assessment of the adequacy of nautical charts. Accepted data inputs are ENCs, bathymetric grids, and sounding selections. The output is GIS-layers that alert to the user various parts of their data that might require more attention
- [QAX](https://www.ausseabed.gov.au/QAX), coded in Python, facilitates quality assurance (QA) of multibeam echosounder data by standardising QA outputs and performing a robust QA. QAX integrates several tools, namely MATE, MBESGC and FinderGC. In a future release QAX will include QC tools [Hydroffice](https://www.hydroffice.org/)
- [Multibeam Advisory Committee Tools](https://github.com/MBAdv/multibeam_tools) are a set of Python tools for evaluating multibeam system installation and performance during Sea Acceptance Trials or Quality Assessment Testing.The tools are intended to simplify the multibeam evaluation process with a more user-friendly and flexible interface. The MAC tools are mostly intended for Kongsberg MBES.
- [CCOM MBES performance](https://vislab-ccom.unh.edu/~roland/acoustics/mbes_performance.html) is an online tool for assessing theorical the performance of an MBES from a set of given parameters.
- [Hydroffice](https://www.hydroffice.org/) is an open-source collaborative effort led by the Center for Coastal and Ocean Mapping to develop a research software environment with applications to facilitate all phases of the ping-to-chart process: facilitate data acquisition, automate and enhance data processing, and improve hydrographic products.
- [Pydro](https://svn.pydro.noaa.gov/Docs/html/Pydro/universe_overview.html) is a suite of software tools used to support hydrography and cartography. It is (almost exclusively) built from open source components as well as public domain custom developed software. Pydro is maintained by the Hydrographic Systems and Technology Branch (HSTB) to support NOAA operations (aiding our survey fleet) and is now made available for public use. Hydroffice tools are included within Pydro.

### Data management and visualization
- [CruisePack](https://www.ncei.noaa.gov/products/cruisepack)  is a data packaging and metadata gathering software tool to simplify submission of cruise-based data. CruisePack has a simple interface to control packager operation and metadata entry. Once the metadata entry is complete, data packaging is automatic. Although CruisePack is intended to comply with NCEI, it can be easily adapted for other organizations since it uses  a SQLite database under the hood.
- [OpenRVDAS](https://github.com/OceanDataTools/openrvdas),  Open Research Vessel Data Acquisition System, is a software framework used for building custom data acquisition systems. OpenRVDAS target audiences are oceanographic research vessel operators and operators of other science-related platforms that have the need to record streaming data. OpenRVDAS is capable of reading data records from serial ports and network-aware sensors, optionally modifying those data records and streaming either the result to one or more destinations, including logfiles, network ports, databases, etc.
  

### Tools for geospatial analysis and generation of derived products 
- [QGIS](https://www.qgis.org/) is a a reference cross-platform desktop geographic information system (GIS) application that supports viewing, editing, printing, and analysis of geospatial data. The numerous community of users support QGIS. Plugins are developed by independent organizations and developers, providing QGIS additional functionalities.
- [Raster Attribute Table QGIS Plugin](https://github.com/noaa-ocs-hydrography/qgis-raster-attribute-table-plugin) allows the user to display and edit Raster Attribute Tables (RATs) for discrete rasters using paletted/unique-values renderer. Useful for Geographic Object-Based Image Analysis (GEOBIA) in seafloor classication.

- [Whitebox Tools](https://www.whiteboxgeo.com/) (WBT) is a package for geospatial analysis that can be embedded into other software in order to facilitate building other types of applications.WBT contains over 500 geospatial analysis tools.
- [GRASS GIS](https://grass.osgeo.org/) is a multiplatform GIS software suite used for geospatial data management and analysis, image processing, producing graphics and maps, spatial and temporal modeling, and visualizing. It comes with a temporal framework for advanced time series processing and a Python API for rapid geospatial programming.
  
  ## Enhanced visualization
- The [CCOM Data Visualization and Interaction Tools](https://ccom.unh.edu/vislab/tools/), developed at the Visualization Laboratory, include VR Point Cloud Editor, Point Cloud Plugin for Unity, BAG Loader Unity Plugin, 3d Flight Unity Script and Coral Viz WebGl Viewer
 - [CesiumJS](https://cesium.com/)  is a JavaScript library for creating 3D globes and 2D maps in a web browser without any plugins. It uses WebGL for hardware-accelerated graphics, and is cross-platform, cross-browser, and tuned for time-dynamic data visualization. 
- [TerriaJS](https://terria.io/) is a library based on CesiumJS for building rich, web-based geospatial data explorers, used to drive  Digital Earth Australia Map and NSW Spatial Digital Twin , among many any others. It falls back to 2D with Leaflet on systems that can't run CesiumJS.

 - 
https://github.com/klakar/potree_deploy

### Python libraries, modules and other scripts
- [Bathycube](https://github.com/noaa-ocs-hydrography/bathycube) is a Python implementation of the CUBE module, Combined Uncertainty and Bathymetry Estimator. It only contains the cube grid/node objects, the original library included other data structures that were not translated here.
- 
https://github.com/GlacioHack/xdem



## Python decoders

https://github.com/CIDCO-dev/MBES-lib
https://github.com/UKHO/gsfpy
https://github.com/pktrigg/survey2ssdm
https://github.com/ices-publications/SONAR-netCDF4
https://github.com/wrenoud/hydrographic-libraries

## Scripts
https://github.com/monsterkittykitty/WaterColumnPlotter
https://github.com/ericrpatton/GRASS-GIS-and-Geomatics-Toolbox


## Cartographic applications
https://github.com/NoelDyer/Sounding-Selection

## Other licenced but free tools
[Ocean Tools: Marine Science](https://t.co/dMAZNAEK21) is an Android to develop useful tools for use in the planning and development of oceanographic surveys. It is not about providing tools that perform large calculations or processing, but rather Ocean Tools is focused on algorithms to perform small calculations on a day-to-day basis during the planning and execution of oceanographic campaigns.





## License and commercial hydrographic software
- QPS 
- EIVA Navisuite
- CARIS
- Beamworx
- Hypack
- SeaSFM
- [CMST-GA MB Process](https://cmst.curtin.edu.au/products/multibeam-software/)i s a proprietary backscatter data processing tool coded in Matlab and developed and used by Curtin University Centre for Marine Science and Technology (CMST) and Geoscience Australia (GA) researchers to process Kongsberg and Reson MBES data

## Other interesting links
https://github.com/javedali99/python-resources-for-earth-sciences
https://github.com/sacridini/Awesome-Geospatial
https://github.com/rvdata/NavManager
https://riverscapes.xyz/Tools/
https://github.com/Riverscapes/gcd/releases/tag/7.5.0
https://www.viametoolkit.org/
https://github.com/ignaciotb/SubmapsRegistration
https://github.com/SophieHCU/Interactive-MBES-processing
https://www.gpxsee.org/

### Reference documentation
- [The International Hydrographic Review](https://journals.lib.unb.ca/index.php/ihr/index) is an international journal by IHO publishing original works on all aspects of hydrography and associated subjects, ranging from the latest technical developments to history.

### Conferences

### Hydrographic Offices / Mapping Agencies




### Web sites 
https://geohab.org/

### Youtube channels


### Vimeo channels
