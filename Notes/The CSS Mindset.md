[[CSS MOC]]

# [[The CSS Mindset]]

- Everything is a rectangle
- No point in declaring width: 100% on a block-level element
- No need to set position: relative if you don't need a new stacking context.

[[Shorthand CSS Rules Change Several Values]]

- Avoid "magic numbers"
- magic numbers are random hard values
```css
.thing {
  width: 218px;
}
```
- Using the arrow key to adjust a pixel value is a code smell for magic numbers


---

**🤝 Related Links**

- 👤 Creator(s): [[@Max Böck]] 
- 🔮 Origin: https://mxb.dev/blog/the-css-mindset/