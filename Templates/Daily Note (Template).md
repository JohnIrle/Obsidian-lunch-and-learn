---
uuid: <% moment(tp.file.title).format("YYYYMMDDHHmmss") %>
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DDTHH:mm:ss") %>
alias: 
- "<% moment(tp.file.title).format("MMMM Do, YYYY") %>"
- "<% moment(tp.file.title).format("dddd Do MMMM, YYYY") %>"
---

## What do you plan to do today?

## What did you accomplish today?

## What are some moments worth sharing?

---

## 📇 Additional Metadata

- 🗓️ Week:: [[<% moment(tp.file.title).format("YYYY-[W]ww") %>]]
- 🗂 Type:: #calendar/timeline/daily