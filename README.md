<p align="center">
    <a href="https://github.com/pyrogram/pyrogram">
        <img src="https://i.imgur.com/BOgY9ai.png" alt="Pyrogram">
    </a>
    <br>
    <b>Telegram MTProto API Framework for Python</b>
    <br>
    <a href="https://docs.pyrogram.org">
        <b>Documentation</b>
    </a>
    •
    <a href="https://github.com/pyrogram/pyrogram/releases">
        <b>Releases</b>
    </a>
    •
    <a href="https://t.me/Pyrogram">
        <b>Community</b>
    </a>
</p>

## Pyrogram

``` python
from pyrogram import Client, filters

app = Client("my_account")


@app.on_message(filters.private)
async def hello(client, message):
    await message.reply_text(f"Hello {message.from_user.mention}")


app.run()
```

**Pyrogram** is an elegant, easy-to-use [Telegram](https://telegram.org/) asynchronous framework written from the
ground up in Python and C. It enables you to easily create custom apps for both user and bot identities
(bot API alternative) via the [MTProto API](https://core.telegram.org/api#telegram-api).

### Features

- **Easy**: You can install Pyrogram with pip and start building your applications right away.
- **Elegant**: Low-level details are abstracted and re-presented in a much nicer and easier way.
- **Fast**: Crypto parts are boosted up by [TgCrypto](https://github.com/pyrogram/tgcrypto), a high-performance library
  written in pure C.
- **Documented**: Pyrogram API methods, types and public interfaces are well documented.
- **Type-hinted**: Exposed Pyrogram types and method parameters are all type-hinted.
- **Updated**, to make use of the latest Telegram API version and features.
- **Bot API-like**: Similar to the Bot API in its simplicity, but much more powerful and detailed.
- **Pluggable**: The Smart Plugin system allows to write components with minimal boilerplate code.
- **Comprehensive**: Execute any advanced action an official client is able to do, and even more.

### Requirements

- Python 3.6.0 or higher.
- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).

### Installing

``` bash
pip3 install pyrogram
```

### Copyright & License

- Copyright (C) 2017-2020 Dan <<https://github.com/delivrance>>
- Licensed under the terms of the [GNU Lesser General Public License v3 or later (LGPLv3+)](COPYING.lesser)
