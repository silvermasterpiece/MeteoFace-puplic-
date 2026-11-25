<p align="center">
  <img src="logo.png" alt="MeteoFace" width="96">
</p>

<h1 align="center">MeteoFace</h1>

<p align="center">
  <b>Hava durumu haritası · Uydu · Havacılık · Denizcilik</b><br>
  Meteoroloji için tek ekranda, mobil uyumlu, ücretsiz platform.
</p>

<p align="center">
  <a href="https://meteoface.com/"><b>🔴 Canlı siteyi aç → meteoface.com</b></a>
</p>

<p align="center">
  <img alt="Durum" src="https://img.shields.io/badge/Durum-Aktif-success">
  <img alt="Mapbox GL JS" src="https://img.shields.io/badge/Mapbox-GL%20JS%20v3-blueviolet">
  <img alt="Veri" src="https://img.shields.io/badge/Veri-Open--Meteo%20%C2%B7%20EUMETSAT%20%C2%B7%20NOAA-orange">
  <img alt="Mobil" src="https://img.shields.io/badge/Mobil-uyumlu-informational">
</p>

---

## Nedir?

**MeteoFace**, sinoptik meteoroloji bakış açısıyla geliştirilmiş bir web platformudur. Amaç, bir meteorologun günlük olarak aradığı şeyi tek bakışta vermek: **nerede ne oluyor**. Dört modülden oluşur ve hepsi aynı arayüz diliyle, aynı ayarlarla çalışır.

| Modül | Ne gösterir |
|---|---|
| 🗺️ **Hava durumu haritası** | Sıcaklık, rüzgâr ve basınç katmanları, izobarlar, alçak/yüksek basınç merkezleri, 48 saatlik tahmin, şehir kartları |
| 🛰️ **Uydu** | Meteosat görüntüleri, 10 dakikada bir yenilenen kareler, animasyon, yıldırım katmanı |
| ✈️ **Havacılık** | Türkiye meydanları için METAR, TAF, uçuş kategorisi ve SIGMET; Türkçe rasat çözümleme |
| ⚓ **Denizcilik** | Dalga, soluğan, deniz suyu sıcaklığı, Beaufort ve gelgit; limanlar ve kıyı noktaları |

---

## ✨ Öne çıkan özellikler

### Hava durumu haritası
* **3B küre veya düz harita:** Mapbox GL JS ile döndürülebilir, yakınlaştırılabilir.
* **Dört katman:** Hava (hadise ikonları), Sıcaklık, Rüzgâr, Basınç; renkler ve lejant seçili katmana göre değişir.
* **İzobarlar ve AB/YB:** Basınç alanından otomatik izobarlar ve alçak/yüksek basınç merkezleri.
* **Renk alanları (isteğe bağlı):** Türkiye ve çevresi için sıcaklık, basınç ve rüzgâr hızı; Katmanlar panelinden açılıp kapanır, opaklığı ayarlanır.
* **48 saatlik zaman çubuğu:** Haritayı ve kartları saat saat ileri alın, oynatın; klavye ile de kontrol edilir.
* **Şehir kartı:** Anlık değerler, 24 saatlik şerit, uydu sayfasına ve (kıyı illeri için) deniz durumuna kısayol.
* **Türkiye modu:** Tek tuşla 81 ilin verisi.
* **Altlık seçenekleri:** Gerçekçi, Koyu, Açık, Gece 3B.

### Uydu
* Meteosat'tan **10 dakikada bir** yenilenen kareler; GeoColour, kızılötesi, bulut türü, toz, sis, yağış ve **yıldırım** katmanları.
* Kare kare animasyon, zaman çizelgesi, paylaşılabilir görünüm ve sinema modu.

### Havacılık
* Türkiye'deki meydanlar haritada **VFR / MVFR / IFR / LIFR** renkleriyle görünür.
* Ham METAR/TAF **Türkçe olarak çözülür**: rüzgâr, görüş, hadise, bulut, sıcaklık, QNH, tehlike uyarıları.
* TAF için saatlik **kategori şeridi**; uçuş bilgi bölgeleri için **SIGMET** poligonları.
* Herkese açık kaynaklarda rasatı olmayan (ör. askeri) meydanlar için **yedek kaynak zinciri** ve, hiçbirinde yoksa, **açıkça "model tahmini" etiketli** değerler.
* `#LTAC` gibi paylaşılabilir adresler.

