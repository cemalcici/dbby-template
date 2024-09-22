---
arsiv_mi: false
yasam_alani: 
olusturma_tarihi: <% tp.file.creation_date() %>
---
## Notlar
---
```dataview
table
from "07 - Notlar"
where beceri = [[<% tp.file.title %>]] and arsiv_mi = false
```

## İçerikler
---
```dataview
table
from "08 - İcerikler"
where beceri = [[<% tp.file.title %>]] and arsiv_mi = false
```