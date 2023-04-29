# Bristol Museums Daily Visitor Numbers 


<write introduction to project basis>

A website that showcases the total visitors to the Bristol museums historically. [The dataset is available on Bristol Open Data]
It will carry a friendly user interface that provides easy readability for the viewer alongside containing some aspects that may encourage the users to use the website.


## Credits:

<outline work credit>

1. [Planning](docs/planning.md) - John/Elliott/Harrison for Text (solely John for Diagram)

2. [Requirements](docs/requirements.md) - Elliott and John for all (indicated where in Requirements page)

3. [Design](docs/design.md) - Elliott and John for Sequence Diagram, Elliott and John for 
Wireframe Diagrams

4. [Implementation](docs/implementation.md) - Elliott entirely (coding, text, and diagrams) Javascript Error table by John

<all comments here written by Elliott>

  
HTML CODE: 
<html>
  <link rel="stylesheet" href="/style.css">
  <!-- A button for the next page in the website -->
  <a href="second-page.html"><button> Historical Data </button></a>
  <a href="second-page.html"><button1>  </button1></a>
  <!-- This is the heading of the website -->
  <h1>Bristol Museums Daily Visitor Numbers</h1>
  <b> </b>
  <!-- Embedded information from opendata -->
  <iframe src="https://opendata.bristol.gov.uk/explore/embed/dataset/bristol-museums-daily-visitor-numbers/table/?dataChart=eyJxdWVyaWVzIjpbeyJjb25maWciOnsiZGF0YXNldCI6ImJyaXN0b2wtbXVzZXVtcy1kYWlseS12aXNpdG9yLW51bWJlcnMiLCJvcHRpb25zIjp7fX0sImNoYXJ0cyI6W3siYWxpZ25Nb250aCI6dHJ1ZSwidHlwZSI6ImxpbmUiLCJmdW5jIjoiQVZHIiwieUF4aXMiOiJudW1iZXJfb2ZfdmlzaXRvcnMiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiIjRkE4QzQ0In1dLCJ4QXhpcyI6ImRhdGVfbG9nZ2VkIiwibWF4cG9pbnRzIjoiIiwidGltZXNjYWxlIjoieWVhciIsInNvcnQiOiIifV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWUsInRpbWVzY2FsZSI6IiJ9&static=false&datasetcard=false" width="630" height="250" frameborder="0"></iframe>
  
<!-- Embedded map for popular Bristol museums using Google Maps (Map pin locations - created by John) -->
<h2>Maps<h2>
<iframe src="https://www.google.com/maps/d/u/0/embed?mid=18Ol0N_5bJzC8FGVZOLOyelNJyaYNkP4&ehbc=2E312F" width="640" height="480"></iframe>
  

<b2> </b>
</div>
</html>

  
  
CSS CODE:   
button {
  float: left;
  margin-right: 10px;
} 

h1 {
	font-size: 2rem;
	font-weight: bolder;
	margin-bottom: 1rem;
}

body {
	font-family: sans-serif;
  text-align: center;
	padding: 3rem;
	font-size: 1.125rem;
	line-height: 1.5;
  transition: all 725ms ease-in-out;
}

  h2 {
    text-align: center;
  
  }
  
  
  var mysql = require('mysql');

var connection = mysql.createConnection({
    "host"     : "mysql5.cems.uwe.ac.uk",
    "user"     : "fet19004181",
    "password" : "6Jrbh1",
    "database" : "fet19004181"
});

connection.connect(function(err){
    if (err) {
        console.error("Connection error: ", err.message);
    } else {
        console.log("Connected as: ", connection.threadId);
    }
});

  
  
Javascript (Error)
var QUERY = "SELECT * FROM `bristol-museums-daily-visitor-numbers`";

connection.query(QUERY, function(err, rows, fields) {
    if (err) throw err;
    for (var i=0; i<rows.length; i++) {
        // change these attributes to those in your database
        var museum = {};
        museum.name = rows[i].Name;
        museum.visitors = rows[i]['Number of visitors'];
        console.log(museum.visitors, museum.name);

        var date = {};
        date.logged = rows[i].Date_Logged;
        console.log(date.logged);
    }

});

connection.end();

console.log("finished");

    
