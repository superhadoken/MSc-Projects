# MSc-Projects
Enterprise Architecture Project


EntProject Application -
This contains both the HTTP call webservices and the AJAX, GAE implementation. Both are deployed to the GAE and available at:

http://1-dot-momutlak-ent.appspot.com/

On load you are presented with 4 hyperlinks which will allow you to access different parts of the web application.

*EntProject*
This is a proof of concept application of a servlet and serves no purpose other than to show a http call to the servlet and the returned text from the servlet "Hello World".

-Show servlet concept functioning
-Return Hello World

*add Films to the GAE*
This link provides access to a web form to create FilmInfo objects which are persisted in the GAE datastore once the submit/add film button is clicked. The server then takes you to a JSP page in which all of the entities in the datastore are displayed in a table.

-Add Film to Datastore via HTTP Form
-Request display of all films upon persistence
-Display JSP page with all stored films

*all Films in Datastore*
This is a HTTP call to the servlet which produces 4 different return type formats for the data. The data type returned is selected via the drop down box.

-Select preferred data type return
-Display all films in datastore in selected datatype
-Available data types:
		~JSON
		~Plain Text
		~HTML Table
		~XML

*AJAX Implementation*
This link provides access to the AJAX version of the above web application. The resulting jsp page is split up into 3 sections.

	~Add Film
Similiar in nature to the previous html form, this form creates a FilmInfo object and persists the object to the datastore. It is a HTML5 page so the input fields are required. Upon submit, an alert box is generated informing the user the film was added. Then all films are retrieved and displayed at the bottom in the DataStore Display section.

-Add Film to Datastore via Ajax 
-Ajax javascript request to retrieve all films in datastore in table
-Insert table into page without refresh/reload.


	~Search Films

Film search that uses text input to match up to Film titles. Results can be displayed in a variety of formats.


	~DataStore Display

Display all current films in the datastore in a table format
