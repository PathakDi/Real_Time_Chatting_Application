# Node.js Chat App

A simple demo chat app built on [Node.js](https://nodejs.org/), [Express.js](https://expressjs.com/) and [Socket.io](https://socket.io/).

## Demo

https://owan-nodejs-chat-app.herokuapp.com

## Pre-requisites

To setup and run the project for local development / testing, you will need to use Node.js and NPM. I don't explicitly specify a minimum Node.js/NPM version for the app but I recommend going with whatever the latest LTS version is at the point in time you are setting things up. The minimum vesion of Node.js that I have tested this app on is **10.16.3**.

Installers can be found here: [https://nodejs.org/en/download](https://nodejs.org/en/download/)

Another option for installing Node is the **Node Version Manager** (**nvm**), which is a POSIX-compliant bash script to manage multiple active Node.js versions. Instructions for installing and using nvm to install Node and NPM can be found at [https://github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm).

## Installation

The code for the chat app can be found at the public [GitHub](https://github.com/) repo [https://github.com/owanhunte/nodejs-chat-app](https://github.com/owanhunte/nodejs-chat-app). Either clone the repo to a local folder on your machine or download and extract the archive if you don't have [Git](https://git-scm.com/) installed.

Node.js Chat App with Location Sender
A simple demo chat app built using Node.js, Express.js, and Socket.io, with a feature allowing users to share their current location.

Demo
Open a terminal window session and enter the following command to install all necessary Node modules:

## npm install
Run the app in development mode
After running npm install, use the following command to start the app:


## npm run dev
This will start the app and set it up to listen for incoming connections on port 3000. Open your browser and go to http://localhost:3000/ to start using the app. The app will restart automatically on any changes made to the code, thanks to the nodemon script.

Customizing the listening port
To configure the port the app listens on, copy the file .env.example to .env, and set the desired value for the PORT environment variable before starting the app.

Features
Real-time Chat: Users can chat with each other in real time.
Location Sharing: Users can share their current location with others in the chat. This is done using the browser's Geolocation API.
Pre-requisites
To set up and run the project locally, you’ll need to have Node.js and NPM installed. The recommended version is the latest LTS version of Node.js, though the minimum tested version is 10.16.3.

You can download Node.js from https://nodejs.org/en/download, or use Node Version Manager (nvm) to manage multiple Node.js versions.

Installation
Clone the repository or download the code from the GitHub repository:

## git clone https://github.com/owanhunte/nodejs-chat-app
## cd nodejs-chat-app
After cloning the repo, install the dependencies with:

## npm install
Running the App on Multiple Computers
## To make the app accessible over the internet and allow multiple users to connect from different computers, you can use ngrok to create a public URL for your local server.

Steps:
Download and install ngrok from https://ngrok.com/download.

Run the chat app with:

## npm run dev
Start ngrok to tunnel port 3000 (or whichever port you're using):

## ngrok http 3000
Share the ngrok URL with others so they can access the chat app from different machines. The ngrok command will generate a URL like https://<your-subdomain>.ngrok.io. Share this URL with anyone who wants to access the chat app.

## Example:
Forwarding    https://1234abcd.ngrok.io -> http://localhost:3000
You can now share the https://1234abcd.ngrok.io URL with others, and they will be able to access your local server from anywhere.

Enjoy using the app!
