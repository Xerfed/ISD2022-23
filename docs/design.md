# Design

## Behavioural design

### Elliott's (UC2) Sequence Diagram

<Create sequence diagram to show user interaction with app>

![image](https://user-images.githubusercontent.com/116878977/222710207-10388509-5556-4d48-899c-44d5598a5bf4.png)

### John's (UC2) Sequence Diagram for a website support system
![image](https://user-images.githubusercontent.com/110387603/235287239-86e941e3-9ae1-46f1-958c-16a6841f6e49.png)
We have decided to explore a way to give the best user experience for our website and this is a diagram which shows how the website will help with users queries and for those who requires assistance.

<Create wireframes to show functions of web app>

## User Interface design (UC1) 
(John)
 
This is a rough idea of what the overall webpage will look like. [Some of the design may be altered at the final stage of implementation.]
Our initial design includes:
- "A Home Page": 
  Within the homepage we will include the total of people visiting the museums using the Bristol Museum OpenData. 
  We plan to create a small text box which showcase information on the popular museums alongside local events. This should also be easy to change.
- "Popular Museums Data":
  This is all the data from Bristol OpenData regarding the museum visits all time. Showcases the historical popularity data of the museum. 
- "Museum List":
   This will be a page that is dedicated to to showcase the most popular museums in the area with detailed explaination about it.
- "Map": A map of the museums which include a short information on the museum using google maps api alongside images of the museum.
  
  
**Johns's Use Case (UC2) Wireframe:**
![image](https://user-images.githubusercontent.com/110387603/221118292-3bf6b68a-c122-4350-851b-80cc99ee36a0.png)


**Elliott's Use Case (UC2) Wireframe:**

This is the prospective design layout and flow of the website from the perspective of assertaining museum popularity data:

An initial page would demonstrate information about the purpose of the web-app, located on the left would be hyperlinks that take you to a map, oriented on your location, that shows (labeled) museums in Bristol near you; click on these would give you a description of said museum.

"Busy Locations" would take you to a page that shows you (as current as possible) data about the popularity of a given museum (decided by dropdown selection). Intended to be informed by hour-to-hour averages instead of realtime.

"Popularity Data" would give you similar information and data choice that is instead informed by historical data on a larger scale, instead of hour to hour, derived from the MySQL database from Bristol Open Data.

![image](https://user-images.githubusercontent.com/116878977/208084953-b898d27c-d399-4c7d-84f1-3db6a32ddba3.png)
