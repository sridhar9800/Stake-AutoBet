## Stake.com Scraper and Autobetting Tool

This tool scrapes odds from Stake.com and places bets systematically, even bypassing their CAPTCHA protection with anti-captcha.

**Please note that this tool is no longer actively maintained, and your account may be limited or closed if you use it. I am not responsible for any lost funds.**

## Requirements

* Libraries: `pip install -r requirements.txt`
* AntiCaptcha: You need to have a funded account with API KEY: [Anti-Captcha](https://anti-captcha.com/)
* PostgreSQL: [Download](https://www.postgresql.org/download/)

## Usage

### 1. Create a database

- Run `stake_postgresql.py` or create the database manually using pgAdmin 4.
- Update the connection data in `stake_postgresql.py` as needed.

```markdown
POSTGRES_USERNAME = 'postgres'
POSTGRES_PASSWORD = 'stakevault'
POSTGRES_IP = 'localhost'
POSTGRES_PORT = '5432'
POSTGRES_DB_NAME = 'stake_db'
POSTGRES_SCHEMA_NAME = 'stake_public'


The tables will be stored in the `public` schema, so no need to create an additional one.

### 2. Run the main program

Simply run `main.py`. The program will scrape odds from Stake.com and place bets according to the logic you have implemented.

### 3. Understand the code

The code is well-written and easy to understand. It is a good starting point for building your own Stake.com scraper and autobetting tool.

## Things to keep in mind

* Authentication only works for accounts without two-factor authentication (2FA) enabled.
* This tool is no longer actively maintained, and your account may be limited or closed if you use it.

## Recommended TODOs

* Add support for 2FA bypass.
* Add scraping and betting modules for OneXTwo, OverUnder, and Handicap bets.
* Add a currency converter.

## Safety Guidelines

* This tool should not be used to harm, exploit, or discriminate against anyone.
* This tool should not be used to promote violence, hatred, or discrimination.
* This tool should not be used to seek private information about individuals.


I hope this is helpful!