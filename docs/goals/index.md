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
To let us know that this event should be saved, you would need to add it to your goals list. Log in and pick the domain you want to add the goal.

Click on goals and the blue button on the right saying `Goals settings.` You can add your goal there.

## Different event types
We support two different event types for now—a normal event or if a user visited a page. Visiting pages could be used to see how many visited sign_up forms, and then you can use the event to know the conversion on the form.

Pick the correct one and type either the event's name if you picked events or type the path (like `/sign_up`) if you chose a path.

## Call the javascript library.
If you picked regular events, you would need to call the event when it should be triggered. Kindmetrics javascript library has that already built-in, so you can quickly get a function to send custom events for that if you have added it in the settings first.

Add javascript library in your header if not done already:
```html
<script src="https://kindmetrics.io/js/kind.js" defer="true" async></script>
```

Then call your event:
```javascript
window.kindmetrics.track("sign_up")
```

You should see the number on your goal in the dashboard increase now.
