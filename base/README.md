# SearchX on Docker
This is a multi-container Docker application, [Docker Desktop](https://www.docker.com/products/docker-desktop) is required to run this version of SearchX.

SearchX consists of two core components: 
* [SearchX-backend](https://github.com/felipemoraes/searchx-backend) to handle the server
* [SearchX-frontend](https://github.com/felipemoraes/searchx-frontend) to take care of user interface, engine configuration, logging (periodically sent to the backend) and specific task setup

In addition, SearchX takes advantage of several external solutions for different needs:
* Storage is currently based on MongoDB and Redis for caching
* Websites (documents) are rendered with [Puppeteer-renderer](https://github.com/zenato/puppeteer-renderer), so users remain inside SearchX throughout their session
* [Etherpad-lite](https://github.com/ether/etherpad-lite) is the real-time collaborative document editor for all users to communicate, which also supports live-chat 

## SearchX Architecture Diagram (TBD)

## Configuration
The environment (ENV) variables for each container can be defined in the `docker-compose.yml` file, such as the BING_API_KEY. 

## Instructions
First Time:
1. Download (or clone) this repository, and unzip the files. 
2. Open a terminal and go to the folder location
3. Run the following command: `docker-compose up --build` (don't close this terminal)
4. This will retrieve the necessary images for Mongo, Redis, Puppeteer, Etherpad, Backend and Frontend; and build the containers
5. You can open the application in your browser in `localhost:8080`
6. To close the application, press `Ctrl+C` on the terminal

The process to re-open the application with the stored data is very similar:
1. Open a terminal and go to the folder location
2. Run the following command: `docker-compose up` (don't close this terminal)
3. Docker will start the pre-built containers
4. You can open the application in your browser in `localhost:8080`
5. To close the application, press `Ctrl+C` on the terminal
