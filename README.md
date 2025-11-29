# Chat index repository.

This is my main demo project that is used for the representation of my skills.

## Disclaimer.
This application is currently in active development state. Most of it's bugs and imperfections are probably very well known.
They will be fixed in the very close future.

For the sake of convinience in the development process at this very moment database containers are placed next to the respectful microservices.

## Purpose.
This is the index repository or meta repository for my chat system that contain various microservices.
This repository links all the other repositories together and keeps track of the most recent updates.

## Repositories of the project.

Authentication microservice: https://github.com/aleksandrshaulskyi/chat-auth  
Transportation microservice: https://github.com/aleksandrshaulskyi/chat-transportation  
Messaging microservice: https://github.com/aleksandrshaulskyi/chat-messaging  
Shared services: https://github.com/aleksandrshaulskyi/chat-shared-services  
React/Typescript service: https://github.com/aleksandrshaulskyi/chat-frontend  
Monitoring microservice: https://github.com/aleksandrshaulskyi/chat-monitoring  
Logging microservice: https://github.com/aleksandrshaulskyi/chat-logging  

## Test it yourself.
1. Clone all the repositories that are linked to this repository.
2. Switch to the directory that contains the **chat-shared-services** repository content.
3. Run ```docker-compose up -d --build```.
4. Repeat the step 3 for every repo of this project.

The application should be accessible on the **http://localhost:80/**

## Recent updates.

Not yet released.
