<p align="center">
  <img src="https://github.com/BrewTheFox/ReKITtyPaw/blob/main/images/rainbow-color.gif?raw=true" alt="ReKITtyPaw" width="100%", =50%>
</p>

<h1 align="center">
  ReKITtyPaw
</h1>

<p align="center">
  <img src="https://github.com/BrewTheFox/ReKITtyPaw/blob/main/images/Shulker.gif?raw=true" alt="ReKITtyPaw" width="10%">
</p>


<p align="center">
  <img src="https://github.com/BrewTheFox/ReKITtyPaw/blob/main/images/rainbow-color.gif?raw=true" alt="ReKITtyPaw" width="100%">
</p>

## What is this?
#### ReKITtyPaw is a Minecraft bot designed to simplify the setup of kit delivery bots in anarchy servers. Developed in JavaScript using the Mineflayer library, ReKITtyPaw aims to simplify the configuration process through an easy-to-use JSON file.

## Key Features:

- #### Easy to configure.
- #### Compatible with almost* any server.
- #### Made to be used together with discord.

## How to install:
- #### First of all clone the git repository of the project with this command:

```bash
git clone https://github.com/BrewTheFox/ReKITtyPaw.git ./ReKittyPaw
```

- #### Then change the directory to ReKittyPaw:


```bash
cd ReKittyPaw
```

- #### Install the project dependencies:


```node
npm install
```

## How to configure:
#### After you have installed the project, you should configure it in the file ./config.json. There are some important things to take into consideration.

- ## Keywords
  
  | **Keyword**        | **Replaced With**                                                     | **Used in**                                                                            |
  |--------------------|-----------------------------------------------------------------------|----------------------------------------------------------------------------------------|
  | {{User}}           | The minecraft username of the person that requested the delivery.     | UTPCancelMSG, UTPAcceptMSG, ExpiredTP, AcceptTPASK, ErrorMessage, UnstockedItemMessage |
  | {{TPAcceptTime}}   | The time that you've set on TPAcceptTime converted to seconds.        | AcceptTPASK                                                                            |
  | {{RequestID}}      | A randomly generated uuid generated after the user requested the kit. | ExpiredTP, AcceptTPASK, ErrorMessage, UnstockedItemMessage                             |
  | {{MinuteKitDelay}} | Replaced with the value of MinuteKitDelay in the config file.         | KitDelayMessage                                                                        |

- ## The example ./config.json file
  
  | **Keyword**               | **Content**                                                                                                         | **Usage** |
  |---------------------------|---------------------------------------------------------------------------------------------------------------------|-----------|
  | token                     | havfYeMZVkMmAfz0TiNmyFYcGk19rdSG1xV11NP2Cp8yP6pygeQndRLSyNezpCz0T9Y2BpDm3JwNUrFcUhuNtVVwzP3d2Rzwe6uw                |           |
  | username                  | MyNameIsBot                                                                                                         |           |
  | password                  | ThisIsMyPassword                                                                                                    |           |
  | host                      | RandomAnarchyServer.net                                                                                             |           |
  | port                      | 12345                                                                                                               |           |
  | version                   | 1.18.1                                                                                                              |           |
  | TPDelay                   | 5000                                                                                                                |           |
  | HomeDelay                 | 8000                                                                                                                |           |
  | LavaCoords                | [-14, 65, 0]                                                                                                        |           |
  | TPAcceptTime              | 15000                                                                                                               |           |
  | MaxDeliverKits            | 10                                                                                                                  |           |
  | BotOwner                  | ThisIsYourMinecraftUsername                                                                                         |           |
  | HomeMessage               | You are now in home                                                                                                 |           |
  | HomeCancelMSG             | Pending teleportation request cancelled.                                                                            |           |
  | AfterRegisterMSG          | Successfully registered!                                                                                            |           |
  | AfterLoginMSG             | You have successfully logged in!                                                                                    |           |
  | RegisterMSG               | Please use /register 'Password' 'Password' to register.                                                             |           |
  | LoginMSG                  | Welcome again. Please use /login 'Password' to start enjoying.                                                      |           |
  | UTPCancelMSG              | [RandomTPA] {{User}} cancelled your petition!                                                                       |           |
  | UTPAcceptMSG              | [RandomTPA] {{User}} Teleported to you!                                                                             |           |
  | AcceptTPASK               | You have {{TPAcceptTime}} seconds to accept your request that have the id {{RequestID}} before it cancels.          |           |
  | ExpiredTP                 | The request with the id {{RequestID}} expired.                                                                      |           |
  | UnstockedItemMessage      | One of the items that you have requested is not in stock, please try again later :(                                 |           |
  | ErrorMessage              | There was a problem delivering the kit, please try again later :(                                                   |           |
  | KitSelectionMenuTitle     | Selection Menu - Ranarchy                                                                                           |           |
  | MinuteKitDelay            | 5                                                                                                                   |           |
  | KitDelayMessage           | Hey hold on you didn't wait the {{MinuteKitDelay}} minutes delay :(                                                 |           |
  | EmbedTitle                | Request a delivery.                                                                                                 |           |
  | Embed1Title               | How to?                                                                                                             |           |
  | Embed1Content             | Just click the button down this text                                                                                |           |
  | Embed2Title               |                                                                                                                     |           |
  | Embed2Content             |                                                                                                                     |           |
  | Embed3Title               |                                                                                                                     |           |
  | Embed3Content             |                                                                                                                     |           |
  | KitMenuOpenText           | Request your kit NwN                                                                                                |           |
  | ServerRestartError        | We're sorry. Our Server restarted, please try filling the form again.                                               |           |
  | MinecraftEmptyServerError | Hey. you're not on the Minecraft Server.                                                                            |           |
  | NameAskMessage            | Now tell me. which one is your nickname?                                                                            |           |
  | GenericError              | We're sorry. there was a problem handling your request.                                                             |           |
  | VoucherText               | Thank you for using Ranarchy delivery bot. Please wait some time for the bot to be available and delivers your kit. |           |
  | KitsDict                  | {"KitOption1":"wither_skeleton_skull", "KitOption2":"detector_rail"}                                                |           |
  | RepresentativeKitEmoji    | 🍕                                                                                                                   |           |
  | SelectedKitEmoji          | 🌏                                                                                                                   |           |
  | UnSelectedKitEmoji        | 🧨                                                                                                                   |           |

