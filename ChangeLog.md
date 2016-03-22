# Version 0.2.4 #
  * Fix unsigned long long incompatibility on some platform. ([Bug #152](https://code.google.com/p/microblog-purple/issues/detail?id=152))
  * Change replies timeline url to /mentions instead

# Version 0.2.3 #
  * Fix the serious corruption when connection dropped bug. Now MBPidgin is much more stable
  * Fix Pidgin 2.6 compatibility

# Version 0.2.2 #
  * Mainly bug fixes

# Version 0.2.1 #

  * Twitter, Identica, and Laconica now serve mainly as protocol only plug-in. You need to enable Twitgin in order to get old fancy output in conversation windows
  * Fix SSL connection bug that may crash Pidgin when connection is unstable
  * Clicking reply link now add in\_reply\_to\_id http parameter (make the message appear sa "reply to message" in web-site)
  * Remove "twitter.com" label. Now conversation showed as if coming from each individual user
  * Add (Favorite) and RT (Retweet) link for easy favorite and retweet (thanks to @nopparat)
  * Move "Enable reply link" preference to Twitgin "Configure plug-in".
  * Adium plugin port created