# Chat App

We're creating chat app where users can join channels and send messages .

![alt text](https://github.com/yassineoua/node-react-chat/blob/master/docs/chat_app.png)

# Setup

This project require a database installation to complete; however, the knex.ts query builder is configured for a sample Mysql database.

## Setup Backend Instructions

Create a `.env` in the `/backend` directory.

See the `.env.example` file to see what fields are available.

Spin up a local Mysql database or connect to the hosted development database.

Add your database credentials to the `.env` file.

Install NPM Packages. `npm i`

For this project We're using Mysql database, but thanks to Knex you can use other RDSMs :

for that install one of these :

$ npm install pg-native
$ npm install @vscode/sqlite3 # required for sqlite
$ npm install better-sqlite3
$ npm install mysql
$ npm install mysql2
$ npm install oracledb
$ npm install tedious

and set database credentials on your `.env` file.

If using a locally hosted database, migrate and seed.

Migrate the database. `knex migrate:latest --knexfile=knex.ts`.

Run the database seeds. `knex seed:run --knexfile=knex.ts`.

Start the dev server, `npm run watch`.

We're using React, MUI and Socket.io client to handle with chat messages events.

## Setup Frontend Instructions

Create a `.env` in the `/frontend` directory.

See the `.env.example` file to see what fields are available.

Install NPM Packages. `npm i`

Start the dev server, `npm run start`.

# Features

- Persist my chat messages
- I can see the list of all the available channels
- I can receive and send gifs
- Join a channel and see the history of it

# Techs

- [Express](https://expressjs.com/fr/)
- [Knex](https://knexjs.org/)
- [Objection](https://vincit.github.io/objection.js/)
- [Socket.io](https://socket.io/)
- [React](https://en.reactjs.org/)
- [react-scripts](https://www.npmjs.com/package/react-scripts)
- [MUI](https://mui.com/)
