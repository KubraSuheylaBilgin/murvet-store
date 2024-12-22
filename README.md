# Müşteri ve Borç Takip Sistemi

Bu proje, müşterilerin borçlarını ve işlemlerini yönetmek için geliştirilmiş bir web uygulamasıdır. Uygulama, modern frontend ve backend teknolojileri kullanılarak geliştirilmiştir ve kullanıcı dostu bir arayüz ile güçlü bir altyapıyı birleştirmektedir.

---

## Demo

[Demo Video](https://github.com/user-attachments/assets/c915e260-1242-481a-9735-1e3353ef4ff0)

---

## Özellikler

- Müşteri ekleme, silme ve güncelleme işlemleri.
- Müşteri bazında borç ve işlem takip sistemi.
- Ad ve soyad ile filtreleme, büyük-küçük harf ve Türkçe karakter uyumlu arama.
- Toplam borç hesaplama ve ödeme işlemleri.
- React ile kullanıcı dostu ve modern arayüz.
- .NET Core Web API ile güvenilir ve performanslı backend.

---

## Proje Mimarisi

Uygulama, frontend ve backend olarak iki ayrı kısma ayrılmıştır:

---

### Backend (API)

**Teknolojiler:**

- .NET Core Web API
- Entity Framework Core
- RESTful servisler
- SQLite (veritabanı)

**Özellikler:**

- Müşteri ve işlemler için CRUD işlemleri.
- Veritabanı validasyonu ve hata yönetimi.
- Borç hesaplama ve işlemlerin toplam borca etkisi.
- Performans için veritabanı optimizasyonları ve ilişkisel sorgular.
- Versiyonlama ile API sürdürülebilirliği.

**Sonuç:**  
Backend, frontend ile etkileşim kurarak müşteri ve işlem verilerini sağlar. React uygulaması, bu verileri dinamik olarak sunar.

---

### Frontend

**Teknolojiler:**

- React
- Ant Design (UI bileşenleri)
- Axios (API çağrıları için)
- React Router (sayfa geçişleri)

**Özellikler:**

- Modern ve kullanıcı dostu tasarım.
- Dinamik listeleme ve arama fonksiyonları.
- Müşteri detayları sayfası: Tüm işlem ve borç bilgileriyle birlikte.
- Yeni müşteri ekleme ve mevcut müşterileri düzenleme.
- Mobil uyumlu tasarım.

**Sonuç:**  
Frontend, kullanıcıların tüm işlemleri kolayca yapmasını sağlar ve backend ile kusursuz bir şekilde entegre olur.

---

## Klasör Yapısı

```plaintext
project-root/
│
├── backend/
│   ├── API/
│       ├── Controller/
│   ├── Application/
│       ├── Service/
│       ├── DTO/
│       ├── Mapper/
│   ├── Domain/
│       ├── Entity/
│   ├── Infrastructure/
│       ├── Repository/
│   └── ...
│
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── services/
    │   └── ...
