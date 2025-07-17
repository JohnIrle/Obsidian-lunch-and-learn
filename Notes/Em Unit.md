---
uuid: 20241022110259
created: 2024-10-22T11:02:59
topics:
  - "[[CSS|CSS]]"
---

- Em is a unit in CSS that uses the font-size of the parent container that the value is being set from. 
- If the the parent container has a font-size of 15px then 1em is 15px, 2em is 30px.

This is problematic if you have several nested children all using em.

```css
.parent {
  font-size: 18px;
}
.child {
  font-size: 1.5em;
}
```

```html
<div class="parent">
  15px
  <div class="child">
    30px
    <div class="child">
      60px
      <div class="child">120px</div>
    </div>
  </div>
</div>
```

- The [[Rem Unit]] is based on the fixed font-size of the HTML element and does not have this problem.

