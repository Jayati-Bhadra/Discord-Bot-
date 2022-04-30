# Discord-Bot-
A Client is an object that represents a connection to Discord. A Client handles events, tracks state, and generally interacts with Discord APIs.

Here, you’ve created a Client and implemented its on_ready() event handler, which handles the event when the Client has established a connection to Discord and it has finished preparing the data that Discord has sent, such as login state, guild and channel data, and more.

In other words, on_ready() will be called (and your message will be printed) once client is ready for further action. You’ll learn more about event handlers later in this article.

When you’re working with secrets such as your Discord token, it’s good practice to read it into your program from an environment variable. Using environment variables helps you:

Avoid putting the secrets into source control
Use different variables for development and production environments without changing your code
While you could export DISCORD_TOKEN={your-bot-token}, an easier solution is to save a .env file on all machines that will be running this code. This is not only easier, since you won’t have to export your token every time you clear your shell, but it also protects you from storing your secrets in your shell’s history.

Create a file named .env in the same directory as bot.py:
