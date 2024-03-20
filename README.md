# Youtube-Comments-API

INTRODUCTION

The YOUTUBE COMMENTS API is an application that allows the users to do the following

1. Pull comment associated to a Youtube video by providing the Youtube video id
2. Analyse and categorize each comment in to several setiment categories such as SPAM, POSTIVE, NEGATIVE etc

# Project Setup Instructions

1. clone repo from https://github.com/darkmooink/Youtube-Comments-API.git
2. create a database using PostgreSQL
3. update .env file with your database credentials
4. run npm install at the root of the project folder
5. use http://localhost:3000/youtubecomments/api/v1/ to view landing page
6. use POSTMAN / browser to view categorisation of comments -
   GET - http://localhost:<APPLICATION-PORT>/youtubecomments/api/v1/comments/<VIDEO-ID>/<NUMBER-OF-COMMENTS-TO-BE-RETURNED>?API_KEY=<YOUR-YOUTUBE-API-KEY>
    - sample API key is 9723667a-1fbe-4998-ae25-a832e1f9aae2

## Step 1: Install Dependencies

Run the following command in the root of your project directory:

```bash
npm i
```

This installs all the packages required for the project as defined in the `package.json` file.

## Step 2: Configure Environment Variables

Create three `.env` files based on the `.env.template`:

1. **Development Environment**:

    - Copy `.env.template` to `.env.development`.
    - Configure with values for the development environment.

2. **Test Environment**:

    - Copy `.env.template` to `.env.test`.
    - Set variables for the testing environment.

3. **Live Environment**:

    - Copy `.env.template` to `.env.live`.
    - Fill in variables for the live environment.

These files are crucial for configuring the project in different environments.

## Getting Started

-   Run `npm start` to run in a development enviroment
-   Run `npm test` to run the unit tests
-   Run `npm run live` to run the live enviroment.
