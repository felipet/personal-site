+++
date = '2025-01-28T16:53:44+01:00'
draft = true
title = 'Shortbot Meets DBs'
author = "Felipe Torres González"
cover = ""
description = ""
categories = ['shortbot']
tags = ['shortbot', 'programming']
+++

# Introduction

As of today, the [IbexShortBot](/projects/shortbot) is a stateless bot. A stateless bot doesn't keep any sort of information of the users. It just replies to the user's requests, one at a time. Despite that design decision made the bot very restricted on its features, it helped me to focus on delivering a solution as quickly as I could, to attract investor's interest on using the bot.

The bot has been used for six months. Lots of users – several tens of them – make use of it every day. That's enough for me to decide to take it a step further. 

**It's time for the bot to meet databases.**

# New features

I ran a survey between the users of the bot, and by far, the most requested feature is related to following stocks and receiving updates when any short position changes.

Compared to the current flow, in which an user has to select the stock every time she/he aims to check whether the position changed or not, the subscription-based flow would heavily simplify the user's experience, and it would avoid missing any update in a position.

It seems a simple change: add an SQLite database, keep user's subscriptions and run a timed-service to inform users when a change occurred.

But this time, I want to think big. That flow was in my mind since the beginning, but I considered that it was more interesting to deliver a simple solution quickly, than a full solution that would have required more development time.

# A Fully Integrated Stock Market Data Information System

One year ago, I started to work on the idea of having a Rust-based ecosystem for investment analysis and trading tools. The overall idea is having all the data centralised in a local database system that would feed my analysis tools.

Information about investment and trading is everywhere these days. One just needs to choose an investment strategy and follow it. However, what if I'd like to explore and implement my own financial models, or design custom trading oscillators? What if I rather make my own way than follow someone else's? Most would say, that's stupid, as only a few can beat the market. I'll say that mostly true when you look where most of people do. But I'm convinced that it is possible to beat inefficient markets. 

I won't enter in what is an efficient market, and what is not. It would be a pretty long explanation (it would well deserve it's own blog entry). Let's say, very very briefly, that an efficient market would find a fair price for a stock pretty quickly, whilst an inefficient market wouldn't do it. It means that inefficient markets include both under valuated and over valuated stocks in higher proportions than efficient markets. Here's where one can beat the market.

My market of choice is the Ibex35, and I do believe it is an inefficient market. Why do you tell me all this nonsense, you'd ask. The answer is related to what I said in the second paragraph of this section: inefficient markets don't offer the market information as easily as efficient markets do, and that's why it is so important for me to develop a **fully integrated stock market data information system**.

And a (small) part of this information system is the **IbexShortBot**.

## 




