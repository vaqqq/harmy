[![harmy](https://harmy.gg/HarmySVGREADME.svg)](https://harmy.gg/)
# Discord presence, activities and other integrations RESTful API, ready for use in under 10 seconds.

## Introduction
Our Presence API is a RESTful API that allows you to access to your live Discord presence via an API endpoint: `(api.harmy.gg/user/:user_ID)` - example: you can use it for displaying your online status (online, idle, dnd, offline) or what you are listening to on Spotify on your own website.  There is a GitHub connection option which you can enable using our Discord bot for displaying your account information, such as public repositories, URL, bio and more.

We also give you the possibility to store your own K/V (key/value), which you can create and manage through our Discord bot.

## Get started with 1 click
Join our [Discord server](https://discord.gg/asyWxPudkQ) and you are good to go and able to request your Discord user data. Simple is that.

## Table of Contents
- [API Docs](https://github.com/vaqqq/harmy/tree/main?tab=readme-ov-file#api-docs)
    - [K/V](https://github.com/vaqqq/harmy/tree/main?tab=readme-ov-file#kv)
        - [What is a K/V system?](https://github.com/vaqqq/harmy/edit/main/README.md#what-is-a-kv-system)
        - [Create a K/V pair](https://github.com/vaqqq/harmy/edit/main/README.md#create-a-keyvalue-pair)
        - [Access through the API](https://github.com/vaqqq/harmy/edit/main/README.md#access-through-the-api)
- [Authorization](https://github.com/vaqqq/harmy/edit/main/README.md#authorization)
    - [Get the API Token](https://github.com/vaqqq/harmy/edit/main/README.md#get-the-api-token)
    - [Hashed Tokens](https://github.com/vaqqq/harmy/edit/main/README.md#hashed-tokens)
- [Spotlight](https://github.com/vaqqq/harmy/edit/main/README.md#spotlight-)

## API Docs
Get a user’s Discord presence data.

`GET` - https://api.harmy.gg/user/:user_ID

Example response:
```json
{
    "presence": {
        "userId": "470320681905684500",
        "status": "dnd",
        "global_name": "Vaq",
        "server_name": null,
        "avatar": "5c11d7292c91e510c2b4f07946ea6d72",
        "spotifyActivity": null
    },
    "KV": {
        "hi": "no",
        "another": "one",
        "hello": "fresh",
        "idk": "what to say"
    },
    "github": {
        "id": 111227553,
        "username": "vaqqq",
        "avatar_url": "https://avatars.githubusercontent.com/u/111227553?v=4",
        "url": "https://github.com/vaqqq",
        "company": null,
        "blog": "https://harmy.gg",
        "bio": "casual coder",
        "public_repos": 1
    }
}
```

## K/V

### What is a K/V system?
The Key/Value system allows users to store and retriev their own data associated with their user profiles. Example: You could use it for storing user preferences, settings, or any other custom data relevant to the user's profile, like the user's location or email.

### Create a key/value pair
The only thing you have to do is to run the `.add <key> <value>` command of our Discord bot for creating a new key/value pair.

### Access through the API
Use your API token as an authentification method to access your custom data.

## Authorization

### Get the API token
Run the `.token` command in our Discord server. You will receive a DM from our Discord bot, including the API Token.

*Note: If you think that your token has been compromised, you can simply just re-run the command for resetting your API token.*

### Hashed Tokens
Your API token will be hashed using a secure hashing algorithm. This means even in the unlikely event of a data breach, your tokens cannot be easily read or misused. - Your data is safe.

# Spotlight [![harmy](https://harmy.gg/APISVG.svg)](https://harmy.gg/)
Here are a few websites that use harmy:

- [harmonybot.ch](https://harmonybot.ch/home)
