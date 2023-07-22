Set Up Telegram Bot:
Go to Telegram and search for the "BotFather" bot.
Start a chat with BotFather and create a new bot by following the instructions.
Once created, BotFather will provide you with an API token for your bot. Save this token as you'll need it later.

Create an AWS Lambda Function:
Go to the AWS Management Console and navigate to the Lambda service.
Click on "Create function" and select "Author from scratch."
Give your function a name, choose the runtime as "Python 3.7".
CLick on 'create function'

Set Up API Gateway:
To make your Lambda function accessible via HTTP requests, create an API Gateway.
In the AWS Management Console, navigate to API Gateway.
Create a new API and define a resource and method (POST) that will trigger your Lambda function.
Use postman to create and setup the webhook.
code for setup of webhook is as follows:
https://api.telegram.org/bot{HTTP Token}/setWebhook

Writing the Lambda Function Code:
In the Lambda function's configuration page, scroll down to the "Function code" section.
Code file has been provided.
Format the data in a way you want to send it back to the Telegram bot.
Deploy the changes.

Now type any url in the telegram bot you created.
It will return a shortened URL
The logs for this can be checked using cloudwatch in AWS.


