---
id: joyce-lin
title: Reverse Engineering a Private API
desc: ''
updated: 1661898027720
created: 1661898027720
tags:
  - api
  - web
  - security
location: 'San Francisco, CA, USA'
uri: ''
twitter: petuniaGray
company: Postman
pronouns: she/her
enableGiscus: true
---
> The contents here is created from the official [CascadiaJS Page](https://2022.cascadiajs.com/speakers/joyce-lin)

## Overview

![Joyce Lin image](https://create-4jr.begin.app/_static/2022/joyce-lin.jpg){max-width: 300px}
- name: Joyce Lin
- [Speaker Page](https://2022.cascadiajs.com/speakers/joyce-lin)

## Abstract

Learn how to inspect APIs for when you're working with poorly documented ones, debugging, web scraping, or penetration testing.

## Notes

## Notes by [aminamos](https://github.com/aminamos)
- https://www.toptal.com/back-end/reverse-engineering-the-private-api-hacking-your-couch
- https://blog.tendigi.com/starbucks-should-really-make-their-apis-public-6b64a1c2e923
- keep in mind
    - review the terms of service before starting this
    - find a path for "responsible disclosure"
    - be ethical
- three common items to analyze
    - individual API request
    - session details
    - stream of HTTP requests
- can use dev tools to copy as curl --> bring into Postman (or API tool) as raw text
- can also look into session details, via HAR files
- the exported HAR can be imported into [Postman](https://www.postman.com/postman/workspace/postman-answers/documentation/9215231-dd262075-9008-429c-8039-c8c67ee9bf67) (P.S. also https://toolbox.googleapps.com/apps/har_analyzer/)
- Postman can also be used as a proxy that captures HTTP requests https://learning.postman.com/docs/sending-requests/capturing-request-data/interceptor/
    - also works on mobile https://blog.postman.com/using-postman-proxy-to-capture-and-inspect-api-calls-from-ios-or-android-devices/
- replay API calls, can be difficult to run one call long term due to expiring info
- if scraping dynamic websites, a lot of the info won't immediately be there
- Googlebot user-agent can help view HTML
