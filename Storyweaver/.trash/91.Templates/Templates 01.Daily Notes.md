---
created: <% tp.file.creation_date() %>
aliases: 
tags:
  - DailyNote
author:
  - "[[찬스]]"
source: 
type:
  - note
index:
  - "[[🏷 Daily Notes]]"
CMDS:
---
# <% tp.file.title %>
## [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %> |◀︎]] <% tp.file.title %> [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %> |▶︎]]
---
## Summary
#### Highlight
- 
#### Gratitude
- 
## Schedule
#### Event
- 
#### To Do
#todo 
- [ ] 
#### Daily Quote
<% tp.web.daily_quote() %>
## Note-taking
#### Created Today
```dataview
list
from ""
where file.cday = date({{title}}) AND !contains(file.folder, "00. Inbox/01. Daily Notes")
```
#### Modified Today
```dataview
list
from ""
where file.mday = date({{title}}) AND !contains(file.folder, "00. Inbox/01. Daily Notes") AND file.cday != date({{title}})
```
## Log
- 

--- 
# Reference
- 