#  SQL Dersleri 

---

##  Temel SQL Komutları
- **CREATE DATABASE / CREATE TABLE** → Yeni veritabanı ve tablo oluşturma  
- **INSERT INTO** → Tabloya veri ekleme  
- **SELECT** → Veri sorgulama  
- **UPDATE** → Var olan veriyi güncelleme  
- **DELETE** → Veri silme  
- **DROP** → Tablo veya veritabanı silme  

---

##  Sorgu Operatörleri ve Filtreleme
- **WHERE** → Koşullu sorgulama  
- **AND / OR / NOT** → Mantıksal operatörler  
- **LIKE / IN / BETWEEN** → Gelişmiş filtreleme  
- **ORDER BY** → Sıralama  
- **GROUP BY / HAVING** → Gruplama ve filtreleme  

---

##  İlişkisel Yapılar
- **JOIN (INNER, LEFT, RIGHT, FULL)** → Tablolar arası ilişki kurma  
- **UNION / UNION ALL** → Sorgu sonuçlarını birleştirme  

---

##  Fonksiyonlar ve Veri Tipleri
- **COUNT, SUM, AVG, MIN, MAX** → Toplama ve istatistiksel işlemler  
- **CAST / CONVERT** → Veri tipi dönüşümleri  
- **GETDATE(), DATEPART(), DATEDIFF()** → Tarih fonksiyonları  

---

##  Ekstra Konular
- **PRIMARY KEY / FOREIGN KEY / CONSTRAINT** → Veri bütünlüğü kuralları  
- **INDEX** → Performans artırma  
- **VIEW** → Sanal tablo oluşturma  
- **STORED PROCEDURE / FUNCTION** → Saklı yordamlar ve fonksiyonlar  
- **TRIGGER** → Otomatik tetikleyiciler  

---

## 📝 Örnek SQL Komutları

---

###  SELECT – Veri Sorgulama
```sql
SELECT FirstName, LastName 
FROM Employees 
WHERE Department = 'IT';
```
- Employees tablosundan sadece IT departmanındaki çalışanların ad ve soyadlarını listeler.
 
 ---

### INSERT INTO – Veri Ekleme
```sql
INSERT INTO Employees (FirstName, LastName, Department, HireDate)
VALUES ('Ahmet', 'Yılmaz', 'IT', '2025-10-01');
```
- Employees tablosuna yeni bir çalışan kaydı ekler.
 
---
### UPDATE – Veri Güncelleme
```sql
UPDATE Employees
SET Department = 'HR'
WHERE EmployeeID = 5;
```
- EmployeeID değeri 5 olan çalışanın departmanını HR olarak günceller.

---
### DELETE – Veri Silme
```sql
DELETE FROM Employees
WHERE Department = 'Stajyer';
```
- Stajyer departmanındaki tüm kayıtları siler.
 
---
### INNER JOIN – Tabloları Birleştirme
```sql
SELECT e.FirstName, e.LastName, d.DepartmentName
FROM Employees e
INNER JOIN Departments d ON e.DepartmentID = d.DepartmentID;
```
- Employees ve Departments tablolarını birleştirerek çalışanların hangi departmanda olduğunu gösterir.

---

##  Kaynak
👉 [Kusha Mühendislik Yazılım – SQL Dersleri Oynatma Listesi](https://www.youtube.com/playlist?list=PLW1Q9KyCBcbRuKW77t5McRJHyITU85VaA)

---

### ✨ Not
Bu özet, oynatma listesindeki derslerde işlenen konuların kısa bir rehberidir.  
