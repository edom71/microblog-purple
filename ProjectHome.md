This project implement a plug-in for any [LibPurple base client like Pidgin or Finch](http://www.pidgin.im) . Currently it support [Twitter](http://twitter.com), [Identica](http://identi.ca), and [Status.net server](http://status.net) through the conversation windows. Right now it run on Linux and Windows.

  * **Please upgrade your MBPurple to 0.3.0 before reporting any bugs!**
  * Ubuntu's PPA is available at [Awashiro Ikuya's PPA repository](https://launchpad.net/~ikuya-fruitsbasket/+archive/ppa/)
  * README is [here](http://code.google.com/p/microblog-purple/wiki/README)

### Version 0.3.0 is released (30/5/2010) ###
  * Most important update is the **support for OAuth for Twitter**. OAuth is now default authentication method.
  * Change identity of identi.ca and status.net
  * Fix twitter-bombard-when-reconnecting bugs.
  * Windows version tested with Pidgin 2.7.0 and 2.6.6.

PPA for Ubuntu is available in the link above.

### Version 0.2.4 is released (26/9/2009) ###
  * Fix "Twitpocalypse2" where mbpurple download whole lots of old tweets over and over. This bug occurred on some platform (as of now Windows XP seems to be affected by this)
  * Fix reply and retweet links for Pidgin 2.6.
  * Fix stability bug that crash Pidgin when connection is unstable

### Version 0.2.2 is released (14/6/2009) ###
  * Fix id overflow (receiving duplicate tweets) bug for twitter.com
  * Add CACerts to windows installer
  * Fix few minor bugs
  * Plug-in for Adium is also released! Thanks to @jsippel.

#### Another new release for Adium (21/5/2009) ####
  * This release update libpurple
  * Courtesy goes to @jsippel!
  * Download it [here](http://microblog-purple.googlecode.com/files/TwitterIM.AdiumLibpurplePlugin-0.2.1b.zip)

#### Version 0.2.1 is released (3/3/2009) ####
**Don't forget to enable Twitgin in Tools->Plugin**

This version contain major bug fixes and some improvements
  * Twitter, Identica, and Laconica now serve mainly as protocol only plug-in. You **need to enable Twitgin in order to get old fancy output in conversation windows**
  * Fix SSL connection bug that may crash Pidgin when connection is unstable
  * Clicking reply link now add in\_reply\_to\_id http parameter (make the message appear sa "reply to message" in web-site)
  * Remove "twitter.com" label. Now conversation showed as if coming from each individual user
  * Add `*` (Favorite) and RT (Retweet) link for easy favorite and retweet (thanks to @nopparat)
  * Move "Enable reply link" preference to Twitgin "Configure plug-in".
We are also working on [Adium](http://www.adiumx.com/) port of MBPurple. Hopefully this will be released very soon!

#### Version 0.2.0 is released (7/11/2008) ####
This is a new major release with some more features, along with major code restructure. This release only works with **Pidgin 2.5.x**
  * Beta support for Identi.ca and Laconica, as separated plug-ins.
  * A bit of improvement in message display
  * Improve Twitgin support, no self-generated message also being renice
  * Support for 2 commands, right now it only works for Twitter.
    * /replies - get replies timeline
    * /refresh - get new tweets immediately
    * /tag, /btag, /untag - automatically tag all your message, good for tagging messages with some hash tag (Example: #election2008).
  * Lots more configurable options in Plug-in.

Don't forget to enable **Twitgin** to see new features!

Note that, this new version **is INCOMPATIBLE with older version**. You will need to remove and re-add the plug-in to get all new features.

#### Version 0.1.2 is released (16/8/2008) ####
This release fix [issue#17](https://code.google.com/p/microblog-purple/issues/detail?id=#17) which can crash Pidgin when clicking "reconnect" or Pidgin do automatic reconnect.

---
