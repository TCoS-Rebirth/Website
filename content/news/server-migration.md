  ---
title: "Server move finished + introducing new account system"
date: 2023-07-06T11:50:00+02:00
draft: false
summary: "The move to the new server and account system."
tags: [ "new server", "future", "account" ]
description: "The move to the new server and account system."
leadtext: "And we're live."
headerimage: "viola.png"
author: "Kevin"
---

Hello there! 

The migration to the new game server has been completed and the game is back online on a brand new (and much more powerful) machine.
This entire endeavour has been centered around allowing The Chronicles of Spellborn to run for many more years by modernizing the software that the server itself runs upon. This entire project ran for many months and required a lot of work, but in the end we're glad to say that the game should run fine on this new generation of software.

With our focus on modernizing the server, we also turned our eye to the current account registration system which was a bit... barebone, to say the least. In essence, this was a debug page that we dug up and re-used for our signup page, but it came with quite a lot of drawbacks - the only unique information stored was the username and password, which made it impossible to implement a password reset feature.
So, quite early on in this process the decision was made to build a custom account system that would wrap around the existing game systems, a "master account" to bind all of your existing and new accounts to. Let's go a bit more in depth.

# Creating a new account
In order to create a new game account, you will need to register a new account on https://account.spellborn.org. This is a completely seperate system from both the forums, our Discord and the previous accounts and it is your new master account. 
This master account can not be used to login to the game with, but can be used to create new game accounts or used to link your existing game accounts to your master account. This has the advantage that you can reset the password of both old and new accounts.

The new Account system is also way more secure, as passwords are stored quite a lot more securely, and enables you to reset your password should you forget it.

In order to create a new game account, you'll need to create an account on the Spellborn Account system. Once that is done, you'll be able to create a new game account from this website. You can also access the Spellborn Account system from within the launcher by clicking on **Create Account**.

# Claiming your existing game accounts
Since there is no information stored that we can use to link your existing accounts, we have built a system where you can log in to your existing accounts and claim this to your Spellborn Account. An account link is permanent and each game account can only be linked to a single Spellborn Account.
In order to link your account, you'll need to login to the Spellborn Account system and choose (in the top bar) **Link existing account** or go to https://account.spellborn.org/game/claim. 

From this page you can link your existing account. Should you get an error, or in the case that you no longer know the password of your original account, feel free to contact us on help@spellborn.org or in the Discord-server.

# Monitoring update
A short while ago, we introduced a Status page on the website, this has now been integrated into the launcher so you can see if the game server is online/offline or down for maintenance.

# Bugs
Ofcourse this is a huge change for both the game as well as us (with the account system), so bugs are to be expected. Should you encounter a bug, feel free to report this on the Discord and we'll glady take a look at it.

From the entire Spellborn team, we thank you all for your support and what lies hidden, must still be found.

- Kevin
