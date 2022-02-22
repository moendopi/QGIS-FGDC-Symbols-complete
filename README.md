# QGIS-FGDC-Symbols-complete
An XML sheet to symbolize all of the FGDC available symbols
This XML sheet was created using the SLYR plugin in QGIS giving the tool an ESRI style file with all the FGDC symbols in it. 

The sheet has symbology for lines, points, and area fill colors for polygons.

When symbolizing you will need a Symbol field as a string. Unfortuantely, how the symbol codes are shown in the FGDC PDF is different than how the style sheet works. 
For instance, if you want to use 1.1.1 for a contact, the symbol field needs to have 01.01.01 in it. Matching symbols to a style is similar to in ArcGIS. 
Go into the Properties menu for the give shapefile/feature class - > Symbology tab - > Categorized for the top drop down, the symbol field for Value, 
then in the bottom right corner under the Advanced drop down select Match Symbols from a File and navigate to where ever the XML sheet is located. A pop up will appear
indicating how many symbols were matched, click okay, then apply. Done. 

** If you have no current install of ArcGIS or if you don't have the FGDCGeoAge fonts installed you will need to go to https://ngmdb.usgs.gov/Info/standards/GeMS/ and download the fonts from the two links under Fonts. These 6 fonts are necessary for the symbology and labels to work correctly in QGIS.
