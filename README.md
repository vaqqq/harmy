[![harmy](https://harmy.gg/HarmySVGREADME.svg)](https://harmy.gg/)
# Discord presence, activities and other integrations RESTful API, ready for use in under 10 seconds.

## Introduction
Our Presence API is a RESTful API that allows you to access to your live Discord presence via an API endpoint: `(api.harmy.gg/user/:user_ID)` - example: you can use it for displaying your online status (online, idle, dnd, offline) or what you are listening to on Spotify on your own website.  There is a GitHub connection option which you can enable using our Discord bot for displaying your account information, such as public repositories, URL, bio and more.

We also give you the possibility to store your own K/V (key/value), which you can create and manage through our Discord bot.

## Get started with 1 click
Join our [Discord server](https://discord.gg/asyWxPudkQ) and you are good to go and able to request your Discord user data. Simple is that.

## Docs
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

# Spotlight [![harmy](https://harmy.gg/APISVG.svg)](https://harmy.gg/)
Here are a few websites that use harmy:

- [harmonybot.ch](https://harmonybot.ch/home)
