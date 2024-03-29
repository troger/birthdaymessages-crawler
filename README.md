# birthdaymessages-crawler

## Overview

This scripts crawls the given URL from [birthdaymessages](http://www.birthdaymessages.com/) to extract messages and post them to the specified SosMessage API URL.

Sample usage:

    ./birthdaymessages-crawler.rb -u http://www.birthdaymessages.com/happy/happy -s http://localhost:3000 -c 4f6a4f80744e34609b3c8127

The crawler will try itself all the available URLs: happy1.htm, happy2.htm, ... until it found a 404 page.

Full options:

    Usage: birthdaymessages-crawler.rb [options]
    -u, --messages-url URL           The birthdaymessages category url
    -s, --sosmessage-url URL         The SosMessage API url
    -c, --category-id CATEGORY_ID    The category id where to post the messages
    -m, --max-characters MAX         MAX characters of the message
    -n, --dry-run                    Don't actually post the messages, only display them
    -h, --help                       Display this screen
