---
up: "[[Home]]"
---

- Bases allow you to query notes and display them as views. 

- You can write bases using a code block or by creating a new file.
- For example, you can construct a code block with a `base` key. The following will filter for notes that are in `Notes/Categories`

```yaml
filters:
  and:
    - file.folder == "Notes/Categories"
views:
  - type: table
    name: Table
```

```base
filters:
  and:
    - file.folder == "Notes/Categories"
views:
  - type: table
    name: Table

```

- You can also create a `.base` file.
- For example, this base will show all notes with no links in them. [[No Links.base]]

- You can also embed bases using the `![]` syntax
![[Modified.base]]

- You can leverage embedding with references to the current note to create generic dynamic bases. 
- For example, you can create top-level "Topic/Category" notes and embed a base like the following. See [[CSS]] for an example.

![[Screenshot 2025-11-24 at 2.40.30 PM.png]]

- Bases can have multiple views. There are also multiple types of views: cards, lists, and tables. 
- You can embed a specific view by using a hash link in the embed.
	- `![[Topics.base#View2]]`
- You can use formulas to calculate columns in the table. 
- The following is a formula to display the created date of notes using a relative format, "a year ago."
 ![[Screenshot 2025-11-24 at 2.46.28 PM.png]]
- For more information on bases, see https://help.obsidian.md/bases/syntax and https://help.obsidian.md/bases