![Hummingbot](https://i.ibb.co/X5zNkKw/blacklogo-with-text.png)

----
[![License](https://img.shields.io/badge/License-Apache%202.0-informational.svg)](https://github.com/hummingbot/hummingbot/blob/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/follow/hummingbot_io.svg?style=social&label=hummingbot)](https://twitter.com/hummingbot_io)
[![Discord](https://img.shields.io/discord/530578568154054663?logo=discord&logoColor=white&style=flat-square)](https://discord.gg/hummingbot/)
[![Discourse](https://img.shields.io/discourse/https/hummingbot.discourse.group/topics.svg?style=flat-square)](https://hummingbot.discourse.group)

Hummingbot is an open source client-side framework that helps you build, manage, and run automated trading strategies, or **bots**. This code is free and publicly available under the Apache 2.0 open source license!

## Elixir protocol fork

This fork implements support for working with a custom data feed provided by Elixir protocol, right now users can test a local datafeeds service running on 0.0.0.0:5000 (this is set hummingbot/hummingbot/connectors/elixir/elixir_constants.py).

After installing hummingbot from this source following the official documentation, you can test running hummingbot with elixir datafeeds:
```shell
bin/hummingbot.py

# Run the following command inside hummingbot client UI.
config elixir_protocol_exchange # This will prompt for a exchange that elixir supports.
```

You can set `elixir_protocol_exchange` manually as well in your respective config yml file. Right now only BINANCE is supported.

Then you should create a new strategy with your bot, you can try with pure_market_making, and when choosing an exchange after you are prompted "Enter your maker spot connector during the creation of the strategy." just enter `elixir_paper_trade`.

## Getting Started

- [Website](https://hummingbot.org)
- [Docs](https://hummingbot.org/docs)
- [FAQs](https://hummingbot.org/faq/)
- [Installation](https://hummingbot.org/installation/)
- [Developers](https://hummingbot.org/developers/)

### Community

- [Discord](https://discord.gg/hummingbot)
- [Youtube](https://www.youtube.com/c/hummingbot)
- [Twitter](https://twitter.com/hummingbot_io)
- [Reddit](https://www.reddit.com/r/Hummingbot/)
- [Forum](https://hummingbot.discourse.group/)

## Other Hummingbot Repos

- [Hummingbot Site](https://github.com/hummingbot/hummingbot-site): Official website and documentation for Hummingbot - we welcome contributions here too!
- [Hummingbot Project Management](https://github.com/hummingbot/pm): Agendas and recordings of regular Hummingbot developer and community calls
- [Awesome Hummingbot](https://github.com/hummingbot/awesome-hummingbot): All the Hummingbot links
- [Hummingbot StreamLit Apps](https://github.com/hummingbot/streamlit-apps): Hummingbot-related StreamLit data apps and dashboards

## Contributions

Hummingbot belongs to its community, so we welcome contributions! Please review these [guidelines](./CONTRIBUTING.md) first.

To have your pull request reviewed by the community, submit a [Pull Request Proposal](https://snapshot.org/#/hbot-prp.eth) on our Snapshot. Note that you will need 1 HBOT in your Ethereum wallet to submit a Pull Request Proposal. See https://www.coingecko.com/coins/hummingbot for markets where HBOT trades.

## Legal

- **License**: Hummingbot is licensed under [Apache 2.0](./LICENSE).
- **Data collection**: read important information regarding [Hummingbot Data Collection](./DATA_COLLECTION.md).