### Denizcilik
* Limanlar, boğazlar ve kıyı noktaları için dalga yüksekliği, soluğan, deniz suyu sıcaklığı, akıntı, **Beaufort** ölçeği ve gelgit.
* Tehlike şeridi ve saatlik/günlük tahmin tabloları.

### Her yerde ortak
* **Ortak ayarlar:** sıcaklık, rüzgâr, basınç ve mesafe birimleri; yerel/UTC saat; altlık; 3B küre; hareketi azaltma; Türkçe/İngilizce.
* **Mobil öncelikli:** telefonda alt sekme çubuğu ve alttan açılan paneller; 360 px'ten geniş ekranlara kadar test edildi.
* **PWA:** ana ekrana eklenebilir, statik dosyalar önbelleğe alınır.
* **Hafif:** çatı yazılımı (framework) yok; ortak kod bir kez indirilip önbellekte tutulur.

---

## 🛠️ Teknolojiler

* **JavaScript (ES modülleri), HTML5, CSS3:** framework kullanılmadan; esbuild ile paketlenir.
* **Mapbox GL JS v3:** WebGL tabanlı harita motoru (küre, Standard altlıklar).
* **Vercel:** statik barındırma ve havacılık verisi için küçük bir sunucu fonksiyonu (CDN önbellekli aracı).
* **Veri kaynakları (hepsi ücretsiz):**

| Kaynak | Kullanım |
|---|---|
| [Open-Meteo](https://open-meteo.com) | Hava ve deniz tahmin modelleri, renk alanları, şehir verileri |
| [EUMETSAT](https://www.eumetsat.int) | Meteosat uydu görüntüleri ve yıldırım ürünleri |
| [NOAA Aviation Weather Center](https://aviationweather.gov) | METAR, TAF, uluslararası SIGMET |
| [OGIMET](https://www.ogimet.com) | AWC'de bulunmayan meydanlar için METAR/TAF yedeği |
| [MGM](https://rasat.mgm.gov.tr) | Meteoroloji Genel Müdürlüğü'nün herkese açık rasat sayfası; son yedek |
| [VATSIM](https://metar.vatsim.net) | Aracı sunucuya ulaşılamazsa METAR yedeği |

---

## 🗺️ Yol haritası

- [x] Havacılık modu: METAR/TAF/SIGMET
- [x] Uydu modülü: Meteosat, yıldırım
- [x] Denizcilik modülü
- [x] Ortak ayarlar, mobil uyum, yeni arayüz
- [ ] Arazi düzeltmeli, daha yüksek çözünürlüklü sıcaklık alanı
- [ ] Olası cephe bölgelerinin gösterimi (sıcaklık gradyanı ve rüzgâr dönüşü)
- [ ] Rüzgâr akış çizgileri
- [ ] Denizcilik değerlerinde ortak birim tercihleri

---

## ⚠️ Sorumluluk reddi

MeteoFace resmî bir meteoroloji hizmeti değildir. Model tahminleri ve otomatik çıkarımlar (izobarlar, tahmini uçuş kategorisi vb.) bilgilendirme amaçlıdır. Uçuş ve seyir planlaması için MGM ve AIS gibi resmî kaynakları kullanın.

> Bu depo yalnızca tanıtım amaçlıdır; kaynak kodu burada yer almaz.

<!--
Ekran görüntüsü eklemek için görüntüleri `docs/` klasörüne koyup şu satırları açın:

| Hava durumu | Uydu |
|---|---|
| ![Harita](docs/harita.png) | ![Uydu](docs/uydu.png) |
| **Havacılık** | **Denizcilik** |
| ![Havacılık](docs/havacilik.png) | ![Denizcilik](docs/denizcilik.png) |
-->

---

## 👨‍💻 Geliştirici

**Anıl Gümüş** — Meteorolog · Yazılım geliştirici
20 yılı aşkın havacılık meteorolojisi tecrübesiyle geliştirildi.

* [GitHub](https://github.com/silvermasterpiece)
* [LinkedIn](https://www.linkedin.com/in/an%C4%B1l-g%C3%BCm%C3%BC%C5%9F-39a4a0256)
* [meteoface.com](https://meteoface.com)

© 2026 MeteoFace
