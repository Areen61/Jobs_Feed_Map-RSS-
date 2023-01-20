Flutter Jobs Feed Map App

This is a Flutter application that displays a list of jobs and their locations (city/country), after fetching them from the RSS field Url, while also locating them on the map. The application makes use of the Flutter Map and Nominatim API to display the markers on the map.

Getting Started
To run this application on your local machine, you will need to have Flutter installed. You can follow the instructions on the Flutter website to install Flutter.
You will also need to get an API key from Nominatim API. You can sign up for an API key on the Nominatim website

Usage
Clone this repository to your local machine using the command git clone https://github.com/Areen61/Jobs_Feed_Map-RSS-.git
Open the project in your preferred IDE an make sure that you have the Flutter SDK installed.

Replace the API_KEY in the getCoordinates( ) function in the Job class with your actual API key.
Run the application on an emulator or a physical device by clicking the run button in your IDE or by using the command flutter run in the terminal.
The application should launch and display markers on the map for the jobs on the RSS feed from https://www.rotanacareers.com/live-bookmarks/all-rss.xml

Features
Displays job listings from an RSS feed on a map using markers
Uses the OpenStreetMap API to retrieve the latitude and longitude of job listings
Allows for zooming and panning on the map

Limitations
Only works with the specific RSS feed URL provided in the code
Only displays markers for job listings that have valid latitude and longitude coordinates

Future Improvements
Allow the user to input their own RSS feed URL
Display more job listings on the map
Add the ability to filter job listings by location or job title

Dependencies
    http: ^0.13.5
    xml2json: ^5.3.6
    url_launcher: ^6.1.7
    flutter_map: ^3.1.0
    latlong2: ^0.8.1

Customization
You can change the maxItems variable to control the number of job markers displayed on the map, but you should consider the actual items number in the feeds you choose.
You can also change the RSS feed URL in the getFeedData() function to display job markers from a different RSS feed

Note
The code uses a hardcoded RSS feed URL, and this may not be available or accessible. So you can use any other RSS feed of your choice.
Also, the code uses nominatim.openstreetmap.org to get the latitude and longitude of the job location, but this service has usage limits, so it may not work as expected. You can use any other service to get the coordinates.

