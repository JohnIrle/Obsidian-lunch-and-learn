---
uuid: 20241022110259
created: 2024-10-22T11:02:59
topics:
  - "[[CSS|CSS]]"
series: "[[The CSS Mindset]]"
tags:
  - source/example
creator: "[[@Max Böck]]"
source: https://mxb.dev/blog/the-css-mindset/
---

Shorthands have long effects
```css 
background: white;
```
is actually setting
```css
background-color: white;
background-image: none;
background-size: auto auto;
background-repeat: repeat;
background-origin: padding-box;
background-clip: border-box;
background-attachment: scroll;
```
