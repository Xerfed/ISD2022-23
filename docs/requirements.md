   # Requirements

## User Needs
The users should be able to see the total number of people visiting and should be able to interact with the web application.
They will not only see museums but also recommend things such as other local restaurants through google maps as this goes with our business goal which is to help local community. The information in which we are planning to showcase should be done in a simple way, for readability and plan to maybe add a translated website for tourist?
The web application will need to ask for users current location to pin point to the nearest museum.

### User stories
Elliott (Museum Popularity):
Role: User in Bristol; avoidant of overly busy museums, not familiar with info on Museums or Bristol in general.
Goal: Aiming to both locate nearby museums, find out about them but more importantly equate name of museum to historical popularity data.
Benefit: Web app shows both map of Bristol Museums and correlating popularity data, (intended, not yet implemented) secondary page with drop down selection that compares 2/3 museums with bar graph data representating popularity.

Our goal is to make it easy for users to see when the museums is busiest and when it is not. We might also apply some ways for more users to use the app such as giving free coupons for museum visit or getting a free coffee for a local restaurant. Our plan is to boost the local businesses and help them. 

### Actors
Our target demographic mostly consists of tourists, the elderly, and teenagers. We have choosen this target demographic as they are the most likely to need information about the local museums for things such as events and if the area is busy. We also want to target the older generations as we want to make a webpage that helps with readiablity.

### Use Cases

| Use Case 1 (John) | Museum Data |
| ---------------------------------------------------- | ----------------------------------------------------- |
| **Description** | Tourist would like to know if the Bristol museums is busy as they would like to visit off peak hours. |
| **Actors** | Tourist/User of App |
| **Assumptions** | Browser is able to show current data of museum. |
| **Steps** |    1. User opens web browser <br /> 2. Get data from Bristol Open Database <br /> 3. Shows the current number of people in the local museum and others.<br /> 4. Shows wether it is busy or not. <br /> 5. Be able to see wether a museum is busy or not print a text "Not Busy", "Moderately Busy", "Busy". 
| **Variations** | The browser may not support the code writen as some phones screen resolution may clutter the readablity of the text. |
| **Non-functional** | Could change the apperance of the app. The sevice should be able to run on Google Chrome as this is the default browser of most phones and desktop. |
| **Issues** | An issue could a rise as the app will print the number of museum vistors accross all Bristol museum not just one. If one museum is busy and another is not the web app will not be able to distinguish which is busy or not as it only shows the data of the most popular museums in Bristol. | </td></tr>

| Use Case 2 (Elliott) | Popularity Data |
| ---------------------------------------------------- | ----------------------------------------------------- |
| **Description** | See historical popularity of Bristol's Musuems and therefore be able to decide which is most sought after.  |
| **Actors** | User seeking least or most busy museums. |
| **Assumptions** | Browser will show popularity trends in museums over longer periods.|
| **Steps** |    1. User opens web browser. <br /> 2. Get data from Open Database. <br /> 3. Shows historical trends of popularity for different museums <br />4. Shows where most people visit and on what days so they can gauge what is most sought after to see. <br /> 5. Showing in bar graph of popularity over time. 
| **Issues** | Requires updating MySQL database over time as the information will change over the course of days/weeks/months as Bristol Open Data is updated. | </td></tr>

### Use Case Diagram
![image](https://user-images.githubusercontent.com/110387603/201328562-351a695f-1833-408e-8e1f-78b637ca5cc2.png)

## Software Requirements Specification

Software Requirements Specification (John)

The program must be able to run on a browser as this will maximise the reach of people using the appilcation and is also universally accessible for not just mobile phone users but also on desktop. We will be using HTML language to create the webpage alongside be able to contact the database using mySQL. 

### Functional requirements

Functional Requirements (John)

The system shall be able to cycle through the different webpages that we will create using the different tabs within the webpage. We will be required to learn how to design a webpage using various programming tools and be able to create a functioning site. We are also required to use the information from Bristol Opendata and add this to our webpage. 


### Non-Functional Requirements

Non-Functional Requirements (John)

**Maintainability** -  This is a way to provide bug fixes and updates to the webpage. By being able to maintain the webpage and providing constant updates this can increase the longevity of the webpage and for the users to keep interacting and using it.

Some functions that will help with the performance and maintainability of the website are:
- Real time monitoring of the website: This would help to continuosly monitor any problems that pop up in the website such as the server response time, website uptime and the status of the database.
- Code optimisation: Downsizing the code needed for operations can help reduce any unecessary computations which would help with the maintainance and the efficiency of the website as a whole. 
- Content delivery: By adding content to the website such as information in the front page would help to attract more users and can enhance the website as there are more things for the user to do. From a business stand point this is important for maintaining their current user base. 


**Efficiency** - This focuses on the effectiveness of the website to the consumer and wether or not it is using the resources allocated to it to deliver and meet the websites objectives. Some ways that the website could be more efficient is through the design, functions and optimisations. 

Some functions for the website that focus on this subject are: 
- Performance Optimisation: The website should be optimised for efficient performance with fast loading times as this will allows the users to have a smooth experience when running the site. 
- Scheduled backups: This will ensure that the entire website's database and files will be backed up to a cloud server which ensures the safety of the website's data and files. This should be done in off-peak hours to avoid any impact on the websites performance.
- Scalability: The website needs to be able to handle lots of user traffic as this could affect the performance. Scalability will help with the various changes in traffic as it will help with the changing visitor load especially during the peak periods or if there any special events. 
- Different browser compatibilities: By ensuring that the website is able to run on different browsers and devices the user will be able to fee consistency and have trust on the website being used regardless of what platform they are using. 
- Website UI (User Interface): This is an important part of the efficiency of the website as by having a good website UI would mean that the users are able to navigate through the website with ease. This will help to provide an efficient user experience as it will help the user find the information in the website and easily find what they are looking for.


Non-Functional Requirements (Elliott)

**Portability** - The ability to use the app both on your PC and phone, therefore it can be used out and on foot for touriosts travelling around, therefore the need to develop the website to be visible and working on both phone and PC and having different UI's for each.

**Reliability** - Given the infrequent updating of the open database and how infrequently museums are closed down/opened, it would only take minimal effort to make sure that the data and map provided have recent information.

**Functionality** - The data is accurate up to the point of Bristol Open Data's data and updates alongside that using MySQL. Given the simplistic design of the app, it is intended to work on both desktop and phone views.

**Usability** - The program is designed with simplicity in mind; the aims of the web-app are to simply show you where you are in relation to local museums, and provide you with historical data based on these museums. This is a two page process with no unnecessary information in between.

### Quality Attributes (Elliott) (Use Case For Museum Popularity)

**NFR1: Interoperability** - The function of the web app is based on and reliant to the connectivity between itself, MySQL and by extension, MySQL's connectivty to Bristol Open Data. Working as a system of derivement from other systems.

**NFR2: Accuracy** - The web apps accuracy is as accurate as any other data that can be obtained about Bristol's Museum Popularity; though can only be up-to-date with how often Bristol Open Data is.
