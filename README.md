# Saf PHP ile Kurumsal ERP Sitesi

Bu proje 2025-2026 yılları arasında BASER TELEKOMÜNİKASYON firmasında lise stajımı yaparken geliştirdiğim bir yönetim paneli sistemidir

Hiçbir framework kullanmadan saf php ile MVC yapısı oluşturulmuştur.

Şu anki hali alfa sürümü sayılabilir. Güvenlik önlemleri ve görünüş iyileştirmeleri yapılabilir.

Bu haliyle;

Admin panelinden yeni kullanıcı eklenebilir (kullanıcılar kayıt olamaz yalnızca adminin verdiği kullanıcı adı ve şifre ile giriş yapabilir).
Sistemde Üye ve Admin olmak üzere iki tane rol tanımlanmıştır. 
Üyeler sadece okuyabilir, Adminler ise her yetkiye sahiptir.
Bütün tanımlamalarda CRUD işlemi yapılabilmekte.
CSRF, SQL INJECTION, SESSION MANUPLATING gibi saldırılara karşı temel önlemler alınmıştır ancak UI/UX tarafında geliştirmeler yapılabilir.

Gösterge panelinde verilerin kabaca hali gösterilmektedir şu an gösterilen tek veri kullanıcı sayısıdır.
Personel sayfasında ilçe ve birim başlıklarında personel sayıları tutulmaktadır. Personeller özelinde okuma, ekleme, güncelleme ve silme (CRUD) işlemleri yapılabilir. Personel eklerken detaylı veriler girilmektedir. 
Projeler sayfasında projeler il bazlı olarak sekmelenmiştir. Her il sekmesinde projelerin detayları listelenmiştir. 
Kullanıcı yönetimi sayfasında kullanıcı ekleme, silme, güncelleme gibi işlemler yapılmaktadır. 
Finans başlığı altında detaylı finans işlemleri sıralanmıştır. SAT->SAS->FATURA->ÖDEME işlem sırası profesyonel şekilde hazırlanmıştır. İlk olarak SAT talebi oluşturulur, SAS bu talebi onaylar, FATURA bu işlemi resmileştirip faturasını keser, ÖDEME de ödemeyi yaparak bu döngüyü sonlandırır. Hakediş özeti eklenebilir, güncellenebilir, silinebilir. SAT yetkilisi tanımlanabilir, "GLOBAL DÖNEM" (2024, 2025, 2026 ...) tanımlanabilir. 
Tanımlamalar sekmesinde, ŞEHİR, BİRİM, DEPARTMAN departman tanımlamaları eklenebilir, düzenlenebilir, silinebilir. 
Son olarak oturum kapatılabilir. 

