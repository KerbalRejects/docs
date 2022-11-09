# Software Requirements

## Vision
* Give the user the ability to search the night sky anywhere in the world. Return to the user a map of the night sky, weather data for the dates searched. And allow the user to select favorite searches, and add comments to those searches.

* Offers the user a one-stop-shop to Xplore the night sky and weather data for a given date range.

* Because people love space and curiosity. Half of all that is visible is "up", you should have an idea of what is up there.

## Scope (In/Out)


* Our app provides the user security and the ability to search locations, set favorite searches, view/modify their profile, provide information about the project team.

1. User authentication through Auth0
2. Gathering API data from AstronomyAPI, WeatherBIT, LocationIQ.
3. Display search data results (map of night sky and weather for the timeframe) on main page.
4. Allow the user to CRUD their profile, including favorites (adding comments, hearts, and deleting previous searches).
5. Utilize MongoDB to store data related to searches and user information.
6. Allow the user to logout and view information related to the project team.

Our MVP is as described above.

## Stretch Goals

* Allow the user to upload photos of the night sky that they took.
* Display the list of celestial objects.
* NASA Image of the day via NASA API
* Spotify playlist for space vibes

## Functional Requirements
List the functionality of your product. This will consist of tasks such as the following:


* A user can read, update, and delete objects in their favorites section.
* A user can search the night sky anywhere in the world,(by location name and date time) and it will return a map and the weather.
* A user can login through Auth0 without the need to create a new login.
* A user will be able to favorite the current search and see that favorite in their profile.
* A user can logout of the website.
* A user can view project team information.

The application data flow will start with the user logging into the webpage. From there they will be able to send a query to the server which will fetch results from 3 different APIs and return the data to display to the user. From there the user will be able to favorite the search using the CREATE method, which will add the favorite to the users profile. The user will then be able to visit the profile and READ, UPDATE, and DELETE the favorites. 

## Non-Functional Requirements (301 & 401 only)
Non-functional requirements are requirements that are not directly related to the functionality of the application but still important to the app.

* Security: Utilizing Auth0, CORS and environmental variables to secure the webpage and its endpoints. User will have to authenticate themselves to *use* the website. We will have one user role with NO admin access.
* Usability: Ensure accessibility, user satisfaction, simplistic and pleasant UI/UX design, 
* STRETCH GOAL: Portability: Mobile
