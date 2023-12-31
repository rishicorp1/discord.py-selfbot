# Discord.py-Selfbot

This is a [Python](https://www.python.org)-based Discord selfbot using the `discord.py-self` library. The selfbot automatically responds to messages that uses it's trigger word using either ChatGPT or BARD and has image generation using an external endpoint, **all for completely free**. It functions as a normal Discord bot, just on a real Discord account, allowing other people to talk to it within DMs, servers and even group chats without you needing to invite a bot or add the bot to the server - making it seem like a real user to others.

This bot was originally [Discord-AI-Chatbot](https://github.com/mishalhossin/Discord-Chatbot-Gpt4Free/) by [MishalHossin](https://github.com/mishalhossin/) but was heavily edited by [Najmul190](https://github.com/najmul190) to work as a selfbot rather than a Discord bot.After that it was heavily edited by [rishicorp1](https://github.com/rishicorp1) !!
### <strong> This repositry is for educational purpose</strong>
### <strong> I take no responsibility for any actions taken against your account for using these selfbots, or how users use my open source code.</strong>

### <strong>Using this on a user account is prohibited by the [Discord TOS](https://discord.com/terms) and can lead to your account getting banned in very rare cases.</strong>
# Preview of image responses:

![image](https://user-images.githubusercontent.com/91066601/236717834-e3f6939f-3641-425c-b9f7-424a38f86ac4.png)

# Preview of text responses:

![image](https://media.discordapp.net/attachments/1158446581721337877/1162558351385833563/image.png?ex=653c5fd6&is=6529ead6&hm=244175cda74c02f8dac556a36dd8a3fb7e9885e3d54a09a653cfb813bb037d58&=)

# Preview of Image Generation:

![image](https://cdn.discordapp.com/attachments/1157235534641496084/1162554826715054110/image.png?ex=653c5c8d&is=6529e78d&hm=e0899c3c597ee464233fbaa726878b4f1a4523535283357ac37eca2f49b40115&)

## Recommended IDE: PyCharm

We highly recommend using PyCharm as the integrated development environment (IDE) for this project. PyCharm offers a range of features that can greatly enhance the development process, including powerful code navigation, intelligent code completion, and excellent debugging capabilities.

To get started, you can download PyCharm from [here](https://www.jetbrains.com/pycharm/). Once installed, open the project folder in PyCharm to start working on it.

# Features

- [x] Discord Selfbot: Runs on a genuine Discord account, allowing you to use it without even needing to invite a bot.
- [x] Free LLM Model: Enjoy the powerful capabilities of this language model without spending a dime.
- [x] Mention Recognition: The bot always responds when you mention it or say its name.
- [x] Reply Recognition: If replied to, the bot will continue to reply to you. It's like having a conversation with a real person!
- [x] Message Handling: The bot knows when you're replying to someone else, so it won't cause confusion. It's like having a mind reader in your server; It can also handle numerous messages at once!
- [x] Channel-Specific Responses: Use the `~toggleactive` command to pick what channel the bot responds in.
- [x] Psychoanalysis Command: Use the `~analyse` command to analyse a mentioned user's messages and find insights on their personality. It's like having a therapist in your server!
- [x] GPT-3.5-Turbo Model: This bot runs on turbo power! Powered by the lightning-fast GPT-3.5-Turbo language model.
- [x] Image Generation: Use the `~imagine` command to generate an ima-rom a prompt using AI.
- [x] BARD Model: Select the BARD model to start using Google's own model, which has up-to-date information and is more accurate, but cannot hold a conversation as well as ChatGPT or follow instructions.
- [x] Secure Credential Management: Keep your credentials secure using environment variables.
- [x] Other fetures you can see in commands.
- [x] Crafted with Care: Made with lots of love and attention to detail.

# Bot Commands

Welcome to the world of endless possibilities! Here are the commands at your disposal:

- `~pfp [image_url]` - Change the bot's profile picture 
- `~wipe` - Clears history of the bot
- `~ping` - Shows the bot's latency
- `~scrap` - Get transcript of the channel
- `~toggleactive` - Toggle the current channel to the list of active channels
- `~toggledm` - Toggle if the bot should be active in DM's or not
- `~togglegc` - Toggle if the bot should be active in group chats or not
- `~ignore [user]` - Stop a user from using the bot
- `~imagine [prompt]` - Generate an image from a prompt
- `~analyse @user` - Analyse a user's messages to provide a personality profile
- `~model [BARD / GPT]` - Change whether the bot uses BARD or ChatGPT
- `~bal (Ltcaddress)` - Fetch the balance of ltc address
- `~ltc` - Know the latest price of ltc
- `~readtext` - Read the letter written on image and send it 
- `~sexw` - Get nsfw using waifu
- `~sext` - Get nsfw of trap
- `~copyserver [source_server id] [target_SERVER ID]`  - It copies the server you need but it needs admin in target server
- `~imgs` - Search in google image and send 
- `~gits` - Find github users and repositories
- `~spam t + m` - Use this to spam messages
- `~ping` - Shows the bot's latency


# Steps to install and run:

### Step 1: Git clone repository

```
git clone 
```

### Step 2: Changing directory to cloned directory

```
cd discord.py-selfbot
```

### Step 3: Getting your Discord token

- Go to [Discord](https://canary.discord.com) and login to the account you want the token of
- Press `Ctrl + Shift + I` (If you are on Windows) or `Cmd + Opt + I` (If you are on a Mac).
- Go to the `Network` tab
- Type a message in any chat, or change server
- Find one of the following headers: `"messages?limit=50"`, `"science"` or `"preview"` under `"Name"` and click on it
- Scroll down until you find `"Authorization"` under `"Request Headers"`
- Copy the value which is yor token

### Step 4: Get your BARD cookie value

- Go to [Google's BARD website](https://bard.google.com)
- Click `Sign in` or `Try it`
- Press `Ctrl + Shift + I` (If you are on Windows) or `Cmd + Opt + I` (If you are on a Mac).
- Go to the `Application` tab
- Click on `Cookies` under `Storage` on the left side
- Click on `https://bard.google.com` under `Cookies`
- Copy the value of `__Secure-1PSID` and paste it in the `.env` file under `BARD_COOKIE`

![image](https://media.discordapp.net/attachments/918997350238797855/1129414138347651122/image.png?width=481&height=357)

### Step 5: Rename `example.env` to `.env` and put the discord token and BARD cookie. It'll look like this:

```
BARD_COOKIE=BARD_COOKIE_GOES_HERE
DISCORD_TOKEN=DISCORD_TOKEN_GOES_HERE
OWNER_ID=OWNER_ID_GOES_HERE
SELFBOT_ID=ACCOUNT_ID_GOES_HERE
TRIGGER=TRIGGER_WORD
PREFIX=~
```
# How to run on Mobile + Keep online 24/7

[![Run on repl.it]()]()

- Click on the button above to create an account and run the bot on repl.it
- Click on `Import from GitHub`
  ![image]()
- Do Step 3 and 4 from above to get the information
- Add the following as a secret each, along with the corresponding value: (trigger value should not be in quotes)

```
BARD_COOKIE
DISCORD_TOKEN
OWNER_ID
SELFBOT_ID
TRIGGER
PREFIX
```

![image]()

- Then click on the `Run` button, which will start to install all dependencies and then run your selfbot.
- Start talking to your new friend!

- To run it 24/7, use [UptimeRobot](https://uptimerobot.com/).

# How to talk to the bot

- To activate it in a channel use **~toggleactive** in the channel or manually add the channel ID in `channels.txt`
- To see all commands use **~help**
- Bear in mind that the bot will only respond to **other accounts** and not itself, including any commands.
- You must also set a trigger word within the `.env`, this is the word that the bot will respond to. For example, if you set the trigger word to `John`, people must say "Hey `John`, how are you today?" for the bot to respond.
- IF YOU WANT TO MAKE MORE CHANGES YOU CAN DO IN INSTRUCTIONS.TXT IT HELPS TO CUSTOMISE BOT BEHABIER
"# discord.py-selfbot"

# Cool Contributions Always Welcome! 🚀

Welcome to our open-source project! We appreciate your interest and encourage you to contribute. Whether it's code, bug reports, feature suggestions, or documentation improvements, your input is valued.

## How to Contribute

1. Fork the repository
2. Create a new branch (e.g., `feature-new-feature`)
3. Make your changes and commit them
4. Push to your branch
5. Create a pull request

Happy coding! 🎉

