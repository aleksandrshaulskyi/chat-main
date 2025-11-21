# Chat index repository.

## Disclaimer.
This application is currently in active development state. Most of it's bugs and imperfections are probably very well known.
They will be fixed in the very close future.

For the sake of convinience in the development process at this very moment database containers are placed next to the respectful microservices.

## Purpose.
This is the index repository or meta repository for my chat system that contain various microservices.
This repository links all the other repositories together and keeps track of the most recent updates.

## Links.

Authentication microservice: https://github.com/aleksandrshaulskyi/chat-auth
Transportation microservice: https://github.com/aleksandrshaulskyi/chat-transportation
Messaging microservice: https://github.com/aleksandrshaulskyi/chat-messaging
Shared services: https://github.com/aleksandrshaulskyi/chat-shared-services

## Test it yourself.
1. Clone all the repositories that are linked to this repository.
2. Switch to the directory that contains the **chat-shared-services** repository content.
3. Run ```docker-compose up -d```.
4. Switch to the directory that contains the **chat-auth** repository content.
5. Run ```docker-compose up -d --build``` to start the auth microservice.
6. Switch to the directory that contains the **chat-transportation** repository content.
7. Run ```docker-compose up -d --build``` to start the transportation microservice.
8. 2. Switch to the directory that contains the **chat-messaging** repository content.
9. Run ```docker-compose up -d --build``` to start the messaging microservice.

The application should be accessible on the **http://localhost:80/**

## Recent updates.

Not yet released.
