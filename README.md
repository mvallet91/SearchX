# SearchX Docker Image

SearchX consists of two core components: 
* [SearchX-backend](https://github.com/felipemoraes/searchx-backend) to handle the server
* [SearchX-frontend](https://github.com/felipemoraes/searchx-frontend) to take care of user interface, engine configuration, logging (periodically sent to the backend) and task setup

In addition, SearchX takes advantage of several external solutions for different needs:
* Storage is currently based on MongoDB and Redis for caching
*  Websites (documents) are rendered with [Puppeteer-renderer](https://github.com/zenato/puppeteer-renderer), so users remain inside SearchX throughout their session
* [Etherpad-lite](https://github.com/ether/etherpad-lite) is the real-time collaborative document editor for all users to communicate, which also supports live-chat 

## SearchX Architecture Diagram
