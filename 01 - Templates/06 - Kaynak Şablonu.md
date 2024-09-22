---
arsiv_mi: false
yasam_alani:
proje:
kaynak_adresi:
olusturma_tarihi: <% tp.file.creation_date() %>
tags:
  - kaynak/makale
  - kaynak/video
  - kaynak/kurs
  - kaynak/kitap
  - kaynak/video-listesi
  - kaynak/dokumantasyon
  - kaynak/stackoverflow
  - durum/eklendi
  - durum/devam-ediyor
  - durum/tamamlandi
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
where kaynak = [[<% tp.file.title %>]] and arsiv_mi = false
```
## İçerikler
---
```dataview
table
from "08 - İçerikler"
where kaynak = [[<% tp.file.title %>]] and arsiv_mi = false
```