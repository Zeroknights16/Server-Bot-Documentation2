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
          <details>
          <summary>General Commands</summary>
            <li><a href="#av">Av</a></li>
            <li><a href="#botinfo">Botinfo</a></li>
            <li><a href="#help">Help</a></li>
            <li><a href="#info">Info</a></li>
            <li><a href="#invites">Invites</a></li>
            <li><a href="#invitetop">Invitetop</a></li>
            <li><a href="#ip">Ip</a></li>
            <li><a href="#ping">Ping</a></li>
            <li><a href="#server">Server</a></li>
            <li><a href="#suggest">Suggest</a></li>
            <li><a href="#uptime">Uptime</a></li>
            <li><a href="#vanity">Vanity</a></li>
          </details>
          <details>
          <summary>Fun Commands</summary>
            <li><a href="#ac">Ac</a></li>
            <li><a href="#ask">Ask</a></li>
            <li><a href="#bird">Bird</a></li>
            <li><a href="#dicksize">Dicksize</a></li>
            <li><a href="#dog">Dog</a></li>
            <li><a href="#fact">Fact</a></li>
            <li><a href="#iq">Iq</a></li>
            <li><a href="#meme">Meme</a></li>
            <li><a href="#nuke">Nuke</a></li>
            <li><a href="#roll">Roll</a></li>
            <li><a href="#rps">Rps</a></li>
          </details>
          <details>
          <summary>Moderation Commands</summary>
            <li><a href="#ban">Ban</a></li>
            <li><a href="#dm">Dm</a></li>
            <li><a href="#kick">Kick</a></li>
            <li><a href="#lock">Lock</a></li>
            <li><a href="#mute">Mute</a></li>
            <li><a href="#purge">Purge</a></li>
            <li><a href="#slowmode">Slowmode</a></li>
            <li><a href="#tempban">Tempban</a></li>
            <li><a href="#tempmute">Tempmute</a></li>
            <li><a href="#unban">Unban</a></li>
            <li><a href="#unlock">Unlock</a></li>
            <li><a href="#unmute">Unmute</a></li>
            <li><a href="#unwarn">Unwarn</a></li>
            <li><a href="#warn">Warn</a></li>
            <li><a href="#warnhistory">Warnhistory</a></li>
          </details>
          <details>
          <summary>Management Commands</summary>
            <li><a href="#approve">Approve</a></li>
            <li><a href="#booster">Booster</a></li>
            <li><a href="#bundle">Bundle</a></li>
            <li><a href="#changelog">Changelog</a></li>
            <li><a href="#clearbundle">Clearbundle</a></li>
            <li><a href="#clearstrike">Clearstrike</a></li>
            <li><a href="#dbcreate">Dbcreate</a></li>
            <li><a href="#demote">Demote</a></li>
            <li><a href="#embed">Embed</a></li>
            <li><a href="#gcreate">Gcreate</a></li>
            <li><a href="#gend">Gend</a></li>
            <li><a href="#greroll">Greroll</a></li>
            <li><a href="#leader">Leader</a></li>
            <li><a href="#lockdown">Lockdown</a></li>
            <li><a href="#lookup">Lookup</a></li>
            <li><a href="#playingadd">Playingadd</a></li>
            <li><a href="#playingclear">Playingclear</a></li>
            <li><a href="#playinglist">Playinglist</a></li>
            <li><a href="#playingremove">Playingremove</a></li>
            <li><a href="#promote">Promote</a></li>
            <li><a href="#reactionpanel">Reactionpanel</a></li>
            <li><a href="#reload">Reload</a></li>
            <li><a href="#resign">Resign</a></li>
            <li><a href="#restart">Restart</a></li>
            <li><a href="#sdeny">Sdeny</a></li>
            <li><a href="#sendmsg">Sendmsg</a></li>
            <li><a href="#setup">Setup</a></li>
            <li><a href="#strike">Strike</a></li>
            <li><a href="#strikeset">Strikeset</a></li>
            <li><a href="#verifypanel">Verifypanel</a></li>
          </details>
         </ul>
      </ul>
    </li>
    <li>
      <a href="#features">Features</a>
      <ul>
        <li><a href="#db-cleanup">DB Cleanup</a></li>
        <li><a href="#event-logs">Event Logs</a></li>
        <li><a href="#alt-detection">Alt Detection</a></li>
        <li><a href="#application">Application</a></li>
        <li><a href="#auto-moderation">Auto Moderation</a></li>
        <li><a href="#welcome">Welcome</a></li>
      </ul>
    </li>
    <li>
      <a href="#developer-api">Developer API</a>
      <ul>
        <li><a href="#commands-1">Commands</a></li>
        <li><a href="#managers">Managers</a></li>
      </ul>
    </li>
    <li>
      <a href="#errors">Errors</a>
      <ul>
        <li><a href="#discord-api-error">Discord API Error</a></li>
        <li><a href="#bot-error">Bot Error</a></li>
        <li><a href="#console-error">Console Error</a></li>
      </ul>
    </li>
    <li>
      <a href="#note">Note</a>
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
> Ticket commands
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

