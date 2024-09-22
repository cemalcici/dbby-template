---
arsiv_mi: false
yasam_alani: 
olusturma_tarihi: <% tp.file.creation_date() %>
tags:
  - durum/eklendi
  - durum/devam-ediyor
  - durum/tamamlandi
  - yasam-alani/is
  - yasam-alani/kisisel
---
## Kaynaklar
---
```dataview
table
from "06 - Kaynaklar"
where proje = [[<% tp.file.title %>]] and arsiv_mi = false
```
## Notlar
---
```dataview
table
from "07 - Notlar"
where proje = [[<% tp.file.title %>]] and arsiv_mi = false
```