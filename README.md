# 🌍 MeteoFace | 3D Weather Analysis Dashboard

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Technology](https://img.shields.io/badge/Mapbox-GL%20JS-blueviolet)
![API](https://img.shields.io/badge/API-Open--Meteo-orange)

**MeteoFace**, modern web teknolojileri kullanılarak geliştirilmiş, 3D küre üzerinde çalışan interaktif bir meteorolojik analiz panelidir. Standart hava durumu uygulamalarının aksine, **izobar (eş basınç) analizi**, **rüzgar vektörleri** ve **atmosferik tahminleri** görselleştirerek profesyonel bir deneyim sunar.

[🔴 CANLI DEMO İÇİN TIKLA](https://www.meteoface.com/) 

---

## 📸 Ekran Görüntüleri

| Genel Görünüm (Karanlık Mod) |
| ![Main View] screenshot1.png) |

---

## ✨ Temel Özellikler

* **🌍 3D İnteraktif Küre:** Mapbox GL JS altyapısı ile tamamen döndürülebilir, yakınlaştırılabilir dünya haritası.
* **⚡ Canlı Veri Akışı:** Open-Meteo API kullanılarak çekilen anlık (Real-time) sıcaklık, rüzgar, nem ve basınç verileri.
* **🔴 AB / 🔵 YB Analizi:** Harita üzerindeki en düşük (Alçak Basınç) ve en yüksek (Yüksek Basınç) merkezlerin otomatik tespiti ve işaretlenmesi.
* **🇹🇷 Türkiye Modu:** Tek tuşla Türkiye'ye odaklanma ve 81 ilin verisini anında analiz etme yeteneği.
* **⏳ Zaman Yolculuğu:** 48 saatlik tahmin verileri arasında gezinebilmeyi sağlayan interaktif zaman çubuğu (Time Slider).
* **🎨 Glassmorphism UI:** Modern, şeffaf ve kullanıcı dostu arayüz tasarımı.

---

## 🛠️ Kullanılan Teknolojiler

Bu proje, herhangi bir Backend (Sunucu) bağımlılığı olmadan, tamamen **Vanilla JavaScript** ile geliştirilmiştir.

* **HTML5 & CSS3:** Modern Flexbox/Grid yapısı ve CSS değişkenleri.
* **JavaScript (ES6+):** Asenkron veri çekme (Async/Await), DOM manipülasyonu.
* **Mapbox GL JS:** WebGL tabanlı harita motoru.
* **Turf.js:** Coğrafi analiz ve izobar (Isoline) hesaplamaları için matematik motoru.
* **Open-Meteo API:** Ücretsiz, açık kaynaklı meteorolojik veri sağlayıcısı.

---

## 🗺️ Yol Haritası (Gelecek Planları)

- [ ] **Havacılık Modu:** METAR/TAF verilerinin havalimanları üzerine işlenmesi.
- [ ] **Radar Katmanı:** Yağış bulutlarının harita üzerine hareketli (GIF) olarak eklenmesi.

---

## 👨‍💻 Geliştirici

**SilverMasterpiece**

* [GitHub Profilim](https://github.com/silvermasterpiece)
* [LinkedIn Profilim](https://www.linkedin.com/in/an%C4%B1l-g%C3%BCm%C3%BC%C5%9F-39a4a0256)

