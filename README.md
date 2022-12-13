# ublock-medium-list
A rule list for websites that break when using uBO medium mode. This is mostly for my personal use, however it is public if anyone else would like to use it or even contribute. 

THE GOAL IS TO ALLOW PAGES TO FULLY FUNCTION, WITH AS MINIMAL TRACKERS POSSIBLE. With this being said, not all websites will be perfect for now. With some websites listed still broken in some way, or finding out that some trackers don't need to be bypassed for a website to work. 

Accepting your contributions may take a while, as I'd like for them to be tested beforehand. 

Please default to only disabling the specific domains which cause trouble. If you genuinely can't figure it out or the website just is that broken, try only disabling 3rd party scripts. If that still doesn't work then disable blocking of both 3rd party scripts and frames, but only use this as a last resort.

## How to use this???

Go to uBO settings which can be managed by clicking on uBO extension in the top right of your browser, and click the settings wheel. Navigate to the *Settings* pane at the top and enable *I am an advanced user*

Once you have done this, navigate to the *My rules* pane and copy everything on [this page](https://raw.githubusercontent.com/RMED24/ublock-medium-list/main/dyna-rules.txt) and paste it into the *temporary rules* box on the right. Press *save* then press *commit* to merge this with your permanent rules. 

(Notice: if you already had some rules there before, you might want to make sure they aren't overwritten. If you don't know what this means, it is safe to ignore this notice)

## Advantages and disadvantages

I've been asked on multiple occasions what benefits and drawbacks come from this. And there's definitely a few of each which was somewhat [listed here](https://github.com/gorhill/uBlock/wiki/Blocking-mode:-medium-mode#characteristics) and [here](https://github.com/gorhill/uBlock/wiki/Blocking-mode)

However, I've also discovered benefits beyond the reduced amount of trackers and fingerprinting done. These benefits include:

Many websites (although not all) will no longer bother you about cookies and tracking, as the cookie notification service isn't even loaded. (This does not have any effect on whether or not cookies can save however, which is a good thing)

Twitch.tv and youtube.com specifically have a habit of randomly breaking support with adblockers when they update their methods of serving ads. This is beneficial for twitch especially, as it means you wouldn't need another extension eating up CPU cycles to block ads [like previously](https://github.com/pixeltris/TwitchAdSolutions)

Some websites like to use 'antiadblock' or 'fuckadblock' tools. Traditionally the best method would be to use a filter list like [fuckfuckadblock](https://github.com/bogachenko/fuckfuckadblock). You would always be relying on the community to frequently keep this up to date however, and websites like megaup would monitor their github page to break whatever methods they had in place to stop these adlocker pop-ups. The good news with this rule list is that it seems to block 98% of these anti adblock ads. And yes, it is confirmed to bypass any anti-adblock tools on megaup.

In rare instances, you may even be able to bypass paywalls which is most common on some news sites. Nobody wants to pay 2$ for a month to read a news article on a website they'll visit once in their life

* * *

It's not all sunshine and rainbows however. There are some things which can come from medium mode that we're actively trying to eliminate. These include:

A small selection of websites won't load at all and need to be unbroken

Quite a few websites that can load may have important elements of the website that don't work. Such as payment gateways or even simple elements like a search box that uses unpkg.com. 

In many instances, less important elements of a website that bake in things like a discord embed or an accounts.google.com login as an option may be broken and need unbreaking. 

* * *

We would like for you to bare in mind that this rule list is still in early development and may not be perfect from the get go. Whilst this has been tested on google chrome and firefox with no extra issues previously. Whilst unlikely, this could still be broken on browsers other than these two. We recommend using firefox with this just to be safe for the time being if you want this to work the best it possibly can. 

Also, google is all but killing off the adblock in manifest V3 starting from January 2023, so it's probably best to consider switching away from chrome to something else anyway... 
