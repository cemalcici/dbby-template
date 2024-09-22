---
arsiv_mi: false
yasam_alani: 
olusturma_tarihi: <% tp.file.creation_date() %>
---
```meta-bind-button
label: Oluştur
icon: ""
hidden: false
class: ""
tooltip: ""
id: ""
style: primary
actions:
  - type: command
    command: quickadd:runQuickAdd
```
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