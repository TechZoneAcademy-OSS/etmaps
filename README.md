# etmaps
Maps combining data from Environics Trust (http://environicsindia.in) and  Data{Meet} Community Maps Project (https://github.com/datameet/maps). 
It's made available under the Creative Commons Attribution 2.5 India (http://creativecommons.org/licenses/by/2.5/in/)


##Development mode howto

tools/createmap.py
------------------
This script should finally create a blank map for local development
This includes
1. Creating a folder for the new map
2. Create a maps subfolder 
3. Create maps/css, maps/js, maps/icons, maps/data
4. Symlinking the mojomap libraries from the specified location
5. Copy over a sample mojomap html file
6. Optionally skip all of the above and use the cloud hosted versions of the js files

While this is not done the structure of a an et map is the same as a mojomap - 
```
< path to map >
|______maps
        |_____js
        |      |
        |      |_____mojomaps.js
        |
        |_____css
        |      |_____mojomaps.css
        |      |_____style.css
        |
        |_____data
        |      |_____< geojson files go here >
        |
        |_____mojomap.html (contains key to drive spreadsheet definition for map)
```