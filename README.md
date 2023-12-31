# Daily Memes Discord Bot

## Overview
This Discord bot, developed in Python, utilizes the `discord` and `requests` packages to post three memes daily in a selected channel. It fetches memes using an API endpoint from Reddit and is hosted on Modal, a cloud computing platform, where secrets and keys are securely stored.

## Features
- **Daily Meme Posting**: Automatically posts three memes every day to a designated Discord channel.
- **Reddit API Integration**: Uses the Reddit endpoint for fresh meme content.
- **Cloud Hosting**: Runs on Modal, ensuring reliable uptime and secure key management.

## Requirements
- Python 3.8 or later
- `discord.py` package
- `requests` package
- Modal account for hosting and key management
- RapidAPI key for meme API access
- Discord bot token

## Setup Instructions

1. **Install Dependencies**:
   Ensure Python is installed on your system. Then, install the required packages:
```
pip install discord.py requests
```
2. **Modal Setup**:
- Sign up for a Modal account and set up a new project.
- Store your RapidAPI key and Discord bot token as secrets in Modal.

3. **Discord Bot Setup**:
- Create a Discord bot on the Discord developer portal.
- Add the bot to your server and note down the bot token.

4. **Environment Variables**:
Set the following environment variables in Modal:
- `DISCORD_BOT_TOKEN`: Your Discord bot token.
- `CHANNEL_ID`: The ID of the Discord channel where memes will be posted.
- `REDDIT_CLIENT_ID`: Your Reddit app client ID.
- `REDDIT_CLIENT_SECRET`: Your Reddit app client secret.
- `REDDIT_USERNAME`: Your Reddit account username.
- `REDDIT_PASSWORD`: Your Reddit account password.

## Usage

1. **Deploying the Bot**:
- Use the provided Modal stub to deploy the bot.
- The bot will automatically post three memes in the specified channel every day.
- The subreddits list can be modified to change the source of memes.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
