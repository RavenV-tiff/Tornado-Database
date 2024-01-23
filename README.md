# Tornado-Database
United States tornado database consisting of vetted NCEI data and DAT tracks.

## Sources
### [DAT](https://apps.dat.noaa.gov/stormdamage/damageviewer/#)
Most detailed tracks are sourced from the Damage Assessment Toolkit. Extra care is taken to ensure tracks are in the correct direction tornado traveled. Test cases are removed.

### Event Pages
Occasionally detailed tracks are sourced from event pages when not in DAT. Event pages may have detailed tracks in the form of KMLs or images. In the case of NWS OUN, most detailed tornado tracks are only in images from [their tornado database.](https://www.weather.gov/oun/tornadodata)

### [NCEI Storm Data](https://www.ncdc.noaa.gov/stormevents/)
Official database of the NWS. When tornadoes are not in DAT they are sourced from Storm Data. Stats such as length, width, damage, injuries/fatalities and narratives are from Storm Data. Occasionally Storm Data contains errors or inconsistencies from PNS and DAT sources and are marked in the error spreadsheet.

### [LSR](https://www.spc.noaa.gov/climo/reports/)
Local Storm Reports are mainly used for near real-time tornadoes when other sources are not available. Most are removed once final yearly data are available. Some tornadoes are only recorded in LSRs and care is taken to ensure these reports are credible, missing tornadoes during the post year review.

## Derived data
### Storm Morphologies and Tornado Types
Low resolution radar imagery of tornadic systems are reviewed to determine storm type. The time of tornado is also validated using this radar imagery. Since the images used are low resolution, the certainty of storm type may be less than with native level-2 resolution data. Tornado types are given as either tornadic or landspout in nature from event narratives.
#### Supercell example
![image](https://github.com/RavenV-tiff/Tornado-Database/assets/60206946/0b546b52-6f74-40bc-aad0-9417023ce5bf)

Classification for rotating descreate cells. Often associated with strong tornadoes.

#### QLCS example
![image](https://github.com/RavenV-tiff/Tornado-Database/assets/60206946/c3e1dc94-6c36-41d6-9dd1-9bc1eb874eb1)

Classification for a line of cells. Hybrid or embedded supercells are included in this group.

#### Disorganized example
![image](https://github.com/RavenV-tiff/Tornado-Database/assets/60206946/6cee888e-f666-47ef-b302-7117ebc114ad)

Classification for unorganized cell or group of cells. Most often associated with landspout tornadoes.

### MRMS Convective Features
Some years have convective feature data. The tornadoes have been paired with MRMS 6-minute data and contain basic radar properties and shapes from the MRMS dataset. This is an automated process where the area under the fitted ellipse is paired with a collocated tornado. However, there's no guarantee the feature paired is the correct one for the tornado. A convective feature is a grouping of four countinuous 1-km pixels of 40 dBZ composite reflectivity or greater.
