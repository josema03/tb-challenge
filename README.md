# TOOLBOX CHALLLENGE TEST APP

## How to clone the repo

1. Clone the repo with the following command:

```
$ git clone https://github.com/josema03/tb-challenge --recursive
```

The `--recursive` flag above is **very important**, otherwise the app won't start.

2. Make sure submodules are up to date with the command below:

```
$ git submodule update --recursive
```

## How to start the app with Docker

If you don't have docker installed in your computer you can get it at [their official webpage](https://docs.docker.com/get-docker/) and follow the instructions.

After cloning the repo and its submodules, at the root folder just run the following command:

```
$ docker compose up
```

This should start the app locally and you should be able to see it by visiting `http://localhost:3000` in your browser

## How to start the app without Docker

Before following any other steps inside the subfolders, you have to install all the dependencies. This can be done by running `npm install` or `yarn` at the project root folder or at each of the subfolders.

### How to start tb-react-app

1. From the root folder, navigate to the `tb-react-app` folder

```
$ cd tb-react-app
```

2. Run the command below:

```
$ npm run start
```

3. The app should start running on port 3000

### How to start tb-express-server

1. From the root folder, navigate to the `tb-express-server` folder

```
$ cd tb-express-server
```

2. Run the command below:

```
$ npm run start
```

3. The app should start running on port 8080

## How to test

### How to start tb-react-app

#### Option 1

Run the following command from the project root folder:

```
$ npm run test --workspace=tb-react-app
```

#### Option 2

1. From the root folder, navigate to the `tb-react-app` folder

```
$ cd tb-react-app
```

3. Run the command below:

```
$ npm run test
```

3. Tests should start running

### How to start tb-express-server

#### Option 1

Run the following command from the project root folder:

```
$ npm run test --workspace=tb-express-server
```

#### Option 2

1. From the root folder, navigate to the `tb-express-server` folder

```
$ cd tb-express-server
```

3. Run the command below:

```
$ npm run test
```

3. Tests should start running
