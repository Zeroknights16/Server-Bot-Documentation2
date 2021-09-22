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
- [Fun](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Suggestions](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Management](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Giveaways](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Logs](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Auto Mod](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
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
