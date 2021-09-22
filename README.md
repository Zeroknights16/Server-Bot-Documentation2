<h1 align="center"> Documentation</h1>
<h2>About the bot</h2>

Ice Server Bot is a usefull tool to manage a minecraft server community. It includes several highly configurable commands and features that are needed.
Check this to see all benefits of Ice Server Bot.

The Server Bot supports Windows, and Ubuntu and works from Discord.js v12 - v13 depending on the used bot version.

<h2>Features Overview</h2>
Ice Server Bot have an amount of commands & features for different uses. At here you find the complete feature list:
<h3> </h3>

- [General](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#general)
- [Tickets](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
- [Moderation](https://github.com/Zeroknights16/Ice-Dev-Server-Bot-V2/blob/main/README.md#features-overview)
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
  
![configurating1](https://user-images.githubusercontent.com/73501749/134250196-28c099c8-4aec-42b3-8155-a9b339076632.png)

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
  
![pic2](https://user-images.githubusercontent.com/73501749/134368410-0c73008a-73f0-4e72-bc3a-c0bea0547e36.png)
![pic233](https://user-images.githubusercontent.com/73501749/134368972-0b884f64-52da-4c8a-b024-3722b9d7eef8.png)
![ffacd8a3b59e53eb2f725fbb9bca1a35](https://user-images.githubusercontent.com/73501749/134369465-7b820e4c-11a1-449c-80c4-4146f3e3a57a.png)
