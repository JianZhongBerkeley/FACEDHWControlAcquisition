# FACEDHWControlAcquisition
Scan control and data acquisition software for FACED 2PFM

![Software Demo](./Assets/SoftwareDemo.gif)


## Citation
Please cite the *FACED 2.0 enables large-scale voltage and calcium imaging in vivo* paper if you use the software in this repository.  


## Dependency
- National Instrument LabVIEW 
- Microsoft Visual Studio Community
- OpenGL


## System requirements 
Te run the software, we recommend to set up workstation with the following computation resources:
- CPUs: Intel® Xeon® Gold 6354 x 2
- RAM: 64GB DDR4 x 4
- GPU: PNY Technologies RTX A4000
- M.2 NVMe SSD: 1.9TB M.2 PM9A3 NVMe Solid State Drive (Gen 4)
- SATA SSD: 960GB 2.5" D3-S4610 SATA 6Gb/s Solid State Drive
(3 x DWPD)
- HDD: 16TB 3.5" Exos X16 7200 RPM SATA3 6Gb/s 256MB
Cache 512E/4Kn Hard Drive


## Descriptions 
- [LabVIEW Scan Control Software](./FACED_DataAcquisition/): miscroscope scanning hardware control program
- [Data Acquistion Software](./FACED_ScanControl/): high-speed data acquistion program


## Installation guide for LabVIEW scan control software
- Connect NI DAQ devices to the host computer
- Follow the [instructions](https://www.youtube.com/watch?v=4x_EH53hb2I) to install NI-DAQmx
- Install SmarAct mcs2 control driver
- Unzip and run the software installer in the [repository directory](./FACED_ScanControl/) to install the LabVIEW software


## Installation guide for data acquisition software
- Connect Teledyne data acquisition device to the host computer
- Follow instructions and install [Visual Studio](https://visualstudio.microsoft.com/)
- Install Teledyne hardware driver and C/C++ API support
- Follow instructions in the Teledyne ADQUpdater User Guide to update PFGA firmware
- Follow instructions and install [freeGLUT](https://freeglut.sourceforge.net/) for OpenGL support (this step can be skiped for installation using the packages saved in JiLab drive)


## License
[GLP-3.0 license](./LICENSE)