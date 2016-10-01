# lambda-es2015-twitter-bot

This is an example to create an AWS Lambda application with Babel-based ES2015. This application simply tweet the current weather (Tokyo).

## Installation

    git clone https://github.com/hkusu/lambda-es2015-twitter-bot
    npm install

Get the keys of your twitter application in [https://apps.twitter.com](https://apps.twitter.com).

> Permission, please choose `Read and Write`.

Set the keys to the `.env` file.

    CONSUMER_KEY = your consumer key
    CONSUMER_SECRET = your consumer secret
    ACCESS_TOKEN = your access token
    ACCESS_TOKEN_SECRET = your access token secret

## Usage

### check the syntax of source code

    npm run lint

### monitoring and automated build of source code

    npm run watch

### run the application in the local environment

    npm run localRun

### create an archive

    npm run build

Upload the created app.zip in the console of the AWS Lambda.

![screen shot](./screenshot1.png)

## Settings in the AWS lambda

![screen shot](./screenshot2.png)

> Role, does not require special permissions.

Triggers, select the `CloudWatch Events(Schedule)`.
