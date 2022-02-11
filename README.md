
# Online-Forever
Make your Discord Account Online 24/7!

----

A Code written in Python that helps you to keep your account 24/7.

The [main.py](https://github.com/EZiskpsy05/Lots-of-Discord-bot-/blob/Self-bot-24/7/main.py) is the main file. [keep_alive.py](https://github.com/EZiskpsy05/Lots-of-Discord-bot-/blob/Self-bot-24/7/keep_alive.py) prevents your repl from going to sleep. (If you have a replit hacker plan, then you can delete [this file](https://github.com/EZiskpsy05/Lots-of-Discord-bot-/blob/Self-bot-24/7/keep_alive.py) and paste this code inside the [main.py](https://github.com/EZiskpsy05/Lots-of-Discord-bot-/blob/Self-bot-24/7/main.py) file : 

</br>

```py
import discord
import os
from discord.ext import commands

client = commands.Bot(command_prefix=':', self_bot=True, help_command=None)

async def on_ready():
  await client.change_presence(status=discord.Status.online, activity=discord.Game("TESTING"))

client.run(os.getenv("TOKEN"), bot=False)
```

This Code is from [this tutorial](https://youtu.be/yfgEbZAXMAQ).
