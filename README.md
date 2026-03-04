# mini-user-management

# Mini User Management

**Description:** CRUD API with FastAPI + SQLite and interactive ipywidgets frontend in Google Colab.

---

## 🚀 Proje Hakkında

Bu proje, kullanıcı verilerini eklemek, listelemek, güncellemek ve silmek için basit bir **CRUD (Create, Read, Update, Delete) uygulamasıdır**.  

- Backend: **FastAPI + SQLite**  
- Frontend: **ipywidgets** (Google Colab üzerinde interaktif)  
- Amaç: API mantığını anlamak, interaktif bir frontend ile veri yönetimi yapmak ve Google Colab’da hızlı test etmek.

---

## 💡 Özellikler

1. Kullanıcı ekleme, güncelleme, silme ve listeleme  
2. SQLite veritabanında veri saklama (kalıcı)  
3. Colab üzerinden interaktif frontend ile işlem yapabilme  
4. JSON formatında çıktı gösterme

---

## 📌 Kullanılan Teknolojiler

- [FastAPI](https://fastapi.tiangolo.com/) – Python API framework  
- [SQLite](https://www.sqlite.org/) – Hafif veritabanı  
- [ipywidgets](https://ipywidgets.readthedocs.io/) – Colab / Jupyter interaktif widgetlar  
- [Google Colab](https://colab.research.google.com/) – Uygulamayı çalıştırmak için  

---

## ⚡ Kullanım

1. Google Colab üzerinde projeyi çalıştırın.  
2. Kullanıcı bilgilerini girin ve aşağıdaki butonlarla işlemleri gerçekleştirin:  

- **Kullanıcı Ekle** → Yeni kullanıcı ekler  
- **Güncelle** → ID üzerinden kullanıcı günceller  
- **Sil** → ID üzerinden kullanıcı siler  
- **Listele** → Tüm kullanıcıları gösterir  

3. Çıktılar anlık olarak ekranda JSON formatında görüntülenir.  

---

## 📷 Görselleştirme (Örnek)
{
"users": [
{
"id": 1,
"name": "Sude",
"age": 22,
"job": "Mühendis",
"blood_group": "A+",
"religion": "None",
"car_brand": "Tesla"
},
{
"id": 2,
"name": "Ahmet",
"age": 25,
"job": "Öğretmen",
"blood_group": "B-",
"religion": "Islam",
"car_brand": "BMW"
}
]
}
---

## 🔜 Gelecek Geliştirmeler

- Filtreleme ve arama özelliği (meslek, kan grubu, vs.)  
- JWT ile kullanıcı doğrulama / login sistemi  
- Daha fazla endpoint ve parametre ile genişletme  
- Streamlit veya başka bir frontend framework ile tam görsel arayüz  

---

## 👩‍💻 Nasıl Çalışır?

1. Backend FastAPI ile çalışıyor, TestClient Colab üzerinde HTTP isteklerini taklit ediyor.  
2. ipywidgets frontend, kullanıcıdan veri alıyor ve butonlar aracılığıyla API’ye gönderiyor.  
3. Kullanıcı ekleme, güncelleme, silme ve listeleme işlemleri anlık olarak ekranda JSON formatında görüntüleniyor.  

---

## 📂 Dosya Yapısı

users.db # SQLite veritabanı (Colab’da oluşturulur)
colab_user_management.ipynb # Colab Notebook (Tüm backend + frontend kodları)
README.md # Bu dosya


---

## 💬 Notlar

- Proje tamamen **eğitim amaçlı** ve Colab üzerinde çalışacak şekilde tasarlanmıştır.  
- Daha ileri seviye eklemelerle (JWT, filtreleme, frontend) geliştirilebilir.

---
Gelecek İyileştirmeler

Kullanıcı filtresi ve arama

JWT login ve yetkilendirme

Web tabanlı frontend (Streamlit veya React)

Deploy (Heroku / Railway / Vercel)

---


[Form: Kullanıcı bilgileri] 
        │
        ▼
[Buton: Ekle/Güncelle/Sil/Listele] 
        │
        ▼
[FastAPI Backend] <---> [SQLite DB]
        │
        ▼
[Çıktı Alanı: Güncel Kullanıcı Listesi]


