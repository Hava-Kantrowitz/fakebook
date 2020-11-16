# fakebook

## High-Level Approach

We first request the login page, at which we extract the CSRF token and session id. We then create a POST with our username, password, token, and session id. We then use the new session id to have our crawler crawl Fakebook. We implemented a modified DFS to traverse the pages to find the flags.

## Challenges

The main challenge that we faced was creating a proper POST request. It took us awhile to figure out the exact fields and formatting that we needed. However, after several attempts, we found the correct configuration to properly make a POST request.

## Testing

We tested our code by running the code on the server until our code printed out the ten flags.
