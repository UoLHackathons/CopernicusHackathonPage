# Welcome to the training page of the Copernicus Hackathon at Univeristy of Leicester
University of Leicester in collaborations with Uni-Soft Systems are holding the first Copernicus Hackathon in UK with a focus on using satellite data for food security on 19-20 Sep. 2019. The training day for all participants will be held on 12th Sep. This page is designed to help the participants to get familiar with the data and the tools for the hackathon.

## General Information
[Copernicus Project Overview](https://www.copernicus.eu/en/about-copernicus/copernicus-brief) provides a brief overview to the Copernicus services and objectives. Copernicus project is served by a set of dedicated satellites: the Sentinel family. For this Hackathon, we are interested in using Sentinel-1 (radar imaging for land and ocean monitoring) and Sentinel-2 (land monitoring of vegetation, soil and coastal areas) data. 

The user guide below gives a top-down overview of the Satellite, the instruments it has onboard, the data it produces and its applications.

- [Sentinel-2 User Guide](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi)

## Training Material
Below is a list of general information and resources about the Copernicus project, specifically the Sentinel-2 satelite mission and the data products it produces.

##Copernicus Climate Data Store (CDS)## site (https://cds.climate.copernicus.eu/#!/home) is a really useful training tool. You will need to create a free account in order to access the data, api and the toolbox. The site also includes the full catalogue of data available which include dataset descriptions.

## Useful links for Understanding the Data: 

https://www.nrcan.gc.ca/maps-tools-publications/satellite-imagery-air-photos/tutorial-fundamentals-remote-sensing/9309  

**Remote Sensing Tutorials by Canada Centre for Mapping and Earth Observation:** a good introduction to the multiple purposes and applications of Remote Sensing. Useful for novices in satellite data.  

https://gdal.org/drivers/raster/sentinel2.html 

**Sentinel-2 Products:** A useful link on the Sentinel-2 products, the bands and the classifications. In addition, it shows the main meta data files for Sentinel-2 downloads and explains some performance issues.  
 
 
## Useful tutorials on data use and algorithms:  

https://www.hatarilabs.com/ih-en/sentinel2-images-explotarion-and-processing-with-python-and-rasterio 

**Sentinel-2 Images Exploration & Processing with Python & Rasterio:** This is a tutorial on how to use Rasterio to get various image bands from the data.  

https://github.com/mapbox/rasterio 

**Rasterio:** A useful GitHub page detailing the purpose of Rasterio and examples of the code and outputs.  

https://towardsdatascience.com/satellite-imagery-access-and-analysis-in-python-jupyter-notebooks-387971ece84b 

**Manipulating satellite imagery using Python in Jupyter:** This is a tutorial on how to access and retrieve data directly in the Python code. It also explores how to create RGB and NDVI (Normalized Difference Vegetation Index) images from the Sentinel-2 bands; useful if you’re working on a project involving optimal crop timing.  

https://step.esa.int/main/doc/tutorials/snap-tutorials/ 

**SNAP Tutorial:** A webpage containing all video tutorials for SNAP processes, tools and calculations.  

## Accessing the data: 

During the Hackathon, the data will be accessed through a S3 bucket provided on the day. However to access the Sentinel data outside of the Hackathon, you need to download the zip file from [Copernicus Open Access Hub](https://scihub.copernicus.eu/dhus/#/home). 

**Step 1:** Register as a user on Scihub to be able to download the data. 

**Step 2:** Once you’ve registered, switch from the area map view over to the navigator tool. From there, select an area on the map that you’re interested in analysing and click search. 

**Step 3:** A list of available data will appear on the left hand side of the site. From there, you can choose the most applicable data and download the zip file to use with whichever programme you're running the data on. 

## Accessing the VM via Sobloo desktop: 

**Step 1:** Enter the IP address of the virtual machine using your browser and https into the address bar.

**Step 2:** You will be directed towards a login page, the credentials are as follows:

** IP address of the VM and credentials will be provided during the hackathon.
   
## Accessing the VM using SSH: 

**Step 1:** Within the Hackathon directory on Sharepoint, download the private key file for your machine. You will be told which key this is on the day of the Hackathon. In this example, we will use the id_rsa_vms-uol-1.txt private key file.

**Step 2:** Download [PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

**Step 3:** Once downloaded, open PuTTYgen (a key generator application downloaded alongside PuTTY) from the start menu.

**Step 4:** Click *Load an Existing private key file*. 

**Step 5:** Make sure *All Files* is selected in the dropdown at the bottom left and find your private key’s .txt file. 

**Step 6:** After clicking open, you will receive a dialogue like the one below notifying you that you need to save the private key in PuTTY’s own format. Click *ok*. 

**Step 7:** If you wish to add a passphrase to protect your key add one in the *Key Passphrase* field and confirm it in the field below, otherwise leave both fields blank and when prompted, click *Yes* on saving your key without a passphrase. 

**Step 8:** Now save the private key in the save dialogue, in this example we named it mykey.ppk 

**Step 9:** Next, open PuTTY and enter the IP of your machine in the *Host Name field*.

**Step 10:** Now, in the category tree in the left handside bar select: Connection >  SSH > Auth 

**Step 11:** In the ‘private key file for authentication’ field, upload the PuTTY key you saved earlier (mykey.ppk). Then click *Open*. 

**Step 12:** When prompted, accept the server’s host key to your cache by clicking *Yes*. 

**Step 13:** Now in the terminal, enter the Username for your machine and if you created a passphrase for your PuTTY key enter that as well. You are now authenticated over SSH and can interact with the VM over the terminal. 

## Tools and IDEs: 
* Pycharm [Download Here](https://www.jetbrains.com/pycharm/download/#section=windows)
* Jupyter [Download Here](https://jupyter.org/install)
* Conda (Anaconda/MiniConda) [Download Here](https://www.anaconda.com/distribution/)
* PuTTY [Download Here](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
* BitVise Tunnellier [Download Here](https://www.bitvise.com/ssh-client-download)

**Useful Libraries and Dependencies:**

Core: Numpy, Gdal, Scikit-learn, hdf-4, hdf-5

Ancilliary: Pandas, Geopandas, Matplotlib, Scikit-image

**Useful Sites & Information:**

John Robert's full environment file is at 

https://github.com/clcr/pyeo/blob/master/environment.yml

You can create it using Conda with the following command:
conda env create --file environment.yml --name pyeo_env

## Presentations from the Training Day (12/9/2019)
Here are all the [presentations](https://github.com/UoLHackathons/CopernicusHackathonPage/tree/master/Training%20day%20presentations) from the training day on 12/9/2019 at Leicester University's Innovation Hub. 

