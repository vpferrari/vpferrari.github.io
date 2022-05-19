## step 1: install gdal

A simple apt-get would do:

    sudo apt-get install libgdal-dev

## step 2: setup your venv

On a project directory:

    python3 -m venv venv

In order to activate it:

    source venv/bin/activate

You may want to upgrade pip:

    pip install pip --upgrade

## step 3: install python binding for gdal

First you need to get the GDAL version:

    gdal-config --version

This shall give you a version number (e.g.: 2.4.0). So you may proceed and install the right version of pygdal:

    pip install GDAL==<your-gdal-version>

So, for our example:

    pip install GDAL==2.4.0

## step 4: install geopandas

As a test you may install geopandas, that heavily depends on gdal:

    pip install geopandas

pip will just get the proper geopandas version based on your GDAL library installed. 
