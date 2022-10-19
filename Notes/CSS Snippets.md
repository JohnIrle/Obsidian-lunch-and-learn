[[Home]]

# [[CSS Snippets]]

- Obsidian supports css snippets that add styles on top of the current theme.
- A good way to customize without building your own theme. 
- Found under appearance in settings. The folder icon will open the correct folder.
- Create a css file in the snippets folder.
- Toggle to apply.

![[Screen Shot 2022-07-12 at 9.42.31 AM.png]]

### Example

```css
.markdown-source-view.mod-cm6 .HyperMD-task-line[data-task]:not([data-task=" "]) {
    text-decoration: none;
}
```