Bleach
================

The goal is simple: block ads and stuff. 

How
----------------

For years, I've been using an [awesome hosts file](http://winhelp2002.mvps.org/hosts.htm) to redirect requests to sites that serve ads to `127.0.0.1`. It's OS-wide, so it works on all your browsers. It shouldn't be difficult to download the file and parse it into the JSON that Safari content-blocking extensions use.

Challenges
----------------

It's going to be tricky for a few reasons. 

1. Sometimes you _want_ content that's blocked by the hosts file. For example, clicking on Google Ads (which aren't blocked) doesn't work anymore.
2. As an iOS developer, it makes it hard to use and test analytics libraries.
3. I want to support the maintainers of the hosts file as much as possible, in some way. It may run afoul of the IAP rules.
4. Apple may not like the idea of an app downloading an arbitrary list of thousands of domains to block content from. 
5. The scale of it may be too much for the APIs to handle. 
