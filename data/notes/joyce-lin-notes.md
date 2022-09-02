
Head of Developer Relations, Postman

### Capturing network traffic

HTTP files

- chrome dev tools
- Right click on network call to copy as curl
- Paste into postman as raw text
- Can then replay and call in postman

Session capture

- har files right click and save all as har
- in postman inspect a the HAR file
    - har is used for ession replay

Capture stream of HTTP API Requests

- use web proxy to capture a stream of HTTP
- Postman has a free proxy tool
    - alternatives fiddler, etc.
    - Postman interceptor chrome extension
        - can apply filters by subdomain
        - see ajax calls
    - in postman desktop create a new collection to capture proxy calls from chrom extension
    
    Proxy through postman, and save as a collection
    
    - capture requests
    - will show connection
    - filter and will proxy all calls live into postmn
    - Stop session, will give analytics afterwords

Proxy mobile app

- see slide

### Replay API Calls

Once you intercept sending reques again after a duration doesn’t work (auth expires)

- Cookie Auth
    - Cookie tab in github
    - manually add cookies to sync w chrome browser → will log you in
    - set cookie in header is the one you use in all your cookies going forward
- can get curl request out of postman so you know how to format the api call so it works

**Spoofing client attributes**

- User agent header
- User-Agent -> Googlebot/2.1
    - Everyone wants to be scraped by google
    - USE THIS AS YOUR USER AGENT
- Replay in code → roll into bot
    - Use code snippet from postman
    

Alissa Knight → hacker

**Hyrums Law**

"With a sufficient number of users of an API, it does not matter what you promise in the contract: all observable behaviors of your system will be depended on by somebody."
