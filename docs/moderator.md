> Hello!
>
> Welcome to the Angular Community team! We are glad to have you here. You are
> helping ensure the community stays welcoming for everyone. Below, you will
> find an overview of the server and a FAQ of the most common scenarios you will
> run into.
>
> If you have any questions about the server or need help with anything, please
> do not hesitate to reach out to me or any other `@Staff` member.
>
> Sincerely,
>
> delasteve

## Preface

Before we begin, you will need to enable the `Developer Mode` feature in
Discord. You can find how to do that [here][discord-developer-mode]. This will
help ensure you're able to view user IDs in the event you have to take action
against a member who is violating our
[Code of Conduct (CoC)](../CODE_OF_CONDUCT.md) or [server rules](../README.md).
To find the ID of a user, simply right click their username and select `Copy ID`
from the menu that appears. This also works for just about everything, such as
messages, channels, and servers.

## Server Overview

Upon receiving the `@Moderator` role, the first thing you'll notice is two new
categories, `Logs` and `Private`.

In the `Logs` category, you will notice quite a lot of channels. As the name
implies, these are set up for logging purposes. Hopefully, we will never need to
use them, but they prove invaluable when we do. It's recommended to either mute
the entire category or individual channels, depending on your preference, then
collapse the category.

The `Private` category is where we chat amongst the other team members. Some
team members have notifications on for all messages sent to a channel,
specifically `#moderator-chat`. You're not required to do the same, but please
be mindful of what channel you're sending messages in.

Our moderation bot, `@Gaius Cicereius+`, takes care of most of the heavy
lifting. It has the ability to filter unwanted words, check user profiles,
reaction roles, and more. The documentation for the bot can be found
[here][gaius-documentation].

Our other bot, `@Statbot`, is a simple analytics bot. Its main goal is to keep
track of the activity in certain channels. This will become helpful if we ever
reach a point where we have too many channels and need to prune unused or
unmaintained channels. Our analytics are public and can be found
[here][statbot-analytics].

All bot commands should be used in the `#bot-commands` channel. This way we can
keep the spam the bots' spam isolated from our actual private moderation
channels.

## FAQ

> A user wants to opt-out of analytic collection from `@Statbot`. What do I tell
> them to do?

Direct them to send a DM the Statbot with the command `s?userprivacy on` and
then type `accept` to the "Are you sure" message that follows.

> A word was caught in the filter that should be allowed. How do I fix this so
> that it won't be caught in the future?

First, test the filter in `#bot-commands` using the command
`g!testword <word-or-phrase>`. The bot will respond with the filter that caught
it. Copy the "word found", use the command `g!unbanword <word>`, and finally
edit the filter as appropriate using `g!banword <word> <variables>`. More
information on filters can be found [here][gaius-ban-word].

> What is our policy on moderating users that are acting out of line?

Our policy is a verbal warning, a bot warning, a 24 hour mute, then a permanent
ban. The last three are automatically handled by the bot. First, check the users
warning history by using the command `g!rapsheet <userId>`. This will bring up
the user's history with our server and any moderation actions that have taken
place. If a verbal was already given, use the command `!warn <userId> reason`.
The bot will choose the appropriate moderation action to take. If the next
action will be a permanent ban, please consult with `@Staff` members as we have
to report the action to the Angular team.

<!--
References
-->

[discord-developer-mode]:
  https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-
[gaius-documentation]: https://docs.gaiusbot.me/books/gaius
[gaius-ban-word]: https://docs.gaiusbot.me/books/gaius/page/banned-words
[statbot-analytics]: https://statbot.net/dashboard/748677963142135818
