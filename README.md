# genshin stats api
This project is meant to be a wrapper for the [hoyolab.com](https://www.hoyolab.com/genshin/) gameRecord api.
I have attempted to reverse engineer their API to find out the important tokens and cookies and then to what urls they are sent.

# how to use
Paste your hoyolab cookies and temporary ds token into `config.ini`, you can then import the `genshin_stats` module and use it's API.
All functions are documented and type hinted.

# how to get your cookie
1. go to [hoyolab.com](https://www.hoyolab.com/genshin/)
2. login to your account
3. click on your profile and go to account info (will look something like `https://www.hoyolab.com/genshin/accountCenter/gameRecord?id=8366222`)
4. right click on the page and press inspect
5. go to network, press `XHR` in the filter row and then reload the page
6. click on `getUserFullInfo` or anything after
7. scroll a bit down, right click and copy the header `cookie`
8. paste into `config.ini`
