# Tornado-Database
United States tornado database consisting of vetted NCEI data and DAT tracks.

## Sources
### DAT
Most detailed tracks are sourced from the Damage Assessment Toolkit. Extra care is taken to ensure tracks are in the correct direction tornado traveled. Test cases are removed.

### Event Pages
Occasionally detailed tracks are sourced from event pages when not in DAT. Event pages may have detailed tracks in the form of KMLs or images. In the case of NWS OUN, most detailed tornado tracks are only in images from their tornado database.

### NCEI Storm Data
Official database of the NWS. When tornadoes are not in DAT they are sourced from Storm Data. Stats such as length, width, damage, injuries/fatalities and narratives are from Storm Data. Occasionally Storm Data contains errors or inconsistencies from PNS and DAT sources and are marked in the error spreadsheet.

### LSR
Local Storm Reports are mainly used for near real-time tornadoes when other sources are not available. Most are removed once final yearly data is available. Occasionally tornadoes are only recorded in LSRs and care is taken to ensure these reports are credible, missing tornadoes during the post year review.

## Derived data
### Storm Morphologies and tornado types
A low resolution radar image of the system is reviewed to determine storm type. The time of tornado is also validated using this radar data. Since the images used are low resolution, the certainty of storm type may be less than with level-2 resolution. Often QLCS are used to describe embedded supercells. Tornado types are given as either tornadic or landspout in nature from event narratives.

### MRMS Convective Features
Some years have convective feature data. The tornadoes have been paired with MRMS 6-minutely data and contain basic radar properties and shapes from the MRMS dataset. This is an automated process and does not gurentee accuracy in the pairing of tornadoes and features.
