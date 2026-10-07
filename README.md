# Sığır Sağlık Rehberi (Offline-First & PWA)

🌐 **Canlı Yayın (Web & Mobil PWA):** [https://mserman90.github.io/sigir-saglik-rehberi/](https://mserman90.github.io/sigir-saglik-rehberi/)  
📦 **GitHub Deposu:** [https://github.com/mserman90/sigir-saglik-rehberi](https://github.com/mserman90/sigir-saglik-rehberi)  
📖 **Detaylı Kullanım Kılavuzu:** [KULLANIM_KILAVUZU.md](./KULLANIM_KILAVUZU.md)

Bu uygulama, **en eski ve en basit akıllı telefonlardan masaüstü/dizüstü bilgisayarlara kadar** her cihazda **hiçbir internet bağlantısı veya sunucu kurulumu gerektirmeden** çalışan, Progressive Web App (PWA) mimarili çevrimdışı bir sürü ve besi sağlığı asistanıdır.

---

## 🚀 Nasıl Çalıştırılır & Kurulur?

1. **Cep Telefonunda (Android / iOS):**
   - [https://mserman90.github.io/sigir-saglik-rehberi/](https://mserman90.github.io/sigir-saglik-rehberi/) adresini açın.
   - Tarayıcı menüsünden *"Ana Ekrana Ekle"* (Add to Home Screen) veya *"Uygulamayı Yükle"* seçeneğine dokunun.
   - Uygulama telefonun hafızasına yüklenir. İnternetsiz dağda, yaylada ve bodrum ahırda bağımsız çalışır.

2. **Bilgisayarda:**
   - [`index.html`](./index.html) dosyasına çift tıklayarak tarayıcınızda doğrudan çalıştırabilirsiniz.

---

## 🧭 Saha Öncelikli Buton ve Menü Hiyerarşisi

Uygulama arayüzü, ahır şartlarındaki **klinik aciliyet** ve eldivenli kullanıma göre optimize edilmiştir:
- **Alt Menü (Bottom Navigation):** `📊 Ahır Özeti` $\rightarrow$ `🆘 İlk Yardım` $\rightarrow$ `🩺 Muayene` $\rightarrow$ `💊 İlaç & Süt` $\rightarrow$ `🥛 Sağımcı` $\rightarrow$ `🌾 Yem & Geviş` $\rightarrow$ `🍼 Buzağı` $\rightarrow$ `🚛 Dana Giriş` $\rightarrow$ `⚖️ Kilo/CAAG` $\rightarrow$ `🩸 Tohum/Doğum` $\rightarrow$ `📅 Aşı Takvimi` $\rightarrow$ `💰 Zarar Defteri`.
- **Hızlı İşlemler Paneli:** Hayat kurtaran `🆘 Acil İlk Yardım` en üstte çift genişlikli buton olarak öne çıkarılmıştır.
- **Eldiven & Saha Uyumu:** Min. 48px dokunma alanları, koyu mod desteği ve yüksek kontrastlı renkler.

---

## 📱 Barındırdığı Temel Saha Modülleri

0. **📷 Kamerayla Küpe Okuma (Barkod & QR):**
   - Hayvan arama, muayene, ilaç/İKAS, sağımcı kontrolü ve yeni hayvan ekleme ekranlarında yerel kamera kütüphanesiyle küpeleri otomatik okur (%100 offline).

1. **📊 Gösterge Paneli (Dashboard):**
   - Toplam sürü mevcudu, karantina, ilaçlı süt engelleri (İKAS), mezbaha/kesim kilitleri ve yaklaşan aşılar.

2. **🆘 Acil İlk Yardım & Besi Hastalıkları (Merck Vet Entegreli):**
   - **Canlı Ağırlık Adrenalin Hesaplayıcı:** Anafilaksi durumunda anında mL dozu verir.
   - **Hayat Kurtaran Kartlar:** Aşı şoku, işkembe gaz patlaması (timpani/trokar), rahim düşmesi (prolapsus), doğum felci (süt humması), patates/pancar boğulması, şiddetli kanama, buzağı canlandırma, sıcak çarpması, üre zehirlenmesi.
   - **Besi Danası Hastalıkları:** **CCN / Polio** (B1 Tiamin eksikliği & yıldız gözleme), **İdrar Taşı / Sidik Zoru** (ürolitiyazis & amonyum klorür) ve **Besi Laminitisi** (arpa vurması & tırnak yanması).

3. **🩺 Saha Triyajı & DART Skorlama:**
   - Rektal ateş ölçümü, nabız, solunum, işkembe hareketleri ve BRD/DART algoritmasıyla otomatik vaka derecelendirmesi.

4. **💊 İKAS (İlaç Kalıntı Arınma Süresi) & Süt/Et Kilitleme:**
   - Genişletilmiş veteriner ilaç kataloğu (Merck Vet 11. Baskı). Süt ve et arınması için saat/dakika canlı geri sayım; kombine ilaçlarda en uzun süreyi kilitler.

5. **🥛 Sağımcı Ekranı (Büyük Puntolu Hızlı Kontrol):**
   - Sağımhane personeli için tek bakışta dev harflerle "🟢 SAĞIMA UYGUN" veya "🔴 BU İNEĞİ TANKA SAĞMA" onayı. Mezbaha kesim kilitleri anlık listelenir.

6. **🌾 Yemlik Yönetimi, İşkembe & Asidoz (SARA) Takibi:**
   - Geviş getirme indeksi ($\ge \%58$ kuralı), tezek kıvamı ve tüm sürü için yemliğe katılacak günlük sodyum bikarbonat dozu hesabı.

7. **🍼 Buzağı Hayatta Tutma & Ağız Sütü:**
   - İlk 2 saat altın kuralı, Brix refraktometre kalite ölçümü ve buzağı ishalinde su kaybı (kuruma) / damar-ağız can suyu hesabı.

8. **🚛 Yeni Dana Giriş & Besiye Alıştırma Protokolü:**
   - Kamyondan inişte ilk 2 saat kuru ot, tuzlu-pekmezli can suyu karşılama protokolü, metafilaksi ciğer kalkanı ve 21 günlük kademeli yem geçiş takvimi.

9. **⚖️ Canlı Kilo & Besi CAAG Takip Motoru:**
   - Baskül tartımı veya şerit metreyle *Schaeffer Formülü* ile kilo tespiti; Günlük Canlı Ağırlık Artışı (CAAG) takibi, karkas randımanı ve kesim geliri projeksiyonu.

10. **🩸 Üreme, Tohumlama & Doğum Çarkı:**
    - 21. gün kızgınlık dönüşü, 40. gün ultrason/gebelik, 220. gün kuruya alma ve 280. gün beklenen doğum tarihi hesaplayıcısı.

11. **📅 Akıllı Aşı Takvimi & Hatırlatıcı:**
    - Şap, Bruselloz, Çiçek, BRD karma ve buzağı ishal aşıları için 21/30 gün rapel takibi ve TÜRKVET kuralları.

12. **💰 Hastalık Masrafı & Dökülen Süt Zarar Defteri:**
    - Veteriner, ilaç ve dökülen sütün litre fiyatına göre parasal maliyetini hesaplayıp deftere işler.

---

## 💾 Çevrimdışı Veri Güvenliği & Yedekleme
- Tüm veriler telefonunuzun yerel hafızasında (`localStorage`) saklanır.
- Sağımcı ekranından tek tıkla JSON formatında yedek alabilir, başka bir telefona verilerinizi kayıpsız aktarabilirsiniz.
