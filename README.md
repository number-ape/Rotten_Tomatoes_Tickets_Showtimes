## What is it?
- Tickets & Showtimes module for a Rotten Tomatoes clone project.
- It allows user to see movie showtimes of the day in a close-by theater and update location.

## Demo
[movie showtimes demo](https://youtu.be/vk07sRRm01M)

## Getting Started
### Prerequisite
- Install PostgreSQL:
https://www.postgresql.org/download/macosx/
- Start a PSQL server
```postgres -D /usr/local/var/postgres```
- In a new window, create database rottentomatoes
```createdb rottentomatoes```
- Use the rottentomatoes database
```psql -s rottentomatoes```
- Copy code in schema.sql and paste into the database command line to create tables and schemas
### Installing
- ```npm install```
### Seed demo data
- ```npm run seed-all```, or
- seed individual tables: ```node_modules/.bin/sequelize db:seed --seed [seed file name, e.g. 20190202201451-demo-movie.js]```
### Build
- Dev: ```npm run dev```
- Production: ```npm run build```
### Start Local Server
- ```npm start```
### Test
- Run Jest tests: ```npm run test```

## Tech Choices
Client
- Vue
- Bootstrap
- Bootstrap-Vue
- CSS
	
Server
- Node
- Express

Database
- PostgreSQL
- Sequelize

Testing
- Jest
- Vue-Test-Utils

## Acknowledgements
- This is a group project that I completed with bernardlau and chrisweilacker at Hack Reactor.
- Each member creates one service module
- A proxy server communicates with all service modules to fetch information for the main movie

## Related Projects
- Proxy Server: https://github.com/number-ape/rotten_pomodoro_proxy_chen
- Scoreboard (chrisweilacker): https://github.com/number-ape/Rotten_Tomatoes_Scoreboard_Service
- Audience Review (bernardlau): https://github.com/number-ape/Rotten_Tomatoes_Reviews_Service




