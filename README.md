# RustBotPy

The Rust server's bot, rewritten in Python on top of discord.py: command cogs, guild
configuration and caches, with everything the bot needs read from `config.json`.

## How to run

Create a `.env` file like so:

```bash
DISCORD_TOKEN=<token here>
```

Then run the following commands:

```bash
 docker build -t rustbotpy -f Containerfile .
 docker run --rm --name rustbotpy --env-file .env rustbotpy
```

Running it outside a container works the same way — `python runner.py` with the token in
the environment — but the container is how it has been deployed.
