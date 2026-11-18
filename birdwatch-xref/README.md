# Birdwatch Crossreferencing (`birdwatch-xref`)

Compare a list of Tweet IDs and determine which, if any, received notes in Birdwatch/Community Notes, Twitter's crowd-sourced program for fact-checking and community moderation.

Birdwatch data is pulled from the [Birdwatch Archive](https://birdwatcharchive.org/) project, which itself relies on these scripts: https://github.com/bpettis/birdwatch-scraper

Note (As of Nov. 2026) -- this is a very early alpha-version script that expects to be able to talk directly with a Postgres databse which contains data parsed from Birdwatch. As part of a larger project to rebuild and redesign the Birdwatch Archive infrastructure, I plan to rewrite this script to work using a publicly accessible REST API.

## Setup

The script expects a `.env` file which contains database connection information. 