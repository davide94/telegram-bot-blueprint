# telegram-bot-blueprint

A template repository to quickly create and deploy (on AWS) a telegram bot.

## Set Up

Once you created a bot with https://t.me/BotFather and retrieved the API key

* Create a `.env` file like:
  ```
  TELEGRAM_API_TOKEN=<YOUR_TELEGRAM_TOKEN>
  ```
* Install requirements by running:
  ```
  $ npm i
  ```
* *If not already done, configured your AWS cli credentials https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html*
* Deploy by running:
  ```
  $ sls deploy
  ```
* Update the `set-webhook` script in `package.json` by replacing `<TELEGRAM_TOKEN>` with the actual token and `ENDPOINT_URL` with the URL output by the deploy command

* Run `npm run set-webook`

Great! the bot is live and will reply to your messages.

##

It's now time to have fun with **the actual implementation**.
