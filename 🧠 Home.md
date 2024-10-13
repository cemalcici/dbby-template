## Yakala

```meta-bind-button
label: Not Oluştur
icon: ""
hidden: false
class: ""
tooltip: ""
id: ""
style: primary
actions:
  - type: command
    command: quickadd:choice:28946aa4-6ae1-4106-bb82-ac966cf6caf6
```

## Gelen Kutusu
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "01 - Inbox"
WHERE kaynak = [[<% tp.file.title %>]]
SORT olusturma_tarihi DESC
```
## Projeler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "02 - Projects"
SORT olusturma_tarihi DESC
```
## İlgi Alanları
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "03 - Areas"
SORT olusturma_tarihi DESC
```
## Kaynaklar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "04 - Resources"
SORT olusturma_tarihi DESC
```
## Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Notes"
WHERE kaynak = [[<% tp.file.title %>]]
SORT olusturma_tarihi DESC
```