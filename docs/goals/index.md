---
layout: default
title: Goals
nav_order: 2
---

# Goals
Kindmetrics have support for Goals you can send to structure a bit more what the user did. Examples of goals:
- Sign up
- Sign in
- Register for newsletter

You can easily do this with our javascript library.

## Setup the events in  your settings
To let us know that this event should be saved, you would need to add it to your goals list. Login and pick the domain you want to add the goal for.

Click on goals and on the blue button on the right saying `Goals settings`. You can there add your goal.

## Different event types
We have support for 2 different event types for now. Normal event or if a user visited a page. Visiting pages could be used for see how many visited sign_up form and then you can use event to see the conversion on the form.

Pick the one that is correct and type either the name of the event if you picked events or type the path (like `/sign_up`) if you picked path.

## Call the javascript library
If you picked normal events, you would need to call the event when it should be triggered. Kindmetrics javascript library have that already built-in so you can easily just call a function to send custom events for that, if you have added it in the settings first of course.

Add javascript library in your header if not done already:
```html
<script src="https://kindmetrics.io/js/track.js" defer="true" async></script>
```

Then call your event:
```javascript
window.kindmetrics.track("sign_up")
```

You should see the number on your goal in dashboard increase now.
