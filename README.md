# Social Network API

Welcome to the Social Network API, a robust solution for handling large amounts of unstructured data in a social media web application. This API is built using Express.js for routing, MongoDB as the NoSQL database, and Mongoose ODM for seamless interaction with the database.

## Table of Contents

- [Installation](#installation)
- [Video](#Video)
- [Image](#Image)
- [Usage](#usage)
- [Walkthrough Video](#walkthrough-video)
- [API Routes](#api-routes)
  - [Users](#users)
  - [Thoughts](#thoughts)
- [Acceptance Criteria](#acceptance-criteria)
- [License](#license)

## Installation

To get started with the Social Network API, follow these steps:

1. Clone the repository to your local machine.
2. Run `npm install` to install the necessary dependencies.
3. Configure your MongoDB connection in the `config.js` file.
4. Run `npm start` to start the server and sync Mongoose models with the MongoDB database.

## Video 

[Link to Walkthrough Video](https://drive.google.com/file/d/1hkS-uDV1HIhxLqDpX_flNu7XmcAk0Spj/view)

## Image 
![Alt text](<images/Screenshot 2023-11-22 182203.png>)

## Usage

Once the server is running, you can use Insomnia or any API testing tool to interact with the available routes. Refer to the API Routes section for details on the available endpoints.

## Walkthrough Video

[Link to Walkthrough Video](#) - Insert the link to your walkthrough video here.

Please watch the video to see the functionality of the Social Network API and ensure that all acceptance criteria are met.

## API Routes

### Users

- **GET /api/users**: Retrieve a list of users in a formatted JSON.

- **POST /api/users**: Create a new user.

- **PUT /api/users/:userId**: Update user information.

- **DELETE /api/users/:userId**: Delete a user.

### Thoughts

- **GET /api/thoughts**: Retrieve a list of thoughts in a formatted JSON.

- **POST /api/thoughts**: Create a new thought.

- **PUT /api/thoughts/:thoughtId**: Update thought information.

- **DELETE /api/thoughts/:thoughtId**: Delete a thought.

- **POST /api/thoughts/:thoughtId/reactions**: Add a reaction to a thought.

- **DELETE /api/thoughts/:thoughtId/reactions/:reactionId**: Remove a reaction from a thought.

- **POST /api/users/:userId/friends/:friendId**: Add a friend to a user's friend list.

- **DELETE /api/users/:userId/friends/:friendId**: Remove a friend from a user's friend list.

## Acceptance Criteria

1. When the command to invoke the application is entered, the server starts, and Mongoose models are synced to the MongoDB database.
2. When API GET routes for users and thoughts are tested in Insomnia, the data for each route is displayed in a formatted JSON.
3. When API POST, PUT, and DELETE routes for users and thoughts are tested in Insomnia, users and thoughts can be successfully created, updated, and deleted in the database.
4. When API POST and DELETE routes for reactions and friends are tested in Insomnia, reactions can be successfully created and deleted for thoughts, and friends can be added and removed from a user's friend list.


## License

This project is licensed under the [MIT License](LICENSE).