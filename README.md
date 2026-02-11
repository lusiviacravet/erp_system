# 🏢 Kurumsal ERP Sistemi (Saf PHP & MVC)

![PHP](https://img.shields.io/badge/PHP-7.4%2B-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-MVC-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Alpha-red?style=for-the-badge)

<div align="center">
  <img src="https://github.com/user-attachments/assets/5286768a-6484-4d3f-9040-171be7dcf0b3" alt="ERP Dashboard Genel Bakış" width="100%">
</div>

## 📄 Proje Hakkında

Bu proje, **2025-2026** yılları arasında **BASER TELEKOMÜNİKASYON** firmasında gerçekleştirdiğim lise stajım kapsamında geliştirilmiştir. 

Kurumsal ihtiyaçları karşılamak amacıyla, **hiçbir hazır Framework kullanılmadan**, tamamen **Saf (Native) PHP** ile kendi **MVC (Model-View-Controller)** yapım oluşturularak yazılmıştır. Proje şu an Alfa sürümündedir; temel fonksiyonların tamamı çalışmakta olup, UI/UX ve ileri seviye güvenlik geliştirmelerine açıktır.

## 🚀 Özellikler

### 🛠 Teknik Altyapı
* **MVC Mimarisi:** Kodun okunabilirliğini ve sürdürülebilirliğini artıran katmanlı yapı.
* **Güvenlik:**
    * 🛡️ SQL Injection koruması.
    * 🔒 CSRF (Cross-Site Request Forgery) önlemleri.
    * 🚫 Session Manipulation engelleme.

### 👤 Kullanıcı & Rol Yönetimi (RBAC)
* **Admin ve Üye Rolleri:**
    * **Admin:** Tam yetkili (Okuma, Yazma, Güncelleme, Silme).
    * **Üye:** Sadece görüntüleme (Read-Only) yetkisi.
* **Kapalı Devre Kayıt:** Dışarıdan üye alımı kapalıdır. Kullanıcılar yalnızca Admin tarafından oluşturulabilir.
* **Güvenli Giriş:** Kullanıcı adı ve şifre ile oturum yönetimi.

### 💼 Modüller

#### 1. Personel Yönetimi (İnsan Kaynakları)
* Personellerin detaylı kaydı (TC, İletişim, Eğitim, Departman vb.).
* Şehir, İlçe ve Birim bazlı personel sayıları ve listeleme.
* CRUD işlemleri (Ekle, Sil, Düzenle).

#### 2. Finans Yönetimi (Satın Alma Döngüsü)
Profesyonel satın alma ve ödeme döngüsü eksiksiz olarak kurgulanmıştır:
1.  **SAT (Satın Alma Talebi):** Talep oluşturulur.
2.  **SAS (Satın Alma Siparişi):** Talep onaylanarak siparişe dönüşür.
3.  **FATURA:** İşlem resmileşir ve fatura kaydı girilir.
4.  **ÖDEME:** Süreç ödeme ile sonlandırılır.
* *Ekstra:* Hakediş özetleri ve Global Dönem (2025, 2026...) tanımlamaları.

#### 3. Proje Yönetimi
* İl bazlı sekmeli yapı.
* Projelerin detaylı listelenmesi ve takibi.

#### 4. Tanımlamalar
* Dinamik Şehir, Birim ve Departman tanımlamaları.

---

## 📸 Ekran Görüntüleri

### 🔐 Giriş Ekranı
Sade ve kullanıcı dostu giriş arayüzü.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0c2b6bc6-8043-4dca-a645-b9fced4317e4" />


### 👥 Personel Listesi ve İstatistikler
Şehir bazlı personel dağılımı ve detaylı personel listesi.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d6dc1578-1396-4c45-b180-844d2dba119b" />



### ➕ Personel Ekleme Formu
Detaylı veri girişi sağlayan personel kartı oluşturma ekranı.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/25f0429b-2b25-4063-86a4-ba9e2aefb73c" />


### 🛠 Kullanıcı Yönetimi
Admin panelinden yeni kullanıcı tanımlama ve rol atama işlemleri.
<img width="1916" height="1079" alt="image" src="https://github.com/user-attachments/assets/0b8fae64-601f-4968-8100-33fb96ba40f5" />


---

## 💻 Kurulum (Geliştirici İçin)

Proje veritabanı bağlantısı için `config` veya `database` klasörü altındaki ayar dosyasını düzenleyin.

1. Repoyu klonlayın.
2. Kök dizindeki `db.sql` veritabanı dosyasını phpMyAdmin vb. üzerinden içeri aktarın.
3. Veritabanı bağlantı ayarlarını (host, dbname, user, password) yapılandırın.
4. Projeyi bir yerel sunucuda (XAMPP, WAMP, Docker vb.) çalıştırın.

## 📝 Yapılacaklar (To-Do)
- [ ] UI/UX tarafında modern CSS framework (Bootstrap/Tailwind) entegrasyonu.
- [ ] Şifrelerin hashlenerek (Argon2 veya Bcrypt) saklanması.
- [ ] Loglama mekanizmasının geliştirilmesi.

---
*Geliştirici: Arda Şeker - 2026*
