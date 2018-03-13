This scraper collects the information about the air quality around the
WestConnex M4 East project in Sydney, Australia.

The information is collected by a contractor for WestConnex and is published at [http://airodis.ecotech.com.au/westconnex/](http://airodis.ecotech.com.au/westconnex).
We then collect the information published there.

Here are examples of the information published:

![Screenshot of the homepage](2018-03-13_homepage.png)

![Screenshop of the Haberfield Public School AQM page](2018-03-13_haberfield_page.png)

![Screenshop of the Concord Oval AQM page](2018-03-13_concord_oval_page.png)

![Screenshop of the Allen St AQM page](2018-03-13_allen_st_page.png)

![Screenshop of the Powells Creek AQM page](2018-03-13_powells_creek_page.png)

![Screenshop of the Ramsay St AQM page](2018-03-13_ramsay_st_page.png)

![Screenshop of the St Lukes Park AQM page](2018-03-13_st_lukes_park_page.png)

## Dependencies

* SQLite 3
* PhantomJS

## Records

For each record we collect:

* **location_name**, the name of the air quality monitoring station, e.g.  'Haberfield Public School AQM'
* **scraped_at**, the date and time the data was collected by us
* **latest_reading_recorded_at**, the time the website says the reading was
  recorded, in the format provided
* **pm2_5_concentration**, Particulate less that 2.5 microns in equivalent aerodynamic diameter
* **pm10_concentration**, Particulate less that 10 microns in equivalent aerodynamic diameter
* **co_concentration**, Carbon Monoxide reading
* **no2_concentration**, Nitrgen Dioxide reading
* **diferential_temperature_lower**, "Differential Temperature - Lower" reading
* **diferential_temperature_upper**, "Differential Temperature - Upper" reading
* **wind_speed**, Wind Speed reading
* **wind_direction**, Wind Direction reading
* **sigma**, Sigma (Wind Direction stability) reading

See the information provided below for more information about what's recorded.

## Information provided

[The Information page](http://airodis.ecotech.com.au/westconnex/index.html?site=6&station=0)
on the WestConnex M4 East - Air Quality Monitoring includes the following text,
retyped here because it is an image of text there, rendering it inaccessible to screen readers etc. :

```
Definitions & Abbreviations

PM10 Particulate less that 10 microns in equivalent aerodynamic diameter
PM2.5 Particulate less that 2.5 microns in equivalent aerodynamic diameter
N02 Nitrogen dioxide
CO Carbon monoxide
WD Vector Wind Direction
WS Vector Wind Speed
Sigma Wind Direction stability
AT Ambient Temperature

Units

µg/m³ Micrograms per cubic meter at standard temperature and pressure (0ºC and
101.3 kPa)
ppm Parts per million
º Degrees (True North)
m/s Metres per second
ªC Degrees Celsius

Traffic light icons on Site Map page side bar

The green, orange and red circles indicate that data was successfully loaded to
the page at the last attempt.
This is not an indication of the pollution index or instrument status

Instantaneous data on the side bar of individual station summary tabs

These are real-time values showing the latest available five-minute result for
each parameter. Graphs show data averaged over periods which coincide with the
relevant air quality goals. As a result, these values may differ.

Disclaimer

The data use in the compilation of this website has undergone only preliminary
quality assurance checks. This data may require modification during the final
stages of validation as a result of calibration changes, power failures,
instrument failures etc
```
