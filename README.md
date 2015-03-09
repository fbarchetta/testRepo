dcs-template-insar-sentinel1
============================

Developer Cloud Sandbox template for InSAR with Sentinel-1 data


## Developer Cloud Sandbox template for InSAR with Sentinel-1 data 


## Quick link
 
* [Getting Started](#getting-started)
* [Installation](#installation)
* [Submitting the workflow](#submit)
* [Authors](#authors)
* [Questions, bugs, and suggestions](#questions)
* [License](#license)

### <a name="getting-started"></a>Getting Started 

To run this application you will need a Developer Cloud Sandbox, that can be either requested from:
* ESA [Geohazards Exploitation Platform](https://geohazards-tep.eo.esa.int) for GEP early adopters;
* ESA [Research & Service Support Portal](http://eogrid.esrin.esa.int/cloudtoolbox/) for ESA G-POD related projects and ESA registered user accounts
* From [Terradue's Portal](http://www.terradue.com/partners), provided user registration approval. 

A Developer Cloud Sandbox provides Earth Sciences data access services, and helper tools for a user to implement, test and validate a scalable data processing application. It offers a dedicated virtual machine and a Cloud Computing environment.
The virtual machine runs in two different lifecycle modes: Sandbox mode and Cluster mode. 
Used in Sandbox mode (single virtual machine), it supports cluster simulation and user assistance functions in building the distributed application.
Used in Cluster mode (a set of master and slave nodes), it supports the deployment and execution of the application with the power of distributed computing for data processing over large datasets (leveraging the Hadoop Streaming MapReduce technology). 
### <a name="installation"></a>Installation


##### Using the releases

Log on the developer cloud sandbox. Download the rpm package from https://github.com/Terradue/dcs-template-insar-sentinel1/releases. 
Install the dowanloaded package by running these commands in a shell:

```bash
sudo yum -y install dcs-template-insar-sentinel1-<version>-ciop.x86_64.rpm
```

#### Using the development version

Log on the developer sandbox and run these commands in a shell:

```bash
cd
git clone git@github.com:Terradue/dcs-template-insar-sentinel1.git
cd dcs-template-insar-sentinel1
mvn install
```

### <a name="submit"></a>Submitting the workflow

Run this command in a shell:

```bash
ciop-run
```
Or invoke the Web Processing Service via the Sandbox dashboard or the [Geohazards Thematic Exploitation platform](https://geohazards-tep.eo.esa.int) providing a master/slave product URL and optionally:

* A set of pairs (Master;Slave) comma separated of Sentinel 1 products e.g.:
```
https://data.terradue.com/gs/catalogue/tepqw/gtfeature/search?uid=S1A_IW_GRDH_1SDV_20150305T051939_20150305T052004_004892_006196_B6ED;https://data.terradue.com/gs/catalogue/tepqw/gtfeature/search?uid=S1A_IW_RAW__0SDV_20150303T053527_20150303T053559_004863_0060F7_124C
```


### <a name="authors"></a>Authors (alphabetically)

* Barchetta Francesco
* Brito Fabrice

### <a name="questions"></a>Questions, bugs, and suggestions

Please file any bugs or questions as [issues](https://github.com/geohazards-tep/dcs-template-insar-sentinel1/issues/new) or send in a pull request.

### <a name="license"></a>License

Copyright 2015 Terradue Srl

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0

> This work has been co-funded by the EC FP7 project MED-SUV Grant agreement 308665 
