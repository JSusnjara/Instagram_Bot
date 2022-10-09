# Instagram_Bot
A simple Instagram bot written in python using selenium framework. Can be used for automated liking of recent posts from custom URLs.

## Description
This bot logs a user into Instagram account with login info provided in `config.ini` file. After that, at a random interval (between 1 to 6 hours) 
starts a new liking cyclus. In each cyclus, bot iterates through provided urls and, at a random interval, likes a random number of most recent posts.

The purpose of random is to mitigate the risk of Instagram recognizing automated activity on the account, which may result with a ban.

The bot is set to do the average of 140 likes a day, and 20 likes an hour, to make sure to avoid ban of a new Instagram account.

## Usage

Download repository and edit `config.ini` file by putting your username and password for Instagram in the AUTH section.
In INSTRUCTIONS sector add your list of desired Instagram urls you want automated liking on. Also, you can edit the list of keywords in users' 
usernames you want to avoid liking.
Start your bot with `python3 bot.py`.
