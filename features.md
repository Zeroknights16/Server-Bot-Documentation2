<div id="top"></div>

<br />
<div align="center">
  <a href="https://github.com/Zeroknights16/Server-Bot-Documentation2/blob/main/features.md">
    <img src="images/e9290f3ece1ec3239eb2c32b74675a25.webp" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Server Bot v2 | Documentation</h3>

  <p align="center">
    An awesome Discord Bot for your Faction, Skyblock & Prison server!
    <br />
    <a href="https://discord.gg/tsG2ZJW9"></strong></a>
    <br />
    <a href="https://github.com/Zeroknights16/Server-Bot-Documentation2/blob/main/features.md">Docs</a>
    ·
    <a href="https://discord.gg/tsG2ZJW9">Report Bug</a>
    ·
    <a href="https://discord.gg/tsG2ZJW9">Request Feature</a>
  </p>
</div>


<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#commands">Commands</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#features">Features</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#developer-api">Developer API</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
  </ol>
</details>


## Commands
The bot currently offers more than **80** commands which are all configurable. This section of the server bot's documentation will go through the general configuration first. After the general configuration the doc will go through each command and its specialties.

### General Configuration
> commands.json
```json
"command_name": {
    "enabled": {Boolean},
    "permission": {String},
    "cooldown": {Integer}
},
```
```json
"accept": {
    "enabled": true,
    "permission": "965719153833041920",
    "cooldown": 2
},
```
* **Enabled:** Whether the command should be loaded
* **Permission:** The role which is required to be able to execute the command. __NOTE:__ You do not have to inherit the role itself to be able to execute the command. The bot will check if the user inherits the configured role or one **above**.
* **Cooldown:** Cooldown of the command in seconds. **NOTE:** ``{Integer}`` >= 3, otherwise it will set the cooldown to the default value 3.

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

Sometimes the command requires a specific channel and/or role to work. In this case open file ``channels.json`` and/or ``roles.json``.
> channels.json
```json
"channel_name": {String/null}
```
```json
"server_stats": "965719204319875082"
```

## Features

## Developer API

## Errors
