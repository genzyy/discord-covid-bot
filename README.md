<h1 align="center">discord-covid-bot</h1>

## Requirements

- A Discord account
- Access to [this](https://discord.com/developers/applications)
- Will to learn

## What we are gonna use for this bot

- An API is needed so that the data can be fetched for all the countries and the API we are using is [covid19api](https://covid19api.com/) which helps us to get the
data
- We will create a JSON file to keep names of all countries avaialable so that we can retrieve the data from the API we are using.
- The data we store into the JSON file needs to be read and accessed acccurately and in the minimum time possible so we need to format the JSON file in that way.
- We make a get request to the API whenever the command is sent to the bot in order to retrieve the data.

## How to setup

Firstly, go to the discord developer portal and make a bot and give it the administrator ability. For a very explained steps check [this](https://discordpy.readthedocs.io/en/latest/discord.html), but when you reach the 6th step in Inviting your bot section, instead of the mentioned permissions, select `Administrator`.

Now, since we have created the bot locally and we need to integrate it into a discord server( for which you have to have the administrator permissions for that server), go the [discord-permissions](https://discordapi.com/permissions.html), and there paste your client id you get in the applications tab of the discord developer portal and then it will create a link to add the bot to your preferred discord server.

Then, you need to have nodejs and npm installed on your system natively. If you have them then no worries and if not, you can install them from their webistes or if
you are working on a linux system, you can install these with the available package manager.

Now if you are cloning this repository, then go to the repository folder and then run `npm install`. This command will install all the necessary packages automatically.
And if you want to make the bot yourself, then run this into your work folder,
```bash
  npm install discord.js axios --save
```

After this to run the bot locally, just run this in the terminal,
```bash
  node index.js
```
## Available Commands

The available command is `!cases country-name` which will give you confirmed cases, deaths and recovered cases from covid of that country.


## Adding bot to your discord server

Follow this link: https://discord.com/oauth2/authorize?client_id=748926086741491712&scope=bot&permissions=0
You must be logged into the discord web app and you have to have administrative permissions of the server you are trying to add the bot to.
