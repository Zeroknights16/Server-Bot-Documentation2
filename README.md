<h1 align="center"> Documentation</h1>
<h2>About the bot</h2>

Ice Server Bot is a usefull tool to manage a minecraft server community. It includes several highly configurable commands and features that are needed.
Check this to see all benefits of Ice Server Bot.

The Server Bot supports Windows, and Linux and works from Discord.js v12 - v13 depending on the used bot version.

<h2>Features Overview</h2>
Ice Server Bot have an amount of commands & features for different uses. At here you find the complete feature list:
<h3> </h3>

- [General](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#general)
- [Tickets](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#tickets)
- [Moderation](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#moderation)
- [Fun](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#fun)
- [Suggestions](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#suggestions)
- [Management](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#management)
- [Giveaways](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#giveaways)
- [Logs](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#logs)
- [Auto Mod](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#auto-mod)
- [Welcome](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#welcome)
- [Gamemode Specific](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#gamemode-specific)
- [Staff Discord](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#staff-discord)
- [Other Features](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#other-features)

<h2>General</h2>

<h3>Available Commands:</h3>

- **botinfo**
- **help <option>**
- **invites <@User>**
- **invitetop**
- **info <@User>**
- **ip**
- **permission <@User>**
- **ping**
- **server**
- **uptime**
- **vanity**

<h3>Configurating:</h3>
  
![913cc3a5cc3367772efad195338fdd92](https://user-images.githubusercontent.com/73501749/153496132-5374d160-5647-4280-85bc-aa4304bb3dc3.png)
![8c2738f0ac588135ae62a1882250c5b8](https://user-images.githubusercontent.com/73501749/153496281-09b0098c-3cce-494b-bba6-604f9d9012c6.png)

```yaml
general:   
  commands:
    botinfo:
      enabled: true #Every command can be disabled. Put "false" instead of "true" to disable a command.
      aliases: #Every command can have its own aliases. This command will also be executed if an user type "<prefix>binfo". It can have up to unlimited aliases. It is not recommended to setup more than 2 aliases per command as it makes the bot slow.
        - "binfo"
      description: "Displays information about the bot" #Command Description
      usage: "botinfo" #Command Usage (Not Recommended to edit.)
      example: "botinfo" #Command Usage Example (Not Recommended to edit.)
      cooldown: 3 #Command Cooldown (Not recommended to set under 3 seconds.)
```
```json
"botinfo": {
    "role_permission": true, # Whether the user requires a role or permission node to be able to execute this command
    "role_id": "804354037662220289", # Required Role (everyone who owns this role or one above will be able to execute this command)
    "permission_node": "VIEW_CHANNEL" # Required permission node
  },
```

<h3>Showcase:</h3>
  
![9df5dd9f62c12142156c00f1bccd57ad](https://user-images.githubusercontent.com/73501749/134369668-d7ed903d-7868-4ea8-8ee7-015714e514d8.png)
![8dbea11437a0ac9065a183ee906954eb](https://user-images.githubusercontent.com/73501749/134369846-7757d18b-baf9-4f96-8474-820f5951f3b5.png)
![84e853e042864cfb7e5bf68a37849a3a](https://user-images.githubusercontent.com/73501749/134369993-c85c959f-66d4-4867-83f0-f8e6c74d2f66.png)

<h2>Tickets</h2>
 
<h3>Available Commands:</h3>
  
- **add [@User]**
- **blacklist [@User] <Reason>**
- **close <Reason>**
- **private [Mode]**
- **remove [@User]**
- **rename [Name]**
- **ticketpanel**
- **tleaderboard**
- **unblacklist [@User] <Reason>**

<h3>Configurating:</h3>

![2aad3e3d0b5c235f185a3fcf2fe25248](https://user-images.githubusercontent.com/73501749/153496784-86bc7566-1a79-4467-8343-e51a3b1ef65f.png)

  ```yaml
tickets:
  options:
    role_advantage:
      enabled: true
      advantage_role_id: "878410148874448928" # e.g. Booster Role id
      mention_role_id: "884573835205148692" # e.g. if the ticket creator boosted the server staff members are getting @ for faster support.
    mention_support_role: false #only tags in categorys where they have permissions to see it
    mention_senior_staff_role: false #only tags in categorys where they have permissions to see it
    cooldown_options: 
      ticket_create_cooldown: 5 #minutes
      bypass_role_enabled: true
      bypass_role_id: "884573835205148692"
    ticket_creation_message:
      enabled: true # Whether a message should be send in the ticketpanel channel that his/her ticket was created. (e.g. Hey @Zeroknights, your ticket (ticket#2422) was successfully created.)
      deletion: 8 # After how many seconds should be the message deleted
    ticket_create_options:
      factions:
        enabled: true
        category_id: "833732233021751306"
        permissions:
          support: true
          senior_staff: true
```
Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![test22222](https://user-images.githubusercontent.com/73501749/139645220-87202596-d428-4159-9fa8-1971d4f6c487.png)
![29a5eb6bece9adcc758fa6da7819fe98](https://user-images.githubusercontent.com/73501749/134380096-beafbb87-6e33-473d-a91c-41cf27ee158a.png)
![b85d54269f5371d321657275d69b85e6](https://user-images.githubusercontent.com/73501749/153497121-c083dbf5-cd02-439a-9a0d-caf74cb9ba33.png)
![b23906dbaaa1971369512d03cd7d0765](https://user-images.githubusercontent.com/73501749/134381893-4e3c55b2-ed6b-4591-86fb-23411f8d984f.png)
![2e5ed11abb2fdef318b754c348a9a52f](https://user-images.githubusercontent.com/73501749/134381953-9165b3c3-e06b-44d5-ad56-7c13c59d2559.png)
![8fdce9d8e5df416a7b4a7a0170e90f6c](https://user-images.githubusercontent.com/73501749/134382290-7d82d2b6-9f53-4ff6-b1e8-9375b898be9e.png)

<h2>Moderation</h2>

<h3>Available Commands:</h3>

- **ban [@User] <Reason>**
- **kick [@User] <Reason>**
- **lock <#Channel>**
- **mute [@User] <Reason>**
- **purge [Amount]**
- **slowmode [Seconds] <#Channel>**
- **tempban [@User] [Duration] <Reason**
- **tempmute [@User] [Duration] <Reason**
- **unban [ID]**
- **unlock <#Channel>**
- **unmute [@User] <Reason>**
- **unwarn [@User]**
- **warn [@User] <Reason>**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![222](https://user-images.githubusercontent.com/73501749/134393042-28e3b95b-b7c3-4e54-a494-f65ec6f6bffa.png)
![f5cbb646ad96ba050aeae7f2452f8e69](https://user-images.githubusercontent.com/73501749/134393150-dbc8a50f-67f6-4c03-b93b-e711023d2f8c.png)
![03f606b5196c6f763411338c49cfe4de](https://user-images.githubusercontent.com/73501749/134393514-1cbd8c88-4887-48dc-a7fd-c04e7d442258.png)

<h2>Fun</h2>

<h3>Available Commands:</h3>

- **ask [Question]**
- **bird**
- **dicksize [@User]**
- **dog**
- **fact**
- **iq**
- **joke**
- **meme**
- **nuke**
- **reverse [Message]**
- **rip [@User]**
- **roll**
- **rps**
- **shit [@User]**
- **trash [@User]**
- **wasted [@User]**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![72ac56506899047ce88aef8944dd1ea3](https://user-images.githubusercontent.com/73501749/134394271-49723321-a89d-44a2-9396-5b9bff3ead8b.png)
![261bf110750461d2178144bcd3e704f0](https://user-images.githubusercontent.com/73501749/134394338-e68a349f-2b01-4b6e-b1b3-308e2f69c1fc.png)
![ae49bc4ebc84d29f236d18083ffc68bd](https://user-images.githubusercontent.com/73501749/134394441-fc677e62-170b-4d7a-88cc-25d78a75dc3a.png)
![873893c2a1f8271a10ec323648173102](https://user-images.githubusercontent.com/73501749/153497753-50658b3c-2c0f-41e6-9658-3d0c584c83e8.png)

  
<h2>Suggestions</h2>

<h3>Available Commands:</h3>

- **suggest [Suggestion]**
- **approve [ID] <Comment>**
- **deny [ID] <Comment>**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![a2c63e140f22e6fc664fcc85c1d55adb](https://user-images.githubusercontent.com/73501749/134395295-1dd64019-82f3-4c41-9727-98192636ba98.png)
![cf501939a4621a887135cb94ad736456](https://user-images.githubusercontent.com/73501749/134395356-920fd72e-d73d-4b71-91d3-8dc81862cd73.png)
![13b110f2a69c63648b607b00ad7272ba](https://user-images.githubusercontent.com/73501749/134395393-946d2d41-dd9f-4b87-b533-07536ac773e7.png)
  
<h2>Management</h2>

<h3>Available Commands:</h3>

- **accept [@User] [<@>Role]**
- **appdeny <@User>**
- **dbcreate**
- **demote [@User] [<@>Role]**
- **deny**
- **devreport [Error]** (In Development!!!)
- **dm [@User] <Message>**
- **embed <#Channel> [Title] [Content]**
- **lookup <@User>**
- **poll [channel] "[title]" "[emojis]" "[options]"**
- **promote [@User] [<@>Role]**
- **reload [Command]**
- **resign <@User>**
- **restart**
- **sendmsg <#Channel> [Content]**
- **setup [Option]**
- **verifypanel**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![1cfb702f36b47dd6b3663b32cdf61654](https://user-images.githubusercontent.com/73501749/134396332-6fa7d2d4-d0d1-434a-8baa-11780dda1b59.png)
![43abece3c8f80e6cad1b7db676dfe526](https://user-images.githubusercontent.com/73501749/139645951-5f5229ef-6b45-408c-95cd-1590ff3d4c26.png)
![e313d2d3aa4b1150a373169aebab39e6](https://user-images.githubusercontent.com/73501749/134396533-193b73f2-4315-4790-8e19-afe7fc448eef.png)

<h2>Giveaways</h2>

<h3>Available Commands:</h3>

- **gcreate [#Channel] [Time] [winnerCount] [Prize]**
- **gend [Message ID]**
- **greroll [Message ID]**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![618d65f4d4bf1619d352327cbb67f3f8](https://user-images.githubusercontent.com/73501749/134397080-df902f9a-99e1-4bab-8a59-70729fcc1858.png)
![64379f25f8bae385c26c0b2aad5b4761](https://user-images.githubusercontent.com/73501749/153498092-c5bc4472-9b75-45c5-9870-d842bf534c90.png)


<h2>Logs</h2>

<h3>Available Commands:</h3>
N/A

<h3>Configurating:</h3>

![572f96443c9e437270972fbd71b10e82](https://user-images.githubusercontent.com/73501749/134397484-2cc88795-4c13-4aa5-8966-25cd386a305f.png)

```yaml
logs: #Either if a event or command should be logged or not
  events:
    channel_create: true
    channel_delete: true
    user_join: true
    user_leave: true
    message_edit: true
    message_delete: true
    role_create: true
    role_delete: true
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
    mute_bypass: true
    auto_verification: true
```

<h3>Showcase:</h3>

![5cb374f927cf50c152e894c6a37834ba](https://user-images.githubusercontent.com/73501749/134397813-958c899b-fc91-4ac7-92fe-e4ca94781437.png)
![ea27c43720424a0c4e1381eb9ecf3b24](https://user-images.githubusercontent.com/73501749/134398030-56ef1013-4c45-466e-869b-c46374884fc6.png)
![55c92f56a4f198187687014ca3e4786c](https://user-images.githubusercontent.com/73501749/134398124-b92c4783-7366-4cc4-9eeb-c5bc6c4b20a6.png)

<h2>Auto Mod</h2>

<h3>Available Commands:</h3>
N/A

<h3>Configurating:</h3>

![13b9a9fe6b1c82bfaecb10e37312a2fa](https://user-images.githubusercontent.com/73501749/134398387-98341db0-88f1-47e9-af4d-0cdbce0809bf.png)

```yaml
auto_mod:
  options:
    links:
      enabled: true #Either if this option is enabled or not
      blacklisted_links: #List of links that should be deleted
        - "discord.gg"
        - "https://www.youtube.com/"
      whitelisted_channels: #List of channel id's that should not be checked by the bot
        - "804354133124448286"
        - "804354133124448286"
      tickets_bypass: true #Either if ticket channels should be checked or not
      role_bypass:
        enabled: true #Either if this option is enabled or not
        role_id: "804354021481381909" #Role ID that bypass the auto mod
      punishment: #Punishment for sending a blacklisted link
        warning: true
        mute:
          enabled: false
          permanent: false
          duration: "1h"
        ban:
          enabled: false
          permanent: false
          duration: ""
    words:
      enabled: true #Either if this option is enabled or not
      blacklisted_words: #List of blacklisted words
        - "nigga"
        - "nigger"
      role_bypass:
        enabled: true #Either if this option is enabled or not
        role_id: "804354021481381909" #Role ID that bypass the auto mod
      punishment: #Punishment for sending a blacklisted word
        warning: true
        mute:
          enabled: false
          permanent: false
          duration: "1h"
        ban:
          enabled: false
          permanent: false
          duration: "1h"
    pings:
      enabled: true #Either if this option is enabled or not
      max_pings_per_message: 10 #Maximum pings per message
      role_bypass:
        enabled: true #Either if this option is enabled or not
        role_id: "804354021481381909" #Role ID that bypass the auto mod
      punishment: #Punishment for spam pinging
        warning: true
        mute:
          enabled: false
          permanent: false
          duration: "1h"
        ban:
          enabled: false
          permanent: false
          duration: "1h"
```

<h3>Showcase:</h3>

![a1d9893d5da6631a4282245db6aaceaa](https://user-images.githubusercontent.com/73501749/134404815-ecee6465-9bbc-4f91-869c-e54dd3995023.png)
![6de15ef3b0244a7365bbdfcf8ec2876a](https://user-images.githubusercontent.com/73501749/134404829-75769820-686b-4d2b-9471-c8a70d835072.png)

<h2>Welcome</h2>

<h3>Available Commands:</h3>
N/A

<h3>Configurating:</h3>

![6086dc6c321217439c3370da7f054e8f](https://user-images.githubusercontent.com/73501749/134405494-2aea18e8-30bc-4841-80c9-4cb67cd0791d.png)

```yaml
welcome:
  options:
    enabled: true
    picture: #BETA!!!!! - There might be a few bugs.
      enabled: true
      pictures: #database/pictures/...
        - "Bild1"
        - "Bild2"
    embed:
      enabled: true
```

<h3>Showcase:</h3>

![6086dc6c321217439c3370da7f054e8f](https://cdn.discordapp.com/attachments/804354078943608842/833611123361316864/welcome-image.png)

<h2>Gamemode Specific</h2>

<h3>Available Commands:</h3>

- **clearstrike [Gamemode/All]**
- **gend [Message ID]**
- **leader [@User] [Gamemode] [Name]**
- **playingadd [Gamemode] [Name]**
- **playingclear [Gamemode]**
- **playinglist [Gamemode]**
- **playingremove [Gamemode] [Name]**
- **strike [Gamemode] [Name] [Strikes] [Reason]**
- **strikeset [Gamemode] [Name] [Amount]**

<h3>Configurating:</h3>

![a1714cfb860e4dda1b65067431d47632](https://user-images.githubusercontent.com/73501749/134406811-d2575565-4894-480e-a5b2-6da46305e3c1.png)

```yaml
gamemode:
  options:
    leader_discord:
      faction:
        discord_link: "https://discord.gg/"
      skyblock:
        discord_link: "https://discord.gg/"
      prison:
        discord_link: "https://discord.gg/"
    strikes:
      faction:
        first_value_deduction: 2 #How much strikes do a Faction need to receive their first value deduction
        strikes_per_step: 2 #How much strikes do a Faction need to get to the next stage
        value_deduction_per_step: 10 #How much value deduction do a Faction receive after getting to the next stage
        max_strike_amount: 10 #What's the maximun amount of strikes a Faction can have
      skyblock:
        first_value_deduction: 2
        strikes_per_step: 2
        value_deduction_per_step: 10
        max_strike_amount: 10
      prison:
        first_value_deduction: 2
        strikes_per_step: 2
        value_deduction_per_step: 10
        max_strike_amount: 10
```
Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![6d47d61a7737466e1285e1a72d39936b](https://user-images.githubusercontent.com/73501749/134407184-ea32c01f-89a4-416e-8715-c9372e5dfc8a.png)
![952ffe1de67a84221bfc29078cf2dba4](https://user-images.githubusercontent.com/73501749/134407310-15c6c33d-c1c4-4de6-b6b8-6217ea555e90.png)
![4ee4a43df93cf3192930333c79996013](https://user-images.githubusercontent.com/73501749/134407410-e0e3d389-47bd-4cfd-98e5-82f854dde0c9.png)

<h2>Staff Discord</h2>

<h3>Available Commands:</h3>

- **staffstrike [@User] <Reason>**
- **staffvote [Strike/DQ/Appeal] [Name] [Evidence/Banned For] <Reason>**

  
<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![a7753a2e2f6a7a3c68a6b6ab7ca70f73](https://user-images.githubusercontent.com/73501749/139646905-762e08ac-15fe-4036-a87f-5615e30c5742.png)
![5d7b9398863095f9f2707aac4fea2aef](https://user-images.githubusercontent.com/73501749/139647025-3e66d63c-ce27-45d0-8aa3-43050e15e43c.png)

<h2>Other Features</h2>

- **Users who got muted can not bypass the punishment via leaving and joining the guild back.**
- **The Auto Moderation does also work when a message was edited and not only when a message was sent**
- **All Timers Persist After Bot Restart ( e.g.: Temp Mutes, Giveaways )**
- **All messages can be edited in the message.yml file**
- **Confirmation menus**
- **and much more...**
