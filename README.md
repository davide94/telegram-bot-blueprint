# telegram-bot-blueprint

A template repository to quickly create and deploy (on AWS) a telegram bot.

## Set Up

Once you created a bot with https://t.me/BotFather and retrieved the API key

- Create a `.env` file like:
  ```
  TELEGRAM_API_TOKEN=<YOUR_TELEGRAM_TOKEN>
  ```
- Install requirements by running:
  ```
  $ npm i
  ```
- _If not already done, configured your AWS cli credentials https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html_
- Deploy by running:
  ```
  $ sls deploy
  ```
- Submit your webhook to telegram by running:
  ```
  $ npm run set-webook --token=<YOUR_TELEGRAM_TOKEN> --url=<YOUR_WEBHOOK_URL>
  ```

Great! the bot is live and will reply to your messages.

##

It's now time to have fun with **the actual implementation**.
