# Implementation

## Introduction
This is version v0.6 of Bristol Museum Popularity Web App using data from Bristol Open Data's [Bristol Museums Daily Visitor Numbers
](https://opendata.bristol.gov.uk/explore/dataset/bristol-museums-daily-visitor-numbers/information/). This web app shows both the location of nearby museums (and a description of them) in Bristol and the historical popularity of those different museums.

Potential issues with this dataset is that it is limited in terms of the museums that it keeps popularity data on, something that can be adressed using outside information to supplement.

## Project Structure
The project structure (though not currently complete) is as such:

├── bristol-museums-daily-visitor-numbers.csv\
├── connection.js\
├── css code.css\
├── DBET.js\
├── node_modules\
├── opedata museum database.sql\
├── package-lock.json\
├── package.json\
├── SQL ISD.sql\
├── var express = require('express');.js\
├── var mysql = require('mysql');.js\
└── website.html

## Javascript Error Reports

| File Name | JSLint Warnings/Reports |
| --------- | ----------------------- |
|connection.js| Undefined variables: Used a variable that was not designed for our project scope. Changed this variable to avoid future errors.|
|DBET.js|'DatabaseConnection' is not defined. "return new DatabaseConnection(dbConfig);": The database was not defined or declared in the current scope. To resolve this warning need to make sure it was properly declared within the code. |
|var express = require('express');.js| 'require' was used before it was defined. This error indicates that JSLint does not recognize the require function and assumes it is an undefined variable. JSLint is not able to recognize Node.js-specific syntax or modules.|
|var mysql = require('mysql');.js| Same error as previous file where JSLint was not able to recognize Node.js-specific syntax or modules.  |



## Software Architecture
This is a 3 phase user-oriented architecture that begins with a web-app about Museum Popularity data, running on a Nodejs server that derives data from a MySQL database inhereted from Bristol Open Data (Bristol Museum Popularity)


The software architecture is as such:

![Insert your component Diagram here](https://github.com/Xerfed/ISD2022-23/blob/de0c830a949044985093fc76062d21264a2162a6/component%20updated.png)
