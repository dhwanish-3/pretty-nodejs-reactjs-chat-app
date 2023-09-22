# pretty-nodejs-reactjs-chat-app

Get detailed documentation at [Build Pretty Chat App](https://blog.chatengine.io/fullstack-chat/nodejs-reactjs).
If you are really confident in yourself then go ahead, I am not stopping you.

## NodeJS Server Setup

Go to [Chat Engine](https://chatengine.io) to set up your own chat server.

- Click "New Project" and follow the steps
- Your `Project ID` and `Private Key` will be required copy them

Inside the project folder
```
mkdir backend
cd backend
npm init -y
npm install express axios cors
npm install --save-dev nodemon
# Add: "scripts": { "start": "nodemon index.js" },
echo node_modules/ > .gitignore
npm run start
```

In `.env` write:

```
PRIVATE_KEY=`Private Key`
```


## Connect React to Chat Engine!

This simple repo shows how to easily add chat functionality into a React project with [Chat Engine](https://chatengine.io).

To understand the code, please watch [this video]()!

### Setup Steps

Set up this chat client in the 3 steps below.

These steps assume you have already set up one of the server projects in `../backend`.

#### 1 - Setup a Chat Engine server

Go to [Chat Engine](https://chatengine.io) to set up your own chat server.

- Click "New Project" and follow the steps
- Your `Project ID` and `Private Key` will be required for step 2

#### 2 - Connect `.env` to Chat Engine

We will connect to your Chat Engine server with environment variables.

This allows you to connect to different chat servers in local vs. staging vs. production.

Replace the UUID below with your own. In `.env.local` write:

```
REACT_APP_CHAT_ENGINE_PROJECT_ID=`Project ID`
```

#### 3 - Install & Start

Run the following two lines of code in `frontend/`.

```
npm install
npm run start
```

Done! Your Express server is on `localhost:3000` and connected to Chat Engine!

All new "Sign Up" users are on Chat Engine, and their credentials are found upon "Login".

To understand the code, please watch [this video]()!
