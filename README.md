# Lead Finder

A python script that scrapes Google maps for contact info of businesses found via the search term provided by the user. This script was intended to create a list of leads 
for B2B marketing, but it might have other OSINT uses. 

# Disclaimer

This might go against Google's terms of service. USE AT YOUR OWN RISK!!! Honestly, they crawl and scrape millions of websites every day, so I don't feel bad about creating something like this.

# Prerequisites

These packages are required to run this script:

```
emailfinder
selenium
tldextract
urllib
```
They can be installed like so: `pip install <package>`

# Usage

Simply provide Lead Finder with a relevant search term (for Google maps), and a name for the output file:

`lfinder <search_term> <output.csv>`

Example:

`lfinder "bakeries Portland OR" bakery_info.csv`

While just searching for "bakeries" will work, I recommend adding a location to narrow down the search and get more tailored results.

# Current Problems

- Email Scraper gets blocked: After a handful of requests from the email finder function, Google blocks future requests. 
Don't know how to prevent this from happening.
- Junk Emails: Some of the emails found are junk (i.e. jdoe@domain.com, lxxxxj@domain.com, x22@domain.com). Not sure how to verify email address legitimacy. 

# Version Notes

- v1.0: Initial Release
