# <img src="https://simpleicons.org/icons/telegram.svg" height="30px" width="30px"> &nbsp;TiTAN

The telegram bot you dream of the whole time.

![Status](https://img.shields.io/badge/status-offline-red)
![Commands](https://img.shields.io/badge/commands-69-red)
![Latest update](https://img.shields.io/badge/latest%20update-2%20hours%20ago-green)
![Uptime](https://img.shields.io/badge/uptime-0%20minutes-yellow)

[German version](https://github.com/aarivex/titanbot-telegram/blob/master/README_German.md)

# :jack_o_lantern: Introduction
TiTAN is a bot designed to provide you with not only entertaining and funny, but also helpful commands that ease up a lot of stuff. From downloading youtube videos directly onto your phone to having reddit media and memes delivered right to your favorite group chat without the hassle of sharing links, TiTAN has got you covered.

The bot is private, meaning its only available for whitelisted users. It'll most likely be available for a subscription soon, but the bot is in a early testing stage currently.

If you're excited and wish to help out, hit me up at [aarivex.dev](https://aarivex.dev) or Telegram (@canathan).  
You can always suggest features or give feedback.

# :ghost: Bug reports
If you've encountered a bug or error, we'd suggest you to use the [Issues](https://github.com/aarivex/titanbot-telegram/issues) page to report any malfunction.

# Technical stuff
The bot is written in the beautiful C# language and built, ran and maintained on the lovely .NET Core 3 runtime. Our main focus is stability and a great user experience. :heart:

#  List of commands
| Command | Description | Usage |
| ------- | ----------- | ----- |
| /toggle **!** | Toggle specific rules. | /toggle ``<rule>`` |
| /about | About this bot. | /about |
| /test | A pretty neat test command. :D | /test |
| /youtube **!** | Download or search youtube videos. The video is downloaded and sent directly as media. | /youtube ``<link>`` **\|** ``<search>`` (``<number>``) |
| /lyrics **!** | Get the lyrics for a song. | /lyrics ``<song title>`` |
| /reddit **!** | Random reddit post from a specified or random subreddit. | /reddit (``<subreddit>``) (``<media type (image\|video\|gif)>``) |
| /weather **!** | Get weather info for a city. Default country is Germany. | /weather ``<postal code\|city>`` (``<country code>``) |
| /motivation **!** | Get motivational images from /r/GetMotivated. | /motivation |
| /r34 **!** | Get rule34 content. ( ͡° ͜ʖ ͡°)<br>If executed in a group, every member must have enabled nsfw. | /r34 (``<tags[]>``) |

Commands marked with ``!`` are upcoming commands that are not available yet.  
``^`` indicates a command in beta with the given possibility of unstability.  

If a usage identifier has a ``[]`` (for example ``<tags[]>``), the argument supports more than one term, like ``/cmd tag1 tag2 tag3..``.  
Identifiers inside brackets ``(<something>)`` are optional arguments, making the command use its defaults if not specified.

# Rules
| Rule | Description | Default |
| ---- | ----------- | ------- |
| nsfw | Enable NSFW content. If disabled, you won't receive NSFW-content from any command.<br>_This needs to be enabled in order to execute the r34 command in groups._ | Yes |
| largefiles | Enable acceptance of large files and media. Disable this if you want to _save data_.<br>Useful for media-related commands like reddit. | Yes |

Non-whitelisted users can still toggle rules.

# Config
| Config | Description | Example value |
| ------ | ----------- | ------------- |
| reddit.subs | Grab posts from one of the specified subreddits when using the reddit command without a specified sub. | ``ProgrammerHumor,csharp,dotnet,gifs,dashcamgifs`` |
| weather.region | Default region (postal code or city) for the weather command. If specified, the weather command can be used without arguments. | ``Berlin``
| weather.country | Default country for the weather command. | ``Germany``
