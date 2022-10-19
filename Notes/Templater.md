[[Home]]

# [[Templater]]

A powerful templating system that allows templates to be composed, specified by folder and conditional logic for template picking.

Uses an API that is built on JavaScript that has access to utilities like momentjs.

```md
<% moment(tp.file.title).format("YYYYMMDDHHmmss") %>
```

Template Composition

```md
<% tp.file.include('[[Frontmatter (Section Template)]]') %>
```

Conditional Template Picking.
```md
<%*
const title = tp.file.title

// "Book" Notes
if (title.includes('(Book)')) {
	return tp.file.include('[[Book (Template)]]')
}
// "People" Notes
else if (title.startsWith("@")) {
 	await tp.file.move("/people/" + title)
 	return tp.file.include('[[People (Template)]]')
} 
// "Starter" Note
else {
	return tp.file.include('[[Starter Note (Template)]]')
}
%>
```

- See [[People (Template)]] for substring example.