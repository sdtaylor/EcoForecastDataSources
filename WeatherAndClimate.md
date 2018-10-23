# Weather and Climate Data

Weather and climate, in the form of temperature and precipitaiton, are key to any ecological system. The majority of ecological studies use the [WorldClim](http://www.worldclim.org/) for their long term forecasts, but there are many other data sources available. 

## Forecasts available from the USA National Oceanic and Atmospheric Administration (NOAA)

### Short Term Forecasts (1-21 days)

- [Global Ensemble Forecast Systems (GEFS)](https://www.ncdc.noaa.gov/data-access/model-data/model-datasets/global-ensemble-forecast-system-gefs)
Ensemble forecast of 21 different global models. Resolution of 1-2.5 deg. Released 4 times daily, each one making forecasts for 0-16 days ahead at 6 hour timesteps.

- [Global Forecast System (GFS)](https://www.ncdc.noaa.gov/data-access/model-data/model-datasets/global-forcast-system-gfs)
Single model global forecasts. 0.5 or 1 deg. released 4 times daily, making forecasts at 3 hour timesteps out to 10 days, and 12 timesteps 10-16 days.

- [NWS National Digital Forecast Database](http://www.nws.noaa.gov/ndfd/technical.htm)
This is *the* database for NWS forecasts for the next 14 days. *LOTS* of data here for all of the US and many different variables. Definitely the most confusing file structure ever. Seriously. Ever.

### Long term forecasts (2 weeks - 1 year)

- [CFSv2 Operational Forecasts](https://www.ncdc.noaa.gov/data-access/model-data/model-datasets/climate-forecast-system-version2-cfsv2)
0.5 deg global forecasts, released 4 times daily. Has an hourly timestep out 9 months. This is NOAA's state of the art system and is the source for things like hurricane forecasts, seasonal forecasts, and El Nino forecasts. 
NWS uses of the CFFv2 here

- [North American Multimodel Ensemble (NMME)](http://www.cpc.ncep.noaa.gov/products/NMME/)
An ensemble of 7-10 month forecasts from different US and Canadian groups.

- [Abatzogula Lab downscaled 7 month forecast](http://climate.northwestknowledge.net/RangelandForecast/download.php)
Uses the NMME project to create downscaled (4km) grid of the western us daily precip and temp forecasts up to 7 months out. Really nice visuals and website tools. Data is also available programatically via a THREDDS server. 

- [European Centre for Medium-Range Weather Forecasts](http://www.ecmwf.int/en/forecasts/datasets)
Hosts many different forecast datasets with global coverage from several days to 7 months out. Includes ensemble forecasts. Some data is free without a login, some available for research use only with a possible small fee. As a US Citizen I haven't been able to (or tried very hard) to access this data, but it may be available for European researchers. 

### Very long term forecasts (1-30 years)
- [CMIP5](https://esgf-node.llnl.gov/projects/esgf-llnl/) 
The [Coupled model intercomparison project](https://en.wikipedia.org/wiki/Coupled_model_intercomparison_project) is a suite of datasets derived from agencies all over the world. Simply put, they each run their respective climate models according to emission scenarios defined in IPCC reports. These are the input to the future conditions available in the WorldClim dataset.

- [Dowscaled CMIP](https://gdo-dcp.ucllnl.org/downscaled_cmip_projections/)
This group downscales CMIP projects to a spatial scale suitable for ecology, and a daily temporal scale. While the prediction for any given day will be wrong, being able to use daily data allows for more accurate forecasts (ie. see that one paper which stresses using daily temperature data instead of averages).

## Historic Data
### For USA / North America
- [PRISM](http://www.prism.oregonstate.edu/). Also see the [PRISM R Package](https://github.com/ropensci/prism)
- [DayMET](https://daymet.ornl.gov/).

### Europe
Unfortunately there is no easily available dataset such as PRISM or Daymet for Europe (that I know of). But see this StackExchange post which points to some [potential reanalysis data sources](https://gis.stackexchange.com/questions/82186/are-there-better-climate-data-than-worldclim-for-europe).
