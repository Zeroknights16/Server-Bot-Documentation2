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
        <li><a href="#general-configuration">General Configuration</a></li>
        <li><a href="#command-usage">Command Usage</a></li>
        <ul>
          <details>
          <summary>Ticket Commands</summary>
            <li><a href="#accept">Accept</a></li>
            <li><a href="#add">Add</a></li>
            <li><a href="#blacklist">Blacklist</a></li>
            <li><a href="#close">Close</a></li>
            <li><a href="#deny">Deny</a></li>
            <li><a href="#move">Move</a></li>
            <li><a href="#new">New</a></li>
            <li><a href="#private">Private</a></li>
            <li><a href="#remove">Remove</a></li>
            <li><a href="#rename">Rename</a></li>
            <li><a href="#ticketpanel">Ticketpanel</a></li>
            <li><a href="#tleaderboard">Tleaderboard</a></li>
            <li><a href="#unblacklist">Unblacklist</a></li>
          </details>
         </ul>
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

> roles.json
```json
"role_name": {String/null}
```
```json
"muted": "965719169406492712"
```
* **ID:** Channel/Role ID of the specific type. **NOTE:** Use ``null`` if the channel/role is not required for your server's specific needs. 

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

If you want to configure the messages the bot sends once a command is executed open file ``lang.yml``.
> lang.yml
```yaml
# Placeholder - ...
<name>:
    title: {String}
    color: {String}
    description: {String}
    timestamp: {Boolean}
```
```yaml
# Placeholder - %ping%
  ping:
    title: ""
    color: "#00FF00"
    description: "``✅`` **Bot Latency:** ``%ping%``ms"
    timestamp: false
```
* **Title:** Title of the embed.
* **Color:** Color of the embed.
* **Description:** Description of the embed
* **Timestamp:** Whether timestamp should be displayed

> If you are unsure how it will looks like refer to [this](https://autocode.com/tools/discord/embed-builder/) website.

### Command Usage
#### Accept
Accept a discord application. The bot will close the application ticket, apply the roles, change nickname, post staff movement, and create a log message including transcript. Fully configurable in file ``config.yml``.
```
/accept <role>
```
![336d750c6d994fb5f6d66b764d3a5a23](https://user-images.githubusercontent.com/73501749/164977490-e104e89e-ef01-466c-a291-f3a8ddb8763c.png)

#### Add
Add an user to a ticket. 
```
/add <User>
```
![7cc96c64f4068ef647d22c64c5c3c570](https://user-images.githubusercontent.com/73501749/164977608-24ba80d7-0fcd-4432-9b62-0f51083b1313.png)

#### Blacklist
Blacklist an user from the ticket system. The user will no longer be able to create a ticket.
```
/blacklist <User> [Reason]
```
![200d3456da52f7b263083ac18d76c699](https://user-images.githubusercontent.com/73501749/164977708-076b6638-d896-420f-b55e-78e5d0273a80.png)

#### Close
Close a ticket. A log message & transcript file will be sent in the configured channel.
```
/close [Reason]
```
![30f551b84f5a57c387ee90270a77744b](https://user-images.githubusercontent.com/73501749/164977780-96ab6cf4-be7b-4e3d-b54a-b7198844bacc.png)

#### Deny
Deny an user's application.
```
/deny [Reason]
```
![7355ce2f3d706a83fba3583a4d8a398d](https://user-images.githubusercontent.com/73501749/164977893-90e6d728-0c70-49c0-bfa5-7cbd28a465c0.png)

#### Move
Move a ticket to a different ticket category. 
```
/move <Category>
```
![09b0b344308573799e62d1245d46090b](https://user-images.githubusercontent.com/73501749/164977960-07b84168-ae57-4be5-a5c8-ff8575a60725.png)

#### New
Tags the ticketpanel channel.
```
/new
```

#### Private
Sets the ticket to srstaff/management only. 
```
/private [srstaff/management/undo]
```
![a14067f797ae1c177033d69aa2b9d927](https://user-images.githubusercontent.com/73501749/164978025-08426300-9fdc-4204-961a-a4bbd2a4002b.png)

#### Remove
Remove an user from the ticket.
```
/remove <User>
```
![a1d0bac609468819a5c494906998a6cb](https://user-images.githubusercontent.com/73501749/164978053-8344a96c-df1c-4a00-9ead-028539158106.png)

#### Rename
Rename a ticket.
```
/rename <Name>
```
![497b0acf1fdabe816a3cd40f1b6f6b8b](https://user-images.githubusercontent.com/73501749/164978084-98e4e41f-8828-4535-af04-8bd74618cb5d.png)

#### Ticketpanel
Sends the ticketpanel. Fully configurable.
```
/ticketpanel
```
![c9c1e6565675ef115fd1c4488bce775e](https://user-images.githubusercontent.com/73501749/164978109-3715a7f2-2fd2-4ff3-9b99-27185cd5650d.png)

#### Tleaderboard
Displays leaderboard of closed & opened tickets.
```
/tleaderboard <closed/opened>
```
![077eb40839b968e522ee5f300bb4b2ee](https://user-images.githubusercontent.com/73501749/164978193-a83d18d7-5ca7-4c58-a5f1-d4d786d9eed3.png)

#### Unblacklist
Unblacklist an user from the ticket system. He will be able to create tickets again.
```
/unblacklist <User> [Reason]
```
![88f7692c4c7789b7ea2cb252b992af35](https://user-images.githubusercontent.com/73501749/164978285-07f3aec3-5370-41bb-8858-c4331d421ce5.png)





## Features

## Config.yml

## Developer API

## Errors