> __________________________

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

> General commands
#### Av
Displays an user's avatar.
```
/av [User]
```

#### Botinfo
Displays information about the bot.
```
/botinfo
```

#### Help
Displays help page for commands.
```
/help
```
![d3fdc13e864ac57fcad2c563ed2b3e82](https://user-images.githubusercontent.com/73501749/164979448-aeb63419-08db-4d9c-b764-cdc6ca3887cb.png)

#### Info
Displays information about a certain user.
```
/info [User]
```
![f5903ce48318adba7144c9e445efe633](https://user-images.githubusercontent.com/73501749/164979492-bcb3e457-b100-4c20-bb20-371f2d48fab0.png)

#### Invites
Displays an user's invites.
```
/invites [User]
```

#### Invitetop
Displays top inviter leaderboard.
```
/invitetop
```

#### Ip
Displays server's ip.
```
/ip
```

#### Ping
Displays the bot's latency.
```
/ping
```

#### Server
Displays information about the guild.
```
/server
```
![e1b9f3f1c97ede2c7a436e6d8dac4bf1](https://user-images.githubusercontent.com/73501749/164979616-230aef9b-b770-43ad-ab1e-2eab05f3aa1c.png)

#### Suggest
Submit a suggestion.
```
/suggest <Suggestion>
```
![3b2ba311ec3a62d0593a1728c3bc1586](https://user-images.githubusercontent.com/73501749/164979650-fb7c2dca-44fa-490e-b8a4-3c91ed5528e5.png)

#### Uptime
Displays the bot's uptime.
```
/uptime
```

#### Vanity
Displays information about the ``vanity_url`` discord feature.
```
/vanity
```

> __________________________

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

> Fun commands
#### Ac
Activity Check!
```
/ac <User>
```

#### Ask
Get a random answer of the bot.
```
/ask <Question>
```

#### Bird
Displays a random bird picture.
```
/bird
```

#### Dicksize
Displays an user's dicksize.
```
/dicksize [User]
```

#### Dog
Displays a random dog picture.
```
/dog
```

#### Fact
Random fun fact.
```
/fact
```

#### Iq
IQ Test?!
```
/iq
```

#### Meme
Random meme.
```
/meme
```

#### Nuke
Nuke the whole server??
```
/nuke
```

#### Roll
Roll a dice.
```
/roll
```

#### Rps
Rock, Paper, Scissors.
```
/rps
```
![d4e83141b5c9eec20beb8263478f9e19](https://user-images.githubusercontent.com/73501749/164980067-e0dbd468-1f75-456f-b195-8f6fe5383827.png)

> __________________________

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

> Moderation commands
#### Ban
Ban an user from the guild permanently.
```
/ban <User> [Reason]
```
![575af96113cdcc9f47943d48c90e40e8](https://user-images.githubusercontent.com/73501749/164980416-503f2d76-a680-45fe-869d-85ac248dff9a.png)

#### Dm
Dm an user from the guild.
```
/dm <User> <Message>
```

#### Kick
Kick an user from the guild
```
/kick <User> [Reason]
```
![224615f33768e9ebd7154f937efa828a](https://user-images.githubusercontent.com/73501749/164980465-1d2faf13-d978-4803-9166-1ec1c19eca84.png)

#### Lock
Lock a channel.
```
/lock <Channel>
```
![a95e1d6fb7840e3645c27faa65fdb4b0](https://user-images.githubusercontent.com/73501749/164980492-345ae086-532e-46d0-9c88-f5faf9f30cab.png)

#### Mute
Prevent an user of sending messages in the guild permanently. 
```
/mute <User> [Reason]
```
![9a9a4455c09bcd59c509bba4afd7f555](https://user-images.githubusercontent.com/73501749/164980551-7f8d053e-b42c-4dd5-9b05-ff415dc9de72.png)

#### Purge
Clear a specific amount of messages in certain channels
```
/purge <Amount>
```

#### Slowmode
Enables slowmode in certain channels. Use ``0`` to clear slowmode.
```
/slowmode <Seconds>
```

#### Tempban
Temporary ban an user from the guild.
```
/tempban <User> <Duration> [Reason]
```
![3b3ebfe70a9463d73bd7e418d1bbd949](https://user-images.githubusercontent.com/73501749/164980656-6370afb7-2eb8-4882-9031-452bede51a74.png)

#### Tempmute
Prevent an user of sending messages in the guild temporary.
```
/tempmute <User> <Duration> [Reason]
```
![b8301a01813ee1909798ac4dac431552](https://user-images.githubusercontent.com/73501749/164980715-67a69c2e-cc4c-4cd7-a11b-2622d17e3895.png)

#### Unban
Unban an user from the guild.
```
/unban <ID>
```
![c81287c57d38d9a01e7bdcc5d01a3c32](https://user-images.githubusercontent.com/73501749/164980766-b172eb50-a5df-45be-b6c4-69280b4242a5.png)

#### Unlock
Unlock a channel.
```
/unlock <Channel>
```
![29c56d983a6656acbdd95d07d77686a7](https://user-images.githubusercontent.com/73501749/164980809-48fa83b6-be26-4fbf-bdf7-3be4ff326f42.png)

#### Unmute
Unmute an user from the guild.
```
/unmute <User> [Reason]
```
![cd6f9f3b2700cef34dff392af1e6f073](https://user-images.githubusercontent.com/73501749/164980844-fe8546c8-febe-4d63-9530-b02add3dacc5.png)

#### Unwarn
Unwarn an user.
```
/unwarn <User> <IDs> [Reason]
```
![b3cc00a14b6355661ff5aba764ff9345](https://user-images.githubusercontent.com/73501749/164980890-a00cefad-8e4b-42f5-90a7-1a26fb4597e4.png)

#### Warn
Warn an user. **Amount:** How many warnings should the user receive for the rule break.
```
/warn <User> [Amount] [Reason]
```
![a2bfba370496ad55fb4326ffb9fc4308](https://user-images.githubusercontent.com/73501749/164980975-4f70d464-e6d4-4328-8479-92d61e680a87.png)

#### Warnhistory
Displays warn history of an user.
```
/warnhistory <User>
```
![440567181e6c220b26bc6ed37d89696d](https://user-images.githubusercontent.com/73501749/164981046-dab92c23-7bf8-42e6-bf18-cd32e6a677b2.png)

> __________________________

<br />
<a href="https://discord.gg/tsG2ZJW9"></strong></a>
<br />

> Management commands
#### Approve
Approve a suggestion.
```
/approve <SuggestionID> [Reason]
```
![48bf9c17437d7c1e76fdf652f0554d66](https://user-images.githubusercontent.com/73501749/164981400-9365516f-1780-412d-81f2-1b6ca2d09fcf.png)

#### Booster
Manage Booster bundle system.
```
/booster <add/remove/info> <user> <realm> <ign>
```
![4f9a8517d2433a7e363fa4e0ed4a7569](https://user-images.githubusercontent.com/73501749/164981497-ede1f872-0e11-4640-bd95-bda98ef07182.png)

#### Bundle
Manage Team bundle system.
```
/booster <add/remove/info> <user> <realm> <ign>
```

#### Changelog
Submit a new changelog.
```
/changelog <changes> [channel]
```

#### Clearbundle
Clear bundle data.
```
/clearbundle <team/booster/all> <realm>
```

#### Clearstrike
Clear strike data.
```
/clearstrike <gamemode>
```

#### Dbcreate
Creates required database tables.
```
/dbcreate
```

#### Demote
Demote a staff member.
```
/demote <User> <Role>
```
![4ddb82f23e846470315aad43417df4b2](https://user-images.githubusercontent.com/73501749/164981690-3f7f312f-d43b-4b7f-94b2-f9586c4a0711.png)

#### Embed
Embed manager.
```
/embed <Title> <Description> [Channel]
```

#### Gcreate
Create a new giveaway.
```
/gcreate <Channel> <Duration> <Winners> <Prize>
```
![ea1968fcb9e4fb5a1966d36c3638adb1](https://user-images.githubusercontent.com/73501749/164981790-8529f80b-c8cf-406a-ab75-cf4dd16d02c4.png)

#### Gend
End a giveaway.
```
/gend <MessageID>
```
![b06c99fce85b164f0b47423b555a38f3](https://user-images.githubusercontent.com/73501749/164981834-ea801f31-d0cf-47c7-88a3-b2453228e25e.png)

#### Greroll
Reroll a giveaway.
```
/greroll <MessageID>
```

#### leader
Applies the leader role.
```
/leader <gamemode> <user> <teamName>
```
![924c8c691f5b4fa8837b8330c0c42861](https://user-images.githubusercontent.com/73501749/164981910-af00f76b-67c7-4c5c-bf49-788e0bc589e9.png)

#### Lockdown
Enables/Disables lockdown mode. No commands/events/features can be executed.
```
/lockdown
```

#### Lookup
Displays information about a certain user.
```
/lookup [User]
```
![db6843b155a047e9d62b7377d39556b2](https://user-images.githubusercontent.com/73501749/164981962-1a0884dd-a739-42c8-9fa6-eabdc29a8b70.png)

#### Playingadd 
Add an user to the playing list.
```
/playingadd <gamemode> <teamName>
```
![7d00e0aaca8f69e18cb962811ff56a28](https://user-images.githubusercontent.com/73501749/164982008-fc39229e-107b-46e6-af8f-fd1a72b52b91.png)

#### Playingclear
Clears the playing list.
```
/playingclear <gamemode>
```

#### Playinglist
Sends the playing list.
```
/playinglist <gamemode> <channel>
```

#### Playingremove 
Remove a team of the playing list.
```
/playingremove <gamemode> <team>
```

#### Promote
Promote a staff member.
```
/promote <User> <Role>
```
![f122236cf99126ec93d071612613117e](https://user-images.githubusercontent.com/73501749/164982075-5f717cba-5699-415e-9207-454cc50aac39.png)


#### Reactionpanel
Creates a reactionpanel.
```
/reactionpanel <channel> <messageID> <Options>
```

#### Reload
Reload a command. Not Recommended!
```
/reload <command>
```

#### Restart
Restart the bot. 
```
/restart
```

#### Sdeny
Deny a suggestion.
```
/sdeny <SuggestionID> <Reason>
```
![592e18104bf036b842b1ab130339e03f](https://user-images.githubusercontent.com/73501749/164982207-715bba8b-d9de-45ef-a98f-c86f2e8ea106.png)

#### Sendmsg
Send a message with the bot
```
/sendmsg <Channel> <Message>
```

#### Setup
Refers to this documentation.
```
/setup
```

#### Strike
Strike a team.
```
/strike <gamemode> <team> <strikeAmount> <reason>
```
![3019d6365badaf1d9844af1e6ad724f0](https://user-images.githubusercontent.com/73501749/164982316-461bde60-d401-4592-a390-f8344c9d5a49.png)

#### Strikeset
Set the amount of strikes a team received
```
/strikeset <gamemode> <team> <strikes>
```

#### Verifypanel
Sends the verification panel. In dms or guild channel using panel.
```
/verifypanel
```
![3a5f6cad43c07e8f7442c90fb32a5d72](https://user-images.githubusercontent.com/73501749/164982384-d643e593-e845-42bb-84e4-f09b4a870f1e.png)



## Features
### DB Cleanup
#### Tickets & Applications
Once a user leaves the guild the bot will close any tickets/application the user created and log everything in the specific channel.
```yaml
ticket_close_on_leave: {Boolean}
application_close_on_leave: {Boolean}
```
```yaml
ticket_close_on_leave: true
application_close_on_leave: true
```

### Event Logs
Whenever an event gets emited the bot will send a log embed in the specific channel.
```yaml
logs:
  events:
    channel_create: {Boolean}
    channel_delete: {Boolean}
    user_join: {Boolean}
    user_leave: {Boolean}
    message_edit: {Boolean}
    message_delete: {Boolean}
    role_create: {Boolean}
    role_delete: {Boolean}
    thread_create: {Boolean}
    thread_delete: {Boolean}
  tickets:
    close: {Boolean}
  moderation:
    warn: {Boolean}
    unwarn: {Boolean}
    kick: {Boolean}
    mute: {Boolean}
    tempmute: {Boolean}
    unmute: {Boolean}
    ban: {Boolean}
    tempban: {Boolean}
    unban: {Boolean}
  applications:
    accept: {Boolean}
    deny: {Boolean}
  bot:
    lockdown: {Boolean}
    mute_bypass: {Boolean}
    ban_bypass: {Boolean}
    auto_verification: {Boolean}
    error: {Boolean}
```
```yaml
logs:
  events:
    channel_create: true
    channel_delete: true
    user_join: true
    user_leave: true
    message_edit: true
    message_delete: true
    role_create: true
    role_delete: true
    thread_create: true
    thread_delete: true
  tickets:
    close: true
  moderation:
    warn: true
    unwarn: true
    kick: true
    mute: true
    tempmute: true
    unmute: true
    ban: true
    tempban: true
    unban: true
  applications:
    accept: true
    deny: true
  bot:
    lockdown: true
    mute_bypass: true
    ban_bypass: true
    auto_verification: true
    error: true
```
![0da20d9bb597dbe1d37b6f2d4b050140](https://user-images.githubusercontent.com/73501749/164982986-c2660dd0-0a45-477f-8486-a2ca00331426.png)


### Alt Detection
Whenever a user joins the guild the bot will check if the user could be a possible alt account.
```yaml
alts:
  enabled: {Boolean}
  account_created: {Integer}
  notification: {Boolean}
  verification: {Boolean}
  punishment:
    mute: {Boolean}
    ban: {Boolean}
```
```yaml
alts:
  enabled: true
  account_created: 60 # How old should be an account atleast be to bypass the punishment below. (days)
  notification: true # Whether a message should be send in the specific channel
  verification: true # Whether the user should be able to start the verification proccess
  punishment:
    mute: false # Whether the user should be muted
    ban: false # Whether the user should be banned
```
![065007016fd3bf794c093974b35e7c76](https://user-images.githubusercontent.com/73501749/164983157-7502f2e2-9822-4372-b0a0-d7b1bfbbbffe.png)

### Application
Step by step discord application. Fully configurable.
```yaml
questions: {Array}
```
```yaml
questions:
  - "Question 1"
  - "Question 2"
  - "Question 3"
```
![31f2e96419f2a4b5ab007ee8c3b7790e](https://user-images.githubusercontent.com/73501749/164983273-807f334b-033a-462d-ab51-f39205cf4891.png)
![2e689dba3c686601c3f42e06c7525f98](https://user-images.githubusercontent.com/73501749/164983274-d27f2137-d67e-4d85-a534-d262df8ee43c.png)

### Auto Moderation
Automatic Moderation System. Keep your discord save from spam pinger, insults, advertisements and much more!

```yaml
  links:
      enabled: {Boolean}
      blacklisted_links: {Array}
      whitelist_gifs: {Boolean}
      whitelisted_channels: {Array}
      tickets_bypass: {Boolean}
      role_bypass:
        enabled: {Boolean}
        role_id: {String}
      punishment:
        warning: {Boolean}
        mute:
          enabled: {Boolean}
          permanent: {Boolean}
          duration: {String}
        ban:
          enabled: {Boolean}
          permanent: {Boolean}
          duration: {String}
```
```yaml
  links:
      enabled: true # Whether this mode should be enabled
      blacklisted_links: # Messages that includes these characters will be deleted and a punishment executed
        - "discord.gg"
        - "https"
      whitelist_gifs: true # Whether gifs should not be deleted
      whitelisted_channels: # Messages that were sent in one of these channels will be not checked. (e.g. recruitement channel)
        - "804354114451800064"
      tickets_bypass: true # Whether messages should be checked that were sent in ticket channels
      role_bypass:
        enabled: true # Whether the messages of users who do not inherit the role (or one above; configured below) should be checked
        role_id: "884573835205148692"
      punishment:
        warning: true # Whether the user should be warned
        mute:
          enabled: false # Whether the user should be muted
          permanent: false # Whether the user should be permanently muted
          duration: "1h" # Duration of temporary mute
        ban:
          enabled: false # Whether the user should be banned
          permanent: false # Whether the user should be permanently banned
          duration: "1h" # Duration of temporary ban
```
> Note: download the config.yml file to see all configuration options.

### Welcome
Whenever a user joins the bot will send a welcome message. It will also check whether the user attempted to bypass a mute/ban punishment. When enabled users who rejoin the guild will also automatically verified if they verified themself before leaving the guild.
```yaml
  auto_verification: {Boolean}
  welcome:
      sendEmbed: {Boolean}
  auto_mute: {Boolean}
  auto_ban: {Boolean}
```
```yaml
  auto_verification: true # Whether users should be auto verified if they leave and join the guild after a successfull verification.
  welcome:
      sendEmbed: true
  auto_mute: true # Whether users should be muted again after they leave and join the guild to bypass the mute punishment
  auto_ban: true
```
![ae1c6640da39d602f5475d544fd9ee63](https://user-images.githubusercontent.com/73501749/164983551-08a25998-507a-44c6-b3d8-268b17efd756.png)

> A few more features are coming soon!

## Developer API
### Commands
You can create and add as much commands as you want. Just execute ``node template.js`` in console and it will generate everything for you. It will be automatically added to the help list once you added and restarted the command.

### Managers
Available Managers: Util, Module, listener & handler.

**Util:**
  * Console Logging
  * MongoDB Management
  * Config Management
**Module:**
  * Moderation Management (ban, mute, ...)
  * Ticket Management
**Listener:**
  * Giveaway
  * Bundle
  * Lockdown
  * Stats
  * Punishments
**Handler:**
  * Event
  * Log
  * Commands

Import each file and you will be given access to all methods. As of right now please use an editor like Visual Studio Code to develop any features for the bot. If you hower over the import variable you will see all available methods including their usage & description.
All methods will be added later once the bot is 100% published.

## Errors
![90a7b4e6c616d6a5716502fcafce69f9](https://user-images.githubusercontent.com/73501749/164983955-918835a4-c646-4419-959a-5ed8c21d78d0.png)

### Discord API Error
Discord API Errors usually occurs when the bot doesn't have the permission to perform an action. Please make sure that the bot inherits the ``ADMINISTRATION`` Permission. NOTE: If a user inherits ``ADMINISTRATOR`` permission the nickname cannot be changed.
If these issues occurs more often create a ticket in our support discord otherwise leave it alone.

### Bot Error
If the Error ``type`` is **critical** please make sure to open a support ticket as soon as possible. As being said in the embed our system automatically reports any issues that occured however we may need more details when the error is critical.

### Console Error
Any errors are getting logged in the console. Every information that is needed to fix a bug can be found in console.
![d0076e37cca08c4fe692f28ad59a2953](https://user-images.githubusercontent.com/73501749/164984094-b434029a-10ca-46f6-8717-3e3c26bb8307.png)



## Note
Please Note that the bot is currently in **private beta**. It cannot be bought.
