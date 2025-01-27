The CAMA Viewer Repository is a reconfigurable web-application built using the latest version of the ArcGIS JavaScript SDK Version 4.26 and the Calcite framework Version 1.3.0. The application uses one Javascript file to reference the cama folder containing all of the JSON files. Upon entering the proper syntax as stated below, the application will be reconfigured on the fly, for the desired CAMA viewer experience. 

To Take advantage of the JSON file configurations in the URL, the proper syntax is ?viewer=cama(json folder name)/Chester(JSON file Name) the correct spelling of the JSON file is imperative for the code to run properly. 

       i.e. ?viewer=cama/Chester

To take advantage of the query functionality in the URL, you add on to the current URL string: &query=Layer Name,Field Name,Feature

	http://127.0.0.1:5500/index.html?viewer=cama/Washington&query=Parcel%20Boundaries,Uniqueid,3143
	
The user will type in query=Parcel Boundaries,Uniqueid,3143, where the code will automatically encode the URL for you upon
making your request. Not requiring the user to concern themselves with spaces, but only the proper spelling of Feature Layers, Field Names 
(not the Alias name),and the desired Feature. 
	
If no JSON file is specified in the URL, the application will fall back to the North_Haven JSON file configuration. 



