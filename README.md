**Reddit Daily Bot**

Reddit Daily Digest Bot is a Python bot designed to simplify the process of aggregating and sharing top posts from your favorite subreddits. It fetches the most popular posts from specified subreddits, compiles them into a neatly formatted daily digest, and automatically posts the digest to a target subreddit of your choice. Also works for hot, controversial, rising & new posts. You can also specify your own time range for the posts the bot will fetch

**Installation**
Clone this repository to your local machine:

git clone https://github.com/SamSon1402/reddit-bot/edit/main
Change the project directory

cd reddit-dailydigest-bot
Install Dependencies

pip install -r requirements.txt
Configuration
Reddit API Credentials
Open the config.py file and replace the placeholders with your Reddit API credentials:

CLIENT_ID = 'your_client_id'
CLIENT_SECRET = 'your_client_secret'
USER_AGENT = 'your_user_agent'
REDDIT_USERNAME = 'your_reddit_username'
REDDIT_PASSWORD = 'your_reddit_password'
Subreddits
Modify the SUBREDDITS variable in config.py to specify the subreddits from which you want to fetch posts. Don't include r/ before the name of the subreddit.

SUBREDDITS = ['science', 'technology', 'maths', 'physics']
Target Subreddit
Replace the TARGET_SUBREDDIT variable with the subreddit name where you want the bot to post the content:

TARGET_SUBREDDIT = 'your_target_subreddit_name'
Time Range
Update the TIME_RANGE to the time range you need for the controversial.py and top.py script

TIME_RANGE = 'day' 
'day': Fetch top posts from the last 24 hours.
'week': Fetch top posts from the last 7 days.
'month': Fetch top posts from the last 30 days.
'year': Fetch top posts from the last 365 days.
'all': Fetch top posts from all time.
