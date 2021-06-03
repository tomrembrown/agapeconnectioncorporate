# agapeconnectioncorporate

A simple website to act as a splash page for the Agape Connection company. It also describes the company's goals, mission, and vision.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Installing

1. Ensure node nd yarn are installed. Since lerna is built on yarn, this uses yarn as the package manager. Node must be at least version 14. This project is just static pages with a contact page - so it does not contain any database.

2. Clone GIT repository and download

```
git clone https://github.com/tomrembrown/allisone
cd allisone
```

3. Download and install packages in various directories, and copy files to create .env - which can be done with the following command

```
yarn initial
```

4. Adjust parameters in .env as necessary (note .env files exist both client and server)

5. a) Development - For development mode, start the servers (command from root directory starts both react & express servers).

```
yarn run dev
```

5. b) Production - For production mode, first build the bundles

```
yarn run build
```

Second, for production, on the server, run the server using pm2 (process manager) using:

```
yarn run server
```

## Running the tests

Tests are not currently configured

### What the tests do

These tests handle linting with jshint, link checking, and some cross-page and unit tests.

## Built With

- [Node.JS](https://nodejs.org/) - JavaScript runtime that allows server-side JavaScript
- [Express](https://expressjs.com/) - Backend framework
- [Vue.js](https://v3.vuejs.org/) - Frontend framework

## Contributing

Please ask Tom Brown (tombrown654321@protonmail.com) if you would like to contribute to this project.

## Authors

- **Tom Brown**

## License

This project is using the MIT license - see the [LICENSE](LICENSE) file for details
