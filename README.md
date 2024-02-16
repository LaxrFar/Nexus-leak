# Nexus ( Xvirus ) ( exitscam ) ( skid )

## Installation

Install [pip](https://pip.pypa.io/en/stable/) to install modules

```bash
pip install -r requirements.txt
```

## How to use

```python
python gui.py
```

## Why did Cyprian leak?

Cyprian leaked Nexus because dexv was using me for the "custom packer" made by eintim. He was using Cyprian for everything. Another reason why Cyprian leaked was because he thinks raiding is really cringe now. Cyprian only made 2 functions (because Cyprian didn't wanna do more).

## Captcha Solver

The captcha solver was a [2captcha](https://2captcha.com/) admin api key. The key is `f86fe003c5bc005f93a7516e2973658c`

# Nexus Breakdown
Nexus raider consists of four components:

Core 1: plugins - proprietary components : primary utilities, Config, Logging, Headers, Session, Scraper and Websocket.

Core 2: Functions - Discord API edpoints + User Input + Threading.

Core 3: Bypasses - Various bypasses for example Wick verify bypass, Restorecord, Sledge Hammer and Server Rules.

Core 4: Solvers - Solver apis like Hcoptcha, Capsolver.

The main.py imports should be compiled in the order described.

# Nexus Session Breakdown
Nexus session system consists of three components:

1. Headers Number 1 - iOS Mobile: [
   * gets the app version through [Discord App (App Store)](https://apps.apple.com/us/app/discord-chat-talk-hangout/id985746746)
   * uses the app version to get the build number from the latest manifest [discord.com/ios/(app_version)/manifest.json](https://discord.com/ios/206.0/manifest.json)
   * utilizes **uuid** package to randomize the vendor id and the iphone module
   * builds the x_super_properties using the previous gathered information
   * and then fnally returns the freshly built headers
   
   ]

   Headers Number 2 - Windows Client: [
   * gets the native build version through [updtes.discord.com](https://updates.discord.com/distributions/app/manifests/latest)
   * gets the main build version from [discord.com/api/downloads/distributions/app/installers/latest](https://discord.com/api/downloads/distributions/app/installers/latest)
   * gets the page [discord.com/app](https://discord.com/app) and uses the **re** package to find the client build number in the page
   * builds the x_super_properties using the previous gathered information
   * and then fnally returns the freshly built headers
     
   ]
    

1. Tls_session: utilizes **tls_client** to make a secure connection.

2. Cookies: uses the current session to get the cookies from [discord.com](https://discord.com) and them uses them as the session cookies

Finally it uses one of the headers to send requests to the discord API very securely

## Credits

### [The biggest skid](https://dexv.lol)
### [Cyprian](https://discord.gg/hbh) (Gay)
