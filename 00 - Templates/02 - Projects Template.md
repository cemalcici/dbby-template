---
olusturma_tarihi: <% tp.file.creation_date() %>
baslangic_tarih: <% tp.date.now("YYYY-MM-DD") %>
bitis_tarih:
ilgi_alani:
tags:
---
<% await tp.file.move("/02 - Projects/" + tp.file.title) %>
## Proje Açıklaması

## Görevler
- [ ] 
## Kaynaklar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "04 - Resources"
WHERE proje = [[<% tp.file.title %>]]
SORT olusturma_tarihi DESC
```
## Notlar
### Gelen Kutusu
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "01 - Inbox"
WHERE proje = [[<% tp.file.title %>]]
SORT olusturma_tarihi DESC
```
### Kalıcı Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Notes"
WHERE proje = [[<% tp.file.title %>]]
SORT olusturma_tarihi DESC
```