<h1 align="center"> Documentation</h1>
<h2>About the bot</h2>

Ice Server Bot is a usefull tool to manage a minecraft server community. It includes several highly configurable commands and features that are needed.
Check this to see all benefits of Ice Server Bot.

The Server Bot supports Windows, and Ubuntu and works from Discord.js v12 - v13 depending on the used bot version.

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
- [Welcome](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Gamemode Specific](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Other Features](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)

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
  
![de8375a01bd0471b4a69c8d229c5095a](https://user-images.githubusercontent.com/73501749/134370218-6c3a694c-44c6-4833-b5ca-491977ab171a.png)

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
      permission:
        role_permission: false #Enable if the bot should use roles as permissions instead of permission notes. (Recommended)
        required_role: "804354021481381909" #If "role_permission" is enabled, the user will need this role or one above to be able to execute this command.
        permission: "VIEW_CHANNEL" #If "role_permission" is disabled, the user will need this permission note to be able to execute this command.
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

![bc5df96783bb24491e60849a21028500](https://user-images.githubusercontent.com/73501749/134371930-b7c2a884-431a-4ee4-8ad6-7173328cb4a0.png)

  ```yaml
tickets:
  options:
    role_advantage:
      enabled: true #Either if this feature should be enabled or disabled.
      advantage_role_id: "804354029076348959" #If it's enabled the bot will check if the ticket creator got this role (e.g. booster role)
      mention_role_id: "804354029076348959" #The bot will mention this role if the ticket creator inherits the role above. (=> faster support for server booster)
    mention_support_role: true #Either if the support role should be @ in new tickets
    mention_senior_staff_role: true #Either if the support role should be @ in new tickets
    ticket_create_cooldown: 10 #Ticket creation cooldown per option in minutes
    ticket_create_options:
      factions:
        enabled: true #Either if this ticket option should be enabled or not
        category_id: "833732233021751306" #Category ID of this ticket type
        permissions:
          support: true #Either if users with the support role should be able to see tickets of this type or not
          senior_staff: true #Either if users with the senior staff role should be able to see tickets of this type or not
```
Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![dd97bcc1c5d415ed42bd7d5cc16cf042](https://user-images.githubusercontent.com/73501749/134373384-d2cfbb82-ae0a-4475-b39b-6ca1fa7486a4.png)
![29a5eb6bece9adcc758fa6da7819fe98](https://user-images.githubusercontent.com/73501749/134380096-beafbb87-6e33-473d-a91c-41cf27ee158a.png)
![5b16e05559953bc6b9017cf3891d5d51](https://user-images.githubusercontent.com/73501749/134381836-8b1bbae7-bb66-46ac-89f3-6454ea9834e1.png)
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
- **iq <@User>**
- **joke**
- **meme**
- **nuke**
- **pickupline**
- **reverse [Message]**
- **rip [@User]**
- **roll**
- **shit [@User]**
- **trash [@User]**
- **wasted [@User]**
- **weather [City]**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![72ac56506899047ce88aef8944dd1ea3](https://user-images.githubusercontent.com/73501749/134394271-49723321-a89d-44a2-9396-5b9bff3ead8b.png)
![261bf110750461d2178144bcd3e704f0](https://user-images.githubusercontent.com/73501749/134394338-e68a349f-2b01-4b6e-b1b3-308e2f69c1fc.png)
![ae49bc4ebc84d29f236d18083ffc68bd](https://user-images.githubusercontent.com/73501749/134394441-fc677e62-170b-4d7a-88cc-25d78a75dc3a.png)
  
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

- **accept [@User] [@Role]**
- **appdeny <@User>**
- **dbcreate**
- **demote [@User] [@Role]**
- **devreport [Error]** (In Development!!!)
- **dm [@User] <Message>**
- **embed <#Channel> [Title] [Content]**
- **lookup <@User>**
- **promote [@User] [@Role]**
- **reload [Command]**
- **resign <@User>**
- **restart**
- **sendmsg <#Channel> [Content]**
- **setup [Option]**  (In Development!!!)
- **verifypanel**

<h3>Configurating:</h3>

Commands can be configured like explained above. ([here](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#configurating))

<h3>Showcase:</h3>

![1cfb702f36b47dd6b3663b32cdf61654](https://user-images.githubusercontent.com/73501749/134396332-6fa7d2d4-d0d1-434a-8baa-11780dda1b59.png)
![17647d70e76a9a934c32dbf4b0093ff3](https://user-images.githubusercontent.com/73501749/134396429-ad8af59b-4465-43d1-8c50-56d5c2b0ae53.png)
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
![7ccb5df6dea41b407ea0d28538428e36](https://user-images.githubusercontent.com/73501749/134397091-13655a58-359c-4640-a261-6732bb1c3542.png)
![ed7bb2f70877ae712983980817ca8a18](https://user-images.githubusercontent.com/73501749/134397100-8123ea46-c3c9-4bd0-9cad-639edd9b2f78.png)

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
