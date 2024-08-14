# FirstMicroservice

Bu proje, mikroservis mimarisini öğrenmek amacıyla geliştirilmiş bir örnek uygulamadır. Proje, ürünler, kategoriler ve bir API Gateway (YARP) olmak üzere üç temel mikroservisten oluşur.

## Proje Yapısı

### 1. Products.WebAPI
- **Amaç**: Ürünlerle ilgili CRUD işlemlerini gerçekleştiren bir mikroservistir.
- **Teknolojiler**:
  - Entity Framework Core (SQL Server)
  - ASP.NET Core Web API
  - Docker (Dockerfile mevcut)

### 2. Categories.WebAPI
- **Amaç**: Kategorilerle ilgili CRUD işlemlerini gerçekleştiren bir mikroservistir.
- **Teknolojiler**:
  - Entity Framework Core (PostgreSQL)
  - ASP.NET Core Web API
  - Docker (Dockerfile mevcut)

### 3. Gateway.YARP
- **Amaç**: YARP (Yet Another Reverse Proxy) kullanarak API Gateway işlevi gören bir mikroservistir. Diğer iki mikroservis olan Products ve Categories API'lerine yönlendirme yapar.
- **Teknolojiler**:
  - YARP (Yet Another Reverse Proxy)
  - Docker (Dockerfile mevcut)
