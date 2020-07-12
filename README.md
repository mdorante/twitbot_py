# twitbot_py

Hi! This is a Twitter bot that I'm coding in order for it to help me with my Twitter account.

This repo is going to be (kind of) a template in case anyone wants to create their own Twitter bot based off of it!

## Requirements

You will need Python 3.8.x

You will need a Twitter Developer Account, if you don't have one yet, create one [here](https://developer.twitter.com/en/apply-for-access).

Please refer to the [Twitter Developer Docs](https://developer.twitter.com/en/docs/basics/developer-portal/overview) for detailed instructions on the creation of your Dev Account.

Once you have your Dev Account all set up, you will need to [create an app](https://developer.twitter.com/en/apps/create).

The steps for the creation of your Twitter Developer Account and Twitter Apps are outside the scope of this project, fortunately, Twitter's Dev Docs are great and will get you up and running in no time!

I will assume you have already applied and have access to a Developer Account from here on after.

## Setup

- First, clone this repo:
  - `git clone git@github.com:mdorante/twitbot_py.git`
- Create a Python Virtualenv (I highly recommend [pyenv](https://github.com/pyenv/pyenv)):
  - `pyenv virtualenv twitbot_env`
- Now you can install the requirements for this project:
  - `pip install -r requirements.txt`
- If you take a look at the files this repo contains, you will see that `setup.py` requires four environment variables. These are your Twitter API tokens for your app. The recommended setup for security reasons is:
  - Create a `.env` file in the root directory of this repo.
  - Add the following environment variables to your `.env` file: (you can find all these tokens at your [Twitter apps page](https://developer.twitter.com/en/apps) -> Details -> Keys and tokens)
    - CONSUMER_API_KEY=\<insert token here>
    - CONSUMER_SECRET_KEY=\<insert token here>
    - ACCESS_TOKEN=\<insert token here>
    - ACCESS_TOKEN_SECRET=\<insert token here>
  - **_DO NOT COMMIT THIS FILE_**, if you do, then anyone that can access your repo will have access to your Twitter account!

## Usage

- You can modify the `basic_hashtags` dict and add your favorite hashtags to it.
- Use the `post_tweet()` function in order to post your tweets.

### TODO

- Add more functionality, all it does is tweet (for now).
