What is responsible for defining the routes of the games resource?
create_router.js

What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?
The client is responsible for displaying data to the user and taking user input. The server is responsible for defining the routes and handling reads from and modifications to the database.

What are the the responsibilities of server.js?
Server.js calls the database server. It calls CreateRouter to create the routes for the app. 

What are the responsibilities of the gamesRouter?
To carry out the routing and make calls to read / modify the databse.

What process does the the client (front-end) use to communicate with the server?
GamesService is called by GamesConainer. GamesService performs a fetch from the server.

What optional second argument does the fetch method take? And what is it used for in this application? 
The optional second argument is an init object. In this application, it is used to specify the method, the data to be passed to the server and hence to the database, and to describe the type of data being passed.

Which of the games API routes does the front-end application consume (i.e. make requests to)?
http://localhost:9000/api/games/ with POST.
http://localhost:9000/api/games/id with DELETE

What are we using the MongoDB Driver for?
The MongoDB driver is used to handle updating and deleting from the database.