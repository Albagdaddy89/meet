
MeetApp is an innovative, user-friendly web application designed to enhance the experience of event discovery and participation. Tailored for individuals who seek to engage with various events, MeetApp offers a suite of features that streamline the process of finding and attending events, both locally and globally.

Key Features:
Filter Events by City: Users can effortlessly search and filter events based on city locations, allowing for a customized view that focuses on their area of interest.

Dynamic Event Details: With a clean and intuitive interface, event details are initially collapsed for easy browsing, and can be expanded upon user request to access more information, ensuring a clutter-free experience.

Customizable Event List: MeetApp adapts to user preferences by displaying a default or user-specified number of events, offering flexibility and control over the amount of information presented.

Offline Accessibility: Understanding the need for constant access, MeetApp provides offline functionality, displaying cached event data, ensuring that users remain informed even without an internet connection.

Home Screen Shortcut: For ease of access, users can add MeetApp as a shortcut on their device’s home screen, streamlining app usage and enhancing user engagement.

Event Analytics Visualization: A unique feature of MeetApp is its ability to visually display event data, such as the distribution of upcoming events across various cities, aiding users in their decision-making process.

Project Goal:
The primary aim of MeetApp is to simplify the process of finding and attending events, making it more accessible, convenient, and tailored to individual user needs. Whether you're a casual event-goer or a frequent participant, MeetApp is designed to enhance your event-discovery journey.

Technology Stack:
React.js for a responsive and dynamic user interface.
Advanced caching techniques for offline functionality.
Integration with event databases and APIs for real-time data.
Data visualization tools for interactive and informative charts.
-------------------------------------------------------------------------------------------------------

Feature 1: Filter Events By City
Scenario 1:

Given the user has not searched for a city,
When they open the app,
Then they see upcoming events from all cities.
Scenario 2:

Given the user starts typing in the city search box,
When they enter some characters,
Then they see a list of city suggestions based on the input.
Scenario 3:

Given the user sees a list of city suggestions,
When they select a city from this list,
Then the app displays upcoming events for that selected city.
Feature 2: Show/Hide Event Details
Scenario 1:

Given the user views the list of events,
When they initially see an event element,
Then it is collapsed by default.
Scenario 2:

Given an event element is collapsed,
When the user clicks on the event,
Then the event expands to show more details.
Scenario 3:

Given an event element is expanded,
When the user clicks on the event again,
Then the event collapses to hide the details.
Feature 3: Specify Number of Events
Scenario 1:

Given the user has not specified the number of events,
When they open the app or view the events list,
Then 32 events are shown by default.
Scenario 2:

Given the user views the events list,
When they adjust the settings to change the number of events displayed,
Then the events list updates to show the specified number of events.
Feature 4: Use the App When Offline
Scenario 1:

Given there is no internet connection,
When the user opens the app,
Then the app shows cached data.
Scenario 2:

Given there is no internet connection and the user is viewing cached data,
When the user tries to change search settings (city, number of events),
Then the app shows an error message.
Feature 5: Add an App Shortcut to the Home Screen
Scenario 1:

Given the user is using the Meet app,
When they choose to add the app to their device's home screen,
Then the app is installed as a shortcut on their home screen.
Feature 6: Display Charts Visualizing Event Details
Scenario 1:

Given the user is viewing the events list,
When they access the section for event analytics,
Then the app displays a chart visualizing the number of upcoming events in each city.
These user stories can be used to guide development, ensuring that the app is user-friendly and meets the needs and expectations of its users.

-----------------------------------------------------------------------------------------------------
Feature 2: Show/Hide Event Details
As a user,

I should be able to view a list of events with their details collapsed,
So that I can quickly browse without being overwhelmed by too much information.
As a user,

I should be able to expand an event to see more details,
So that I can learn more about events I'm interested in.
As a user,

I should be able to collapse an expanded event,
So that I can simplify the view when I've finished reading the details.
Feature 3: Specify Number of Events
As a user,

I should see a default number of events (e.g., 32) when I haven't set a preference,
So that I can have a standard, manageable list of events to start with.
As a user,

I should be able to specify the number of events I want to see,
So that I can customize the list according to my reading preference or time constraints.
Feature 4: Use the App When Offline
As a user,

I should be able to view cached event data when I'm offline,
So that I can access event information without an internet connection.
As a user,

I should receive an error message when changing search settings while offline,
So that I understand why I can't update search criteria without an internet connection.
Feature 5: Add an App Shortcut to the Home Screen
As a user,

I should be able to install the app as a shortcut on my device's home screen,
So that I can quickly and easily access the app without navigating through the browser.
Feature 6: Display Charts Visualizing Event Details
As a user,

I should be able to view charts visualizing event details, like the number of upcoming events per city,
So that I can get a quick graphical overview of event distribution and plan my participation accordingly.
-------------------------------------------------------------------------------------------------------
In the Meet app, we use serverless functions to make the app run smoothly. This means we handle things like getting data, sending notifications to users, and updating content without needing a lot of complex infrastructure. Serverless functions help our app handle more users easily, especially when lots of people use it at the same time. This makes sure the app works well for everyone, no matter how busy it gets. Also, by using serverless, we keep our costs low and make things less complicated behind the scenes. This lets us spend more time making cool new features and making sure our users have a great experience. Our main aim is to make Meet a fun, easy-to-use app for finding and joining events.

