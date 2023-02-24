# Requirements

## User Needs
The users should be able to see the total number of people visiting and should be able to interact with the web application.
They will not only see museums but also recommend things such as other local restaurants through google maps as this goes with our business goal which is to help local community. The information in which we are planning to showcase should be done in a simple way, for readability and plan to maybe add a translated website for tourist?
The web application will need to ask for users current location to pin point to the nearest museum.

### User stories
Our goal is to make it easy for users to see when the museums is busiest and when it is not. We might also apply some ways for more users to use the app such as giving free coupons for museum visit or getting a free coffee for a local restaurant. Our plan is to boost the local businesses and help them. 

### Actors
Our target demographic mostly consists of tourists, the elderly, and teenagers. We have choosen this target demographic as they are the most likely to need information about the local museums for things such as events and if the area is busy. We also want to target the older generations as we want to make a webpage that helps with readiablity.

### Use Cases
TODO: Describe each use case (one per team member).
    Give each use case a unique ID, e.g. UC1, UC2, ...
    Summarise these using the use-case template below.

| Use Case 1 (John) | Museum Data |
| ---------------------------------------------------- | ----------------------------------------------------- |
| **Description** | Tourist would like to know if the bristol museums are busy or not. |
| **Actors** | Tourist/User of App |
| **Assumptions** | Browser is able to show current data of museum. |
| **Steps** |    1. User opens web browser <br /> 2. Get data from Bristol Open Database <br /> 3. Shows the current number of people in the local museum and others.<br /> 4. Shows wether it is busy or not. <br /> 5. Be able to see wether a museum is busy or not print a text "Not Busy", "Moderately Busy", "Busy". 
| **Variations** | The browser may not support the code writen as some phones screen resolution may clutter the readablity of the text. |
| **Non-functional** | Could change how the web app is going to look. The sevice should be able to run on Google Chrome as this is the default browser of most phones and desktop. |
| **Issues** | An issue could a rise as the app will print the number of museum vistors accross all Bristol museum not just one. So if one museum is busy and another is not the web app will not be able to distinguish which is busy or not. | </td></tr>


| Use Case 2 (Elliott) | Popularity Data |
| ---------------------------------------------------- | ----------------------------------------------------- |
| **Description** | See historical popularity of Bristol's Musuems and therefore be able to decide which is most sought after. |
| **Actors** | Tourist/User of App |
| **Assumptions** | Browser will show popularity trends in museums over longer periods. |
| **Steps** | 1. User opens web browser. <br /> 2. Get data from Open Database. <br /> 3. Shows historical trends of popularity for different museums.
<br /> 4. Shows where most people visit and on what days so they can gauge what is most sought after to see. <br /> 5. Showing in bar graph of popularity over time. 
| **Issues** |  Reqiures updating over time as the information will change over the course of days/weeks/months. | </td></tr>


![image](https://user-images.githubusercontent.com/110387603/201328562-351a695f-1833-408e-8e1f-78b637ca5cc2.png)

## Software Requirements Specification
The program must be able to run on a browser as this will maximise the reach of people using the appilcation and is also universally accessible for not just mobile phone users but also on desktop. We will be using HTML language to create the webpage alongside be able to contact the database using mySQL. 

### Functional requirements

The system shall be able to cycle through the different webpages that we will create using the different tabs within the webpage. We will be required to learn how to design a webpage using various programming tools and be able to create a functioning site. We are also required to use the information from Bristol Opendata and add this to our webpage. 


### Non-Functional Requirements
TODO: Consider one or more [quality attributes](https://en.wikipedia.org/wiki/ISO/IEC_9126) to suggest a small number of non-functional requirements.
Give each non-functional requirement a unique ID. e.g. NFR1, NFR2, ...

Indicate which UC the requirement comes from.
