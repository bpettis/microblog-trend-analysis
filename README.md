# Microblog Trending Topics Analysis

This repo will contain some basic scripts for interacting with previously scraped data from Twitter, Bluesky, Mastodon, etc. 

This is a spin-off of an earlier project which aimed to assess the activities of right-wing "culture warriors" on Twitter (https://github.com/bpettis/twitter-ringleaders). That project was built around parsing Twitter data, specifically. However, 



### Input Data

Scripts will likely expect input data files to be placed in a `data` directory in the project root. This directory is excluded via the `.gitignore` file to avoid committing sensitive info to a public repo. Be sure to create this directory beforehand, if it doesn't already exist.

### Output Directories

Similarly, scripts' output directories will be excluded via `.gitignore` to avoid inadvertently committing data. Making data publicly available is a good thing, but I think that it should be done on your terms - rather than happening automatically. It's better to have a chance to review output to make sure PII isn't getting exposed. Be sure to create this directory beforehand, if it doesn't already exist.

---

## Scripts

Simple descriptions/overviews of each script and/or project component. Some scripts are platform-agnostic, that is to say that they will work with data scraped from any social media platform so long as it is formatted in a consistent and predictable way. 

### Twitter/X

### Birdwatch Crossreferencing ([birdwatch-xref](./birdwatch-xref/))

Compare a list of Tweet IDs and determine which, if any, received notes in Birdwatch/Community Notes, Twitter's crowd-sourced program for fact-checking and community moderation.

Birdwatch data is pulled from the [Birdwatch Archive](https://birdwatcharchive.org/) project, which itself relies on these scripts: https://github.com/bpettis/birdwatch-scraper. (UPDATE as of Fall 2026 - due to issues with my own hosting infrastructure and Twitter/X making changes to their data accessibility, the Birdwatch Archive website is temporarily unavailable.)


More details here: [birdwatch-xref/README.md](birdwatch-xref/README.md)

### Check TwitterUsers (`user-checking`)

Takes a CSV file which contains twitter usernames and attempt to determine whether the account is active, suspended, or deleted.

More details: (user-checking/README.md)[user-checking/README.md]
