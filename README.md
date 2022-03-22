# DSNNowPlotting
    This tool is to plot DSN Now datasets in real time.
## Overview

    To plot various datapoints related to its mission that is accessed through the DSN API available here: 

        https://eyes.nasa.gov/dsn/data/dsn.xml

## Access
### Local Browser:
    Locate and open the "WebScrapeScript.html" file and open it within a browser. 
    This will start the javascript code to provide you a chart provided by the ApexCharts javascript library.

## Usage

### Page Header
**Refreshing data**: 
    Press the refresh button on the top left
**Add new chart**: 
    Press the "Add new chart" button to add a new chart to the page. By default 1 chart will be pre-loaded.
**Data Rate**: 
    The data rate by default is polling the site every 5 seconds. You can change the number in the number box which will reflect in the charts (in seconds). Minimum of 1 second.
### Chart View
**Add Item**: 
    Press the "Add Item" button in order to add a new value to be plotted to the graph. A dropdown menu by default is provided to add the first item. Additional items will populate with a "X" button to remove the item from the chart.
**Y Min/Y Max**:
    The Y min and Y max input field will auto populate with the tallest view possible that the data in the chart has. This is calculated with the min/max values. You can statically set each of these values by entering the number into the respective input. This will adjust the chart range automatically.
    You can "unset" these static values by clearing the field and the chart will go back into "auto" mode for that respective input. 

#### Dropdown Menus
**Signal Type**: 
    This is a unique list generated from each dish.

**Target name/Spacecraft**: 
    This is a unique list of name (if signal type is target) or SpaceCraft (if signal type is up/down signal) generated by each of the selected signal type data sets. 

**Mnemonic**: 
    This is a unique list of attribute values within the selected signal type data sets. 

#### Saving Data

    Pressing the "Download CSV" at the bottom right will loop through each item on each chart and create a CSV file with the data as an ISO string and mnemonic value listed in csv format.

    Note: The browser will likely prompt the user to approve "multiple file download" so you will have to "allow" that to happen if you want all the data. Otherwise, you will just download the first file.

#### Replotting the data

    To replot the data, it is recommended to save the CSV file after the realtime data needed has been plotted. In excel, you can select the data and "insert line graph" to view the plot again.

## On-going effort

### Separating by dish
    The data should be separated by dish
