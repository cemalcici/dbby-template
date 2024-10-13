---
olusturma_tarihi: <% tp.file.creation_date() %>
tags:
---
<% await tp.file.move("/03 - Areas/" + tp.file.title) %>
## Projeler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "02 - Projects"
WHERE contains(ilgi_alani, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```
## Kaynaklar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "04 - Resources"
WHERE contains(ilgi_alani, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```
## Notlar
### Gelen Kutusu
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "01 - Inbox"
WHERE contains(ilgi_alani, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```
### Kalıcı Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Notes"
WHERE contains(ilgi_alani, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```