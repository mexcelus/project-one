# FreeTime App :date: 

Appointment/Meeting scheduler. 
Create an event and find a time that works best for EVERYONE.

####  Created using HTML, CSS, JavaScript, jQuery, Uikit, Firebase


## Application Overview

* Event organizer fills out form on landing page to create an event.
* organizer enters their availability by checking appropriate boxes on time selection screen.
	* on submit of time-selection, organizers is presented with 2 unique URLs.
		* first link is to send out to participants to enter their availability.
		* second link is for organizer, once all participants have entered their availability. 
* link is copied to clipboard to forward to participants to enter their availability. 
	* when a participant enters their times, a notification is displayed on the screen, and the times are stored in the database.
	* when final participant has entered their time page will display "all responses recorded"
* organizer follows organizer URL when all participant entries have been recorded
	* most popular time for all responses is displayed tot he page
	* if no best time is available, the page displays which user's had conflicts

## Code Overview
the application uses forms to collect user data. user data is stored in Firebase. hashids library is used to generate unique id's and create unique URLs for organizer and participants. user times are stored in an array and pushed to database. once all user times have been entered, each user time array is evaluated to assert a match based on the data-time attribute of each checkbox. if a match exists, the match is displayed when the organizer visits the URL generated by hashids. if conflicts exist, the name of the user is displayed to the page. Organizer is presented with add to calendar button, to call google calendar API to add it to the calendar for all users. 

## Deployed Project

[FreeTime App](https://mexcelus.github.io/freetime-app/) - Create an event and find a time that works best for EVERYONE.



## Authors

* **Cody Bender** - *front-end/database/backend* - [cfbender](https://github.com/cfbender)
*  **Chris Lucynski** - *front-end (HTML/CSS/Uikit/JavaScript)* - [chrislucynski](https://github.com/chrislucynski)
*  **Gerritt Black** - *front-end/API(HTML/CSS/Uikit/JavaScript)* - [gmocore](https://github.com/gmocore)
* **Guillermo Villalta** - *front-end/API (HTML/CSS/Uikit/JavaScript)* - [mexcelus](https://github.com/mexcelus)



