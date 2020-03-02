
### Questions

1. What is responsible for defining the routes of the `games` resource?

const gamesRouter = createRouter(gamesCollection)
  app.use('/api/games', gamesRouter)

2. What do you notice about the folder structure?  Whats the client responsible for? Whats the server responsible for?

client is responsible for front end/ managing the vue files and server is responsible for updating and fetching data from database.

3. What are the the responsibilities of server.js?

setting up the database connection.

4. What are the responsibilities of the `gamesRouter`?

setting up the RESTful routes for accessing and updating the database

5. What process does the the client (front-end) use to communicate with the server?

It uses gameService.js to send GET POST and DELETE requests to the sertver.

6. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs

An init object containing additional instructions for the fetch request including request type (GET, POST, PUT DELETE) and header info.


7. Which of the games API routes does the front-end application consume (i.e. make requests to)?

it makes a GET request to 'http://localhost:3000/api/games/' to get all of the games currently in the database

8. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?

??

## Extension

Why do we need to use [`ObjectId`](https://mongodb.github.io/node-mongodb-native/api-bson-generated/objectid.html) from the MongoDB driver?

Add to your diagram the dataflow for removing a game.
