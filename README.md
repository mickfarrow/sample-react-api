# sample-react-api
Sample React application and API

# Terms

## Visual Studio

Visual Studio is an enterprise level IDE (Integrated Development Environment) from Microsoft.
You can develop many different types of application, using many different languages.

## VS Code

VS Code is an IDE from Microsoft, it is a scaled down version of Visual Studio. You can develop many different types of application using VS Code, but you will not get some of the WYSIWYG helpers that you get in Visual Studio

## API

Aplication Programming Interface, an API is a program that runs as a web service, and exposes end points. An end point is a web address, something like 

http://myshop.com/api/shirts/

http://myshop.com/api/shirts/1

When you call the endpoint, instead of a web page, you get back data which is in the form of JSON (Javascript Object Notation)

JSON is a way of describing the data and schema in one file.

https://www.w3schools.com/js/js_json_intro.asp

## Database

A database is a repository for storing data, there are many different types of database, MySQL, Mongo, Oracle, SQL Server etc.

Usually the type of data you are storing will push you towards one or other of the DB types, but for a regular database, a good choice is SQL Server.

## SQL Server (pronounced sequel server)

MS SQL Server is a database product from Microsoft. It has evolved over a number of years and is highly scalable. It is arguably the most popular DB in the world.

It is easy to create tables, add data etc. when using SQL Server. Visual Studio has a capability to do this, and also a free product SQL Server Management Studio (SSMS) has full functionality to administer your database.

SQL Server takes it's name from Structured Query Language (SQL), which is a simple language used to query data inside a database.

Not all Databses use SQL, but the main ones, SQL Server, Oracle all use ANSI Standard SQL.
.
https://www.w3schools.com/sql/sql_intro.asp

## UI

### MVC

The User Interface is the bit that you see, the web page. This is always HTML which is presented to the browser as a result of a HTTPRequest.
The browser (Edge, Chrome etc.) has a rendering engine that interprets the HTML and formats it on your browser.

No matter whether you code your site using C#, Python, PHP etc the end result is always HTML.

An MVC application is a web programming method that returns pages from the server, the server fetches the data, and then binds the data to some HTML, sending the whole page back to the browser.

With an MVC app there is no need for an API, as the MVC app has it's own endpoints.

MVC is a rather old fashioned way of writing web sites.

### Client Side UI

All browsers have a javascript engine that can run snippets of javascript code.

Client side applications will typically consist of a single html page, some styling information (css), and some javascript code. 

When you navigate to the web site, the html, css, and javascript are sent to the browser and loaded in to memory. 

The javascript code will bootstrap the application, and render the page with the initial view (home page). 

Now, as you click around the site, instead of making a round trip back to the server, the client side app will call out to API endpoints for data, and as it receives the data, it will redraw the UI on the browser.

This is much more user friendly as the site will not freeze when requesting a new page as it waits for the server code to run.

React, Angular and Vue are examples of Client Side Web Applications.

### Requests, Responses and Callbacks

With the traditional web site, you click a button, or a link, and this sends a HTTPRequest to the server, the request is processed, and passed back to the browser as a HTTPResponse. This is done synchronously, the browser will freeze and be unreponsive until the Response is received.

With the Client side way, the HTTPRequest goes to the API and is made asynchronously. The request is made, and a callback function is provided which waits for the response to arrive. The repsonse from the API is data only (JSON), and the app redraws only the part of the page which needs to display the data. 
