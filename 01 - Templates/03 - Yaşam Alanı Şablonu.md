---
arsiv_mi: false
olusturma_tarihi: <% tp.file.creation_date() %>
tags:
  - yasam-alani/is
  - yasam-alani/kisisel
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
## Beceriler
---
```dataview
table
from "04 - Beceriler"
where yasam_alani = [[<% tp.file.title %>]] and arsiv_mi = false
```
## Projeler
---
```dataview
table
from "05 - Projeler"
where yasam_alani = [[<% tp.file.title %>]] and arsiv_mi = false
```
## Kaynaklar
---
```dataview
table
from "06 - Kaynaklar"
where yasam_alani = [[<% tp.file.title %>]] and arsiv_mi = false
```
## Notlar
---
```dataview
table
from "07 - Notlar"
where yasam_alani = [[<% tp.file.title %>]] and arsiv_mi = false
```