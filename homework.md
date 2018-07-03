**Questions**

What is responsible for defining the routes of the games resource?
 - gamesRouter.js is reponsible for defining the routes.

What are the the responsibilities of server.js?
- server.js connects with data persisted to the database with games_hub. It uses a body parser to access the request's body and extracts it from a POST request to make it accessible. It also specifies the gamesRouter with the use method.


What are the responsibilities of the gamesRouter?
- the gamesRouter handles requests and inserts new data into the gamesCollection and provides a response.

Which of the games API routes does the front-end application consume (make requests to)?
- GET(index), POST(new) and DELETE(destroy) are the routes which the front-end application consumes? Sorry, not sure if I fully understood the question.



**Extensions**

What are we using the MongoDB Driver API for?
- We use mongoDB Driver API because it's non-relational and can handle large collections of objects with different properties and stores this data in JSON docs which are perfect for JS. The MongoDB Driver is an an API that enables us interact with the MongoDB database from inside our JavaScript application.

Why do we need to use ObjectId from the MongoDB driver API?
- We need to use ObjectID to determine the ID of a specific object as a first step to updating it's details in PUT.

suggested: "When the front-end makes a request regarding a specific game (SHOW, UPDATE, DELETE), the server access the ID of the particular game from the params object. This is always a string. To query the database for an object of a particular ID, if we ask it for the object with the ID of string type, it will never find a match. It needs us to make the query with an instance of ObjectId. We create the instance of ObjectId by passing in the ID as a string, for example, ObjectId("5af17fe430e043c3e62149b8")."
