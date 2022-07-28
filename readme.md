# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

Get [Docker](https://docker.com) & [Docker Compose](https://https://docs.docker.com/compose/)
Once you have ensured you have Docker & Compose and all related necessary libraries installed;
From the root of the project dir run;
docker-compose up    # Go grab a coffee because this part takes awhile

After docker-compose finishes PUMA webserver will be waiting on localhost. Check that everything worked by hitting this route;
http://localhost:3000/api/ping

Rails will first tell you their are pending migrations. Hit the button and run the migrations. The site will shortly load thereafter. 

Congrats! We have our backend up! Let's check our frontend and make sure it's connected to the backend. Try to hit this route and create any test user;
http://localhost:3001/register

If that works, way to go! Everything is setup correctly. Happy hacking!