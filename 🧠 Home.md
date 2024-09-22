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
## Durumlarına Göre Bileşenler
---
### Eklenenler
```dataview
TABLE file.folder as "Klasör", olusturma_tarihi as "Oluşturma Tarihi"
FROM #durum/eklendi 
where arsiv_mi = false and file.folder != "01 - Templates"
SORT file.folder ASC, olusturma_tarihi DESC
```
### Devam Edenler
```dataview
TABLE file.folder as "Klasör", olusturma_tarihi as "Oluşturma Tarihi"
FROM #durum/devam-ediyor  
where arsiv_mi = false and file.folder != "01 - Templates"
SORT file.folder ASC, olusturma_tarihi DESC
```
### Tamamlananlar
```dataview
TABLE file.folder as "Klasör", olusturma_tarihi as "Oluşturma Tarihi"
FROM #durum/tamamlandi  
where arsiv_mi = false and file.folder != "01 - Templates"
SORT file.folder ASC, olusturma_tarihi DESC
```

## Tüm Bileşenler
---
### Yaşam Alanları
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "03 - Yaşam Alanları"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```
### Beceriler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "04 - Beceriler"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```
### Projeler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Projeler"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```
### Kaynaklar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "06 - Kaynaklar"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```
### Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "07 - Notlar"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```
### İçerikler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "08 - İçerikler"
where arsiv_mi = false
SORT olusturma_tarihi DESC
```

## Arşivlenenler
---
### Yaşam Alanları
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "03 - Yaşam Alanları"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```
### Beceriler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "04 - Beceriler"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```
### Projeler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "05 - Projeler"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```
### Kaynaklar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "06 - Kaynaklar"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```
### Notlar
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "07 - Notlar"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```
### İçerikler
```dataview
TABLE olusturma_tarihi as "Oluşturma Tarihi"
FROM "08 - İçerikler"
where arsiv_mi = true
SORT olusturma_tarihi DESC
```