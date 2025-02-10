+++
date = '2025-02-10T18:02:49+01:00'
title = 'A Finance Data Harvesting Library'
author = "Felipe Torres González"
description = "I've wrote a new library in Rust to harvest financial data from web sites into a database."
categories = ['shortbot']
tags = ['shortbot', 'programming']
toc = true
+++

I'm very pleased to announce the release of the (humble) version **v0.1.0** of a new Rust library that I'm developing: **The Rust Finance Data Harvest Library**.

This is a library that I plotted to start developing in early 2024, but had to postpone it in order to focus on other more pressing projects. Fortunately, I've finally had enough time to start developing it, and I'm really excited about its first public release.

# What's For?

In early 2024 I started to focus on short selling stocks, actually futures using CFDs, as I wanted to take advantage of a fact which is know by a financial markets adage: _Bulls take the stairs, bears take the lift_. During my early years as an investor, I was feeling frustrated when a plunge happened either to the whole market or to any of the stocks that I had in my portfolio.

A lot of people complain bitterly about short sellers and hedge funds, as did I. But eventually I realised that they are actually necessary to keep the market healthy. And sometimes they offer great opportunities to make money.

So instead of fighting against them (figuratively, I certainly can't do that), I decided to _join_ them. I decided to become a _carrion bird_. 

Hedge funds spend a lot of money and resources researching and finding weak stocks that are overvalued or are likely to fall due to some event. 

Thanks to regulators, these hedge funds are forced to report their short positions against a company's shares when the position exceeds certain threshold. In the European regulation, the threshold is set at the 0.5% of the company's value. Funds must report whenever the position goes up or down by 0.1%. And they are required to report such short positions within 24 hours at the latest. The complete information about that regulation for Europe can be found in this [link](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:02012R0236-20240116).

That's a really interesting information to benefit from, however I found that the access to the information is really cumbersome, so in practice it's really difficult to benefit from it.

**Here it when it comes the idea of developing a data harvest library to automate the extraction of such information and push it into a private database.**

# Goal

The ultimate goal is to have enough information to make an analysis between a stock's price movement and the movement of short positions. However, this is a complex task, so I have decided to start simple and get more complicated over time.

So the first thing you could do with this information would be to avoid opening long positions when a company's shares are under heavy short pressure. And wait until that pressure seems to be easing.

To achieve this, I planned two main modules:

1. A module that would automate the retrieval of information from the official website.
2. A front-end module that would present the information in a handy way.

# Short Information Data Harvesting

The first item of the list was covered by the library presented in this post. However, as I started to design it, I realised it would take a considerable amount of effort to properly develop it. Then I took the decision of developing the core functionality of the library and leave the extra features for later.

And to make it faster, I developed it within the scope of the application in which it would be used: [**Shortbot**](https://felipe.nubecita.eu/projects/shortbot/). So I took all the code related to scrapping data from the Spanish regulator and pushed it into the application project (see [this](https://github.com/felipet/shortbot/commit/2a91d7b6ee8a43de5a5555b3455f6f4030e694c4)).

Today, the library includes an improved implementation of such module introduced in **Shortbot** plus the code to handle the insertion of the data into a database.

# Information Access

**Shortbot** was the main application that would consume the harvested data. However, that was only the first step. For the achievement of more complex analysis of the collected information, having the information well structured in a database is a must.

After a bit of research, I decided to use a type of database engine that I had never used before: [QuestDB](https://questdb.com/). Although my usual DB choice, **PostgreSQL**, can handle time series data, there are other engines which are more suitable for handling time series, and specially stock related time series. **QuestDB** is designed with finance data as main application, and offer a decent community version to install it locally without paying a penny.

So the missing component of the library was a module that would handle the data collected by the scrapper modules and push it into a database. And that is the big feature introduced in this first version of the library.

# Resources

The code of the library is released to the public using the Mozilla Public License v2.0. This means it is open source code! And you can use free of charge.

The repository with the code is found in [GitHub](https://github.com/felipet/data_harvest), and if you plan to build an application using the library, you'll find a crate ready to go in [crates.io](https://crates.io/crates/data_harvest). Finally, the documentation of the source code is found [here](https://docs.rs/data_harvest/0.1.0/data_harvest/).

# Future Plan

As you might guess, **Shortbot** does not make use of this library yet. And yes, it is in the plan to include such support. The first thing **Shortbot** will benefit from it is a near-zero latency when requesting a short position against a company when using the bot in Telegram.

Nowadays, it takes ages to retrieve the information as it is scrapped directly from CNMV's website (which is damn slow).  From today, **Shortbot** can decouple the data harvesting, and simply connect to the local database which keeps the updated record of the short positions.

And beyond its use in the **Shortbot** application, I plan to start analysing how hedge funds work and eventually develop a model that will help me make money from their efforts. But to do this, I need to extend the library's code to parse the CNMV's records, which are delivered in a spreadsheet. In this way, I will not only have all the information offered today, but also the historical information.
