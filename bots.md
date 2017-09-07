# Bot Development Guidelines
We're a community of programmers, and as such we rely pretty heavily on bots.
We can proudly say that all of the bots in our server are home-made, but as the number of bots increases we need to set up some rules to keep things from going out of hand.
Below is a list of what we expect from the bots in our server, and what we'd like you to think about if you're developing a bot for us.

## Interface
To avoid the problem of figuring out which bot should respond to the message `!help`, we ask that each bot uses `@mention`s to differentiate when a command is addressed to it.

If your bot gets tagged in a message, that message is for your bot.
If the message is a valid command, we would like your bot to respond to it.
If the message is an invalid command, we would like your bot to print its usage information so that the user can send a valid command next time.

If your bot doesn't get tagged in a message (unless your bot is designed to listen to everything) then that message probably isn't for your bot.
Please don't respond to it.

Also, just to avoid the possibility of infinite loops, please ensure your bot ignores messages from other bots (including itself).

To keep some consistency between all the bots in our server, we have a short list of generic commands that each bot should be able to respond to.

### `@yourbot help`
This should print the help information for your bot.
This is where you explain what your bot does, why it does it, and how people can learn more about what your bot does.

### `@yourbot usage`
This should print the _usage_ information for your bot.
This should not be a block of text.
Keep this short and sweet - just a list of "command -> one line description" is enough.

### `@yourbot source`
We all like open source software.
It helps people to trust what the bots in their channels are doing, and it makes life easier if people want to help add features to your bot.
If you're able to open source your bot, please do so, and then reply to this command with a link to your source code.
If you're not able to open source your bot for whatever reason, that's okay, but make sure your bot explains that in response to this command.

### `@yourbot author`
This one's pretty simple.
Let us know who you are.
We've put this in here so we can build a community of bot developers, and also so people know who to talk to about feature requests / bug reports.

## General Rules
The bots in our server are here to make things better for us as a community.
We aren't going to put strict, black-and-white limits on what we do and don't accept, but please keep that in mind when you're designing bots.

Each bot should respect the privacy of people in the server, and should not be built to offend or hurt.
Please don't write bots that spam, and try to avoid writing bots that encourage other people to spam.

## Bot Testing
We've got a `#bot-testing` channel set up.
Ask a moderator or admin if you'd like to join.
We have a bunch of people that have made bots before, and can help you out.
We also can supply you with bot tokens for testing within that sandboxed channel.
Once your bot is ready, let us know and we can send it out to the rest of the server.

## Getting Your Bot into Our Server
So you've written a bot - it follows all the above guidelines, and you're ready to deploy it.
First of all, **congratulations**!
By this stage a few admins will have probably seen your bot (most of us are bot developers ourselves) and will have spoken to you about moving it into the server as a whole once its ready.
But if we haven't, or you'd like to know in advance, it works a little like this.

Each deployed bot gets its own user account within our server.
You can make that account yourself, or if you want we can help make it for you and supply you with the token for it.
Your bot is going to have its own role that we use to control its permissions, and then it will be a part of the `bots` role so that it gets grouped nicely with the other bots in the discord sidebar.

When we're ready to add your bot to the server, tell us exactly what permissions your bot is going to need.
We operate this server on a minimum permissions system (out of habit) so the more accurately you can tell us what your bot needs to be able to do the better we will feel inside as admins.
Once its set up, that's pretty much it.
If your bot starts acting up we will either remove permissions or remove your bot.
If you add new features that require extra permissions let us know and we'll probably give them to your bot.

## Conclusion
If you've got a good idea for a bot, or even if you don't but you'd just like to learn how bot development works, we'd love to hear from you.
Over in `#bot-testing` we have quite a few people who have made bots before and are more than happy to help out (including myself).

Best of luck with all your bot adventures!

Sincerely,

`@artemis` and the rest of the CSST admin team.
