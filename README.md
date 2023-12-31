
# JavaScript Discord Bot 
![Discord Bot](https://github.com/Nyaundi/JavaScript-Discord-Bot/)

This tutorial will guide you through the process of creating a Discord bot using JavaScript and hosting it for free on platforms like Heroku or Glitch. Discord bots can add fun and useful features to your server, making your community more engaging and dynamic.

## Prerequisites
Before you start, make sure you have the following prerequisites:

- [Node.js](https://nodejs.org/) installed on your computer.
- A [Discord account](https://discord.com/).
- Create a Discord application and bot on the [Discord Developer Portal](https://discord.com/developers/applications).
- Invite your bot to a server with the necessary permissions.

## Step 1: Setting Up Your Project
1. Create a new directory for your project.
2. Open your terminal and navigate to the project directory.
3. Initialize a Node.js project by running:

```shell
npm init -y
```

4. Install the necessary packages:

```shell
npm install discord.js
```

## Step 2: Creating the Bot
1. Create a new JavaScript file, for example, `bot.js`.
2. Write your bot's code using the `discord.js` library. You can find an example bot code in [example-bot.js](example-bot.js) in this repository.

## Step 3: Adding Your Bot Token
1. Go to the [Discord Developer Portal](https://discord.com/developers/applications) and click on your application.
2. Go to the "Bot" tab and copy your bot's token.
3. In your `bot.js` file, add the following line at the top:

```javascript
const { Client, GatewayIntentBits } = require('discord.js');
const client = new Client({
  intents: [
    GatewayIntentBits.Guilds,
    GatewayIntentBits.GuildMessages,
    GatewayIntentBits.GuildMessageReactions,
  ],
});
const token = 'YOUR_BOT_TOKEN';
```

Replace `'YOUR_BOT_TOKEN'` with your bot's token.

## Step 4: Running Your Bot
1. In your `bot.js` file, add the following code to log in your bot:

```javascript
client.login(token);
```

2. In your terminal, run your bot using:

```shell
node bot.js
```

Your bot should now be online and operational in your Discord server.

## Step 5: Hosting Your Bot
You can host your bot for free on platforms like Heroku or Glitch. Refer to the following guides:

- Hosting on Heroku: [Heroku Hosting Guide](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- Hosting on Glitch: [Glitch Hosting Guide](https://glitch.com/help/kb/article/21-how-do-i-add-an-existing-express-js-app-to-glitch/)

## Conclusion
Congratulations! You've created a Discord bot using JavaScript and learned how to host it for free. You can now expand your bot's capabilities by adding more commands and features.

## Resources
- [Discord.js Documentation](https://discord.js.org/)
- [Discord Developer Portal](https://discord.com/developers/applications)

If you have any questions or need further assistance, feel free to ask for help on the [Discord.js official server](https://discord.gg/bRCvFy9).

Don't forget to customize your bot, add new commands, and make it a valuable addition to your Discord community. Happy coding! 🤖🚀

---
Feel free to customize this README with your specific project details, and don't forget to include your bot's icon and replace `'YOUR_BOT_TOKEN'` with your actual bot token.
