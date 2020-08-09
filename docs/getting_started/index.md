---
layout: default
title: Getting Started
nav_order: 1
---

# Getting started

You need to start by getting an account, you do that by going to [kindmetrics.io/sign_up](https://kindmetrics.io/sign_up)

## Add your domain

You will be shown an form where you add your domain, you add an domain without `www.`, as an example: `kindmetrics.io`

## Add the javascript to your website

You will then be presented an javascript code. Add that to your head on all the sites you want to track visitors.

```html
<script src="https://kindmetrics.io/js/track.js" defer="true" async></script>
```
If you instead want to specific set the domain it shall come into, you can add data paramter called domain:

```html
<script src="https://kindmetrics.io/js/track.js" defer="true" data-domain="kindmetrics.io" async></script>
```
