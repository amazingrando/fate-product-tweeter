[![Build Status](https://travis-ci.org/amazingrando/fate-product-tweeter.svg?branch=master)](https://travis-ci.org/amazingrando/fate-product-tweeter)

# Fate SRD auto tweeter

This project creates a script that will pull a random product from fate-srd.com and post about it to the @FateSRD twitter account.

The project is based on the advice of http://techknights.org/workshops/nodejs-twitterbot/.

## Requirements

- NodeJS (tested with 7+)
- Yarn for package management

## Installation

- `git clone` this repo and `cd` into it.
- `yarn` to install packages
- Create a [Twitter app](https://apps.twitter.com/), including Access Tokens.
- `cp config.js config.local.js` and enter your credentials into `config.local.js`.
- You will also need to set the source for the json in `config.local.js`

## How to Use

- Run `node app.js`

## Heroku Deployment

Heroku needs `config.local.js` so when there are changes:

1. Create `heroku` branch
2. In `.gitignore` remove `config.local.js` and add changes to the branch
3. `git push heroku heroku:master`
4. Remove `heroku` branch.
