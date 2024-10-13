---
dosya:
yazar:
yayin_tarihi:
olusturma_tarihi: <% tp.file.creation_date() %> 
okuma_baslangic_tarih: <% tp.date.now("YYYY-MM-DD") %>
okuma_bitis_tarih:
proje:
ilgi_alani:
tags:
---
<% await tp.file.move("/04 - Resources/" + tp.file.title) %>
## Özet
- 
## Ana Fikirler
- 
## Alıntılar
- 
## Notlar
### Gelen Kutusu
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "01 - Inbox"
WHERE contains(kaynak, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```
### Kalıcı Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Notes"
WHERE contains(kaynak, [[<% tp.file.title %>]])
SORT olusturma_tarihi DESC
```