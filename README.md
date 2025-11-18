# Chat index repository.

## Disclaimer.
This application is currently in active development state. Most of it's bugs and imperfections are probably very well known.
They will be fixed in the very close future.

## Purpose.
This is the index repository or meta repository for my chat system that contain various microservices.
This repository links all the other repositories together and keeps track of the most recent updates.

## Test it yourself.
1. Clone all the repositories that are linked to this repository.
2. Switch to the directory that contains the **chat-shared-services** repository content.
3. Run ```docker-compose up -d rabbitmq``` to start the broker.
4. Switch to the directory that contains the **chat-auth** repository content.
5. Run ```docker-compose up -d --build``` to start the auth microservice.
6. Switch to the directory that contains the **chat-transportation** repository content.
7. Run ```docker-compose up -d --build``` to start the transportation microservice.
8. 2. Switch to the directory that contains the **chat-messaging** repository content.
9. Run ```docker-compose up -d --build``` to start the messaging microservice.
10. Finally switch back to the directory that contains the **chat-shared-services** repository content.
11. Run ```docker-compose up -d --build``` to start the rest of shared services such as Redis and Nginx.

The application should be accessible on the **http://localhost:80/**
