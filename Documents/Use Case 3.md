#Use Case: 3, User Navigates World and Views Reddit Content

###Characteristic Information

**Primary Actor:** Reddit Guest

**Goal:** Actor will be able to travel around our world, navigate to the Reddit content they desire, and view that content.

**Scope:** User Interface

**Level:** User Goal

**Trigger:** User opens our application

**Success End Condition:** User navigates world, views content, and exits

**Failed End Condition:** User told that content unavailable and application either exits or loads default structure

###Stakeholders/Interests

 * Reddit guests: Navigate and view content in the virtual world

 * Server: Receive correct requests for data and send it back to the user

 * Reddit: Requires its data to be appropriately used and represented, and to give user appropriate warnings when they attempt to access certain functions when not logged in

###Preconditions

 * Application is loaded

 * Server is currently running

 * User is connected to the internet and has a system with correct capabilities (windows, android)

###Minimal Gaurantee

 * The program will open and provide a correct error message

 * The program will handle errors from the server

###Main Success Scenario

1. User appears in the main page of the virtual world

2. User successfully navigates to desired content (subreddit, thread, comment)

 a) Using map

 b) Using searchbar

3. User views content

 a) If the user attempts to interact with content, the program will prompt the user to login or create an account

4. User downloads content to their device’s library (images, gifs, videos, etc.)

###Extensions

 * 1: Content unavailable (server down, server not responding, Reddit down etc.)
 
   + 1: Give error message
   
   + 2: Quit application

 * 2: Content unavailable (server down, subreddit private, Reddit down etc.)
 
   + 1: Tell user that the content is unavailable
 
   + 2: In background, continuously attempt to get content
 
   + 3: Load default structure in place of content

 * 3a: Reddit unavailable
 
   + 1: Tell user they are unable to login
   
 * 3a: Unable to login
 
   + 1: Respond with error message
   
###SCHEDULE

**Due Date:** release 1.0
