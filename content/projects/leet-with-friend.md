{
"title":"LeetWithFriend",
"link":"https://github.com/MarcusTXK/LeetWithFriend",
"date": "2022-08-01",
"image":"https://user-images.githubusercontent.com/50147457/203652014-86f10774-f472-42f9-bc0c-ea91dbc83a4f.png",
"description":"Led a team of 4 to develop an interview preparation platform and peer matching system, where students can find peers to practice whiteboard-style interview questions together. Developed a real-time matchmaking system between users via web sockets using Socket.IO and Incorporated WebRTC video calls between users in rooms.",
"desciptionImage":"https://user-images.githubusercontent.com/50147457/203652014-86f10774-f472-42f9-bc0c-ea91dbc83a4f.png",
"tags":[
"React",
"Express",
"NodeJS",
"Redis",
"Socket.IO",
"Docker",
"Kubernetes",
],
"featured":true
}

### Description

- An interview preparation platform and peer matching system, where students can find peers to practice whiteboard-style interview questions together.
- To provide a conducive environment for practising interviews, in a room, we have added a Question Pane displaying difficulty and type tags as well as offering forward and backward question navigation. A collaborative editor offering customisable syntax highlighting for multiple popular programming languages and configurable tab sizes for users with different preferences. Video Call functionality is also offered at the bottom right, with toggleable video and audio controls.

![image](https://user-images.githubusercontent.com/50147457/203652120-1d73e89d-b129-4132-aa24-e8dce2ab587e.png)
![image](https://user-images.githubusercontent.com/50147457/203651935-8a8225a3-68f4-458b-8326-de786042fa00.png)

- To accommodate different colour preferences, our frontend will apply the system-preference colour mode initially, and support changing of colour mode (light vs dark) on our navigation bar.
- Our home page includes a Hero Section describing features that our website has to offer them and to encourage users to start a match. Instructions with animations are also included, such as on how to use matching service as well as other features such as keeping track of history.

For more details on design decisions, please check out the report [here](https://drive.google.com/file/d/17dYqfifKffW5hBYldEGQgPU0FoOkhgbe/view?usp=sharing)

### Architecture Overview

![image](https://user-images.githubusercontent.com/50147457/203652611-432dc3b0-b4c3-4c06-a04a-c71627883480.png)

We are using the Microservices architecture, employing a Domain Driven Design to decompose the application into supporting microservices. To identify the services, we decompose by resources – each microservice is responsible for all operations on a given entity in our application. For example, the User Service handles all aspects of managing the user and their account, while the Question Service manages the question bank and individual questions.

To keep dependencies simple and manageable for the ease of development and debugging, we strived to make the services independent of each other and have a one way relationship. The services hence are all able to work with the frontend and have their own database supporting their storage needs. The interactions between the services are minimal as we decided to go for orchestration instead of choreography. The frontend, acting as the entry point of our user interaction, also serves as the service that talks to the rest of the services for information. For example, the frontend contacts the user service to acquire user information, which it relays to the rest of the services when necessary e.g. when the Matching service requires user information to perform matching.

### Overall Technology Stack

| Area                  | Technology                                                                                                                                                |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Frontend              | React<br>TailwindCSS<br>Chakra UI<br>Socket.IO<br>Axios<br>charaka-ui-markdown-renderer<br>PeerJS                                                         |
| Backend               | Express.js, Node.js<br>Mongoose<br>Axios (Communication between microservices)<br>Sequelize<br>Socket.IO<br>Node Scheduler (Timer for matching)<br>PeerJS |
| Database              | PostgreSQL, MongoDB, Redis                                                                                                                                |
| Deployment            | GCP Kubernetes Engine                                                                                                                                     |
| Pub-Sub Messaging     | Socket.io                                                                                                                                                 |
| CI/CD                 | GitHub Actions                                                                                                                                            |
| Tooling               | Eslint, Prettier                                                                                                                                          |
| Orchestration Service | Docker-Compose, Kubernetes                                                                                                                                |
| Project Management    | GitHub Issues & milestones                                                                                                                                |
| Testing               | Jest, Mocha & Chai, Supertest                                                                                                                             |
