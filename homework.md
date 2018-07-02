**Questions**

What is responsible for defining the routes of the games resource?
 - create_router.js is reponsible for defining the routes.

What are the the responsibilities of server.js?
- server.js connects with data persisted to the database. It uses a body parser to access the request's body and extracts it from a POST request to make it accessible. It also specifies the gamesRouter with the use method.


What are the responsibilities of the gamesRouter?
- the gamesRouter handles requests and inserts new data into the gamesCollection and provides a response.

Which of the games API routes does the front-end application consume (make requests to)?
- POST is the route which the front-end application consumes? Sorry, not sure if I fully understood the question.



**Extensions**

What are we using the MongoDB Driver API for?
- We use mongoDB Driver API because it's non-relational and can handle large collections of objects with different properties and stores this data in JSON docs which are perfect for JS. 

Why do we need to use ObjectId from the MongoDB driver API?
