You can host modmail bot for your server on replit.com 24/7 for free without credit card! Just follow this guide. 
Modmail bot wiki: https://github.com/kyb3r/modmail/wiki


- Create account on https://repl.it/signup
- Create a bot from Discord dev portal and invite it to your Discord server- [guide](https://github.com/kyb3r/modmail/wiki/Installation#2-discord-bot-account)
- Create MongoDB Atlas database - [guide](https://github.com/kyb3r/modmail/wiki/Installation-(cont.)#installation-continued) 
 ## Deploying the Log Viewer
 We will need MongoDB connection string.
 - Fork logviewer repl [here](https://replit.com/@modmailsetup/logviewer)
 - Go to Secrets tab and add there:
    * `MONGO_URI` - Your Mongo connection URI
 
 - Click on Run button and wait!
 - Copy your logviewer's url, you will need it later
    
## Deploying the Modmail bot
 - Fork modmail repl [here](https://replit.com/@modmailsetup/modmail)
 - Go to Secrets tab and add there:
    * `TOKEN` - your [bot's token](https://github.com/kyb3r/modmail/wiki/Installation#creating-a-bot-account)
    * `GUILD_ID` - [ID of your Server](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-)
    * `OWNERS` - your own Discord ID, if there are multiple owners, separate them by a comma like this: `180314310298304512, 355790471219511297, 325012556940836864`.
    * `CONNECTION_URI` - your Mongo connection URI from the previous section
    * `LOG_URL` - URL of your logviewer repl (`https://logviewer.<your_username>.repl.co`)
    * `disable_autoupdates` - `on` (This will prevent the bot from making auto updates, if you skip this, then your bot will be broken. If there is a new update, please fork my repl again and fill the same Secrets and then delete your old repl and rename new repl to the same name as it was before. *You can ping me on Pinglik Support server if I haven't updated my repl.*)

- Click on Run button and wait
- Copy your modmail bot's webserver url
- 🎉 Your modmail bot should be online now, try to run `?setup` command on your Discord server.

## Keeping Modmail bot + logviewer alive
If you will skip this step your modmail will go offline after 30 minutes of inactivity (when you leave replit project's page).
So we will need logviewer's url and modmail webserver's url

- You can use Uptime robot. It will ping your replit projects to keep them online for free.


**Uptime Robot**: [Click here](https://uptimerobot.com)



### That's all.

If you need help you can open new modmail support thread on [BubbleGum Cafe Server](https://its.ventispurr.xyz/bubblegumcafe) and we will help you 😉
