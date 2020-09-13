---
layout: default
title: Hide yourself from the stats
parent: Domain
nav_order: 6
---

# Hide yourself from the stats

For many reasons, it might make sense to hide from the stats. You can do that in two ways.

- Block the script with an adblocker
- Use of Do Not Track header.


## Adblocker
Blocking the pageviews on Kindmetrics can be done by using an adblocker extension in your browser. You can use [Adblock Plus](https://adblockplus.org/) or [uBlock Origin](https://github.com/gorhill/uBlock/#installation).

### Locate My Rules
- Click the **"uBlock Origin"** icon in your browser
- Then click the "Dashboard" icon in the lower-right corner to open the uBlock Origin dashboard
- Tick the "I am an advanced user" box

Select then My Rules. You will now see two fields, in the **temporary rules** on the right side, type in:
```
yourdomain.com kindmetrics.io * block
```
Change **yourdomain.com** to your domain you used when installing Kindmetrics.

If that didn't work, it could be that you use a different address; try to add this line as well:
```
yourdomain.com app.kindmetrics.io * block
```

### Check if it works
Go to your website and check if your visits are registered. If not, it didn't work.

## Do Not Track
Do Not Track was a thing that was bigger before, but some browsers still use it.

This DNT will send a little text on every request to every website you visit that you don't want to track. Kindmetrics won't send anything if this is enabled to respect users' wishes not to be tracked fully.

Go to browser specific tutorial how to enabled it for you:
- [Brave](https://support.brave.com/hc/en-us/articles/360017905612-How-do-I-turn-Do-Not-Track-on-or-off-)
- [Firefox](https://support.mozilla.org/en-US/kb/how-do-i-turn-do-not-track-feature)
- [Chrome](https://support.google.com/chrome/answer/2790761?co=GENIE.Platform%3DDesktop&hl=en)
