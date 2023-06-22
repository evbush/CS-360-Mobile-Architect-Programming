# CS-360

### Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
The requirements and goals for this app were to create an event tracking app that allowed users to login or register an account. These logins needed to be stored in a database. Once they user was inside the app, they needed to be presented with a table of all events and have an ability to create new ones and edit or delete already created ones. These events needed to be stored in a database as well.


### What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
The first screen and feature needed was a login mechanism to verify the user’s identity. The main feature of this screen was to prompt the user to create and register an account if we did not find their username in the database. The next screen was the event list. The main feature was giving the user the ability to search for their events via an on screen calendar. In order to find their event, they had to select the correct date on the calendar. Then the list of events would appear under the calendar in an agenda section. The final key features were allowing the user to add, edit, and delete events. The main idea behind the add and edit functionality was to provide the screen as a dialog fragment to keep the user on the home screen while performing these actions. My UI designs were meant to keep the user engaged with the main purpose and theme of the app. I believe my designs were successful because the user doesn’t need to leave the main screen at all during their time within the app.


### How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?
I approach the coding process by building out the databases first. I want to make sure I can store any data as I build out the functionality. The technique I use is following the flow of the user experience as I build out each screen an activity. I tried to modularize sections, just in case I would need to move them around. The main concept I applied was creating a model of the events to help store data that was being sent or received from the core database. This allowed me to work with the data in any way I needed to. This all can apply to future development by ensuring code is modular-based while also encapsulating data within models.


### How did you test to ensure your code was functional? Why is this process important and what did it reveal?
I tested my code by physically working through the app in the emulator. It was effective but not efficient. A more efficient method would have been creating some unit tests to make sure core functionality worked. However, testing through the emulator allowed me to view the design and functionality in the eyes of the user. It helped me pick out key issues or concerns on features. 


### Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?
For the full process, I had to overcome an issue of connecting all of my activities to the database. I implemented a controller class to operate as the middleware to perform the business logic of the app. This allowed me to manipulate the data as needed. One challenge faced by this was allowing my main activity to prompt the controller to send event data to a dialogue fragment that lets the user edit a chosen event. The trouble was transferring the model. I ended up updating my event model to a parcelable class.


### In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I believe the main activity, add event, and event controller components were the most successful. They helped demonstrate my ability to create a seamless user experience. For example, whenever a user added or deleted an event, the agenda list would automatically update in their view. This would allow a user to see their changes in real time. Another example would be my use of separating the UI, business logic, and the data. I think that is a vital process to ensure correct usage of functions when it comes to usable data.

