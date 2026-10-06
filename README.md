# Sığır Sağlık, Saha Triyajı ve İKAS Sistemi (Offline-First)

🌐 **Canlı Yayın (Web & Mobil):** [https://mserman90.github.io/sigir-saglik-rehberi/](https://mserman90.github.io/sigir-saglik-rehberi/)  
📦 **GitHub Deposu:** [https://github.com/mserman90/sigir-saglik-rehberi](https://github.com/mserman90/sigir-saglik-rehberi)

Bu uygulama, **en eski ve en basit akıllı telefonlardan masaüstü/dizüstü bilgisayarlara kadar** her cihazda **hiçbir internet bağlantısı veya sunucu kurulumu gerektirmeden** çalışmak üzere tasarlanmıştır.

## 🚀 Nasıl Çalıştırılır?

1. **Bilgisayarda:**
   - [`index.html`](file:///C:/Users/mert/.gemini/antigravity/scratch/sigir-saglik-rehberi/index.html) dosyasına çift tıklayın (Chrome, Edge, Firefox veya Safari ile doğrudan açılır).

2. **Cep Telefonunda (Android / iOS):**
   - Bu `index.html` dosyasını WhatsApp, Bluetooth veya USB kablosu ile telefona atın.
   - Dosyaya dokunup herhangi bir tarayıcıyla açın.
   - **Ana Ekrana Ekleme (İsteğe Bağlı):** Tarayıcı menüsünden *"Ana Ekrana Ekle"* (Add to Home Screen) dediğinizde telefonunuzda tıpkı App Store / Play Store'dan yüklenmiş bir uygulama gibi tam ekran ikonla çalışır.

---

## 📱 Barındırdığı 6 Temel Saha Modülü

1. **📊 Gösterge Paneli (Dashboard):**
   - Toplam sürü sayısı, karantinadaki hayvanlar, aktif kalıntılı süt engelleri (İKAS) ve yaklaşan aşılar.
   - Kritik kırmızı alarm başlığı: Antibiyotikli ineklerin küpe listesi.

2. **🚨 Saha Triyajı & DART Skorlama:**
   - Rektal ateş (38.0–39.3 °C referansı, >39.5 °C alarmı).
   - Kalp, solunum, rumen motilitesi ve dehidrasyon kontrolü.
   - **BRD için DART Algoritması:** Depresyon (0–3), İştah (0–3), Solunum (0–3), Ateş (0–3). Skor $\ge 4$ ise otomatik tedavi ve karantina tetikleyicisi; $\ge 7$ ise sistemik şok/agresif müdahale kararı.

3. **💊 İKAS (İlaç Kalıntı Arınma Süresi) & Farmakoloji (Merck Vet 11. Baskı Entegreli):**
   - **Genişletilmiş İlaç Kataloğu:** Florfenikol, Meloksikam, Fluniksin, Ketoprofen, Seftiofur, Tulatromisin (Tablo 50), Tilmikosin (Tablo 50), Tilosin (Tablo 50), Prokain Penisilin G, Amoksisilin, Oksitetrasiklin LA (Tablo 43), Sodyum Sefapirin Meme İçi, Sülfametazin (Tablo 42), Enrofloksasin ve İvermektin.
   - Laktasyondaki süt ineklerinde yasaklı ilaçlar için kırmızı bariyer uyarısı.
   - **Kombine Tedavi Kuralı:** Birden fazla ilaç yapıldığında otomatik olarak en uzun İKAS süresini baz alma.
   - Canlı saat/dakika geri sayımı.

4. **📅 Akıllı Aşı Takvimi & Rapel Motoru:**
   - Şap (FMD), Bruselloz (S19 - Dişi 3-6 ay), Sığır Çiçeği (LSD), BRD karma ve Buzağı İshali aşıları.
   - Rapel (tekrar) tarihini otomatik hesaplama (30 gün, 21 gün kuralı).
   - TÜRKVET resmi kayıt ve sevk 21 gün kuralı hatırlatması.

5. **🆘 Acil İlk Yardım Rehberi & Protokoller (Merck Vet 11th Ed.):**
   - **Adrenalin Hesaplayıcı:** Canlı ağırlığı girildiğinde (her 45 kg için 1 mL Epinefrin 1:1000 / 0.01-0.02 mg/kg) anında mL dozu verir.
   - **Akut Rumen Şişkinliği (Timpani):** Mide sondası, köpük söndürücü ajanlar (Poloxalene 25-50 g PO, 250-500 mL bitkisel yağ drench) ve boğulma tehlikesinde trokar uygulaması.
   - **Uterus Prolapsusu (Rahim Düşmesi):** Organı yükseltme, nemli bezle sarma, ödem için gliserol, kornu uçlarının tam repozisyonu ve Oksitosin tonus protokolü.
   - **Süt Humması (Hipokalsemi / Parturient Paresis):** Evre 1-3 sınıflandırması, %23 Kalsiyum Boroglukonat (10-20 dk yavaş IV perfüzyon), kardiyotoksisite uyarısı ve relaps önleyici oral Ca jeli.

6. **🥛 Sade Sağımcı Ekranı:**
   - Sağımhane personeli için küpe numarasını girdiği anda dev puntolarla:
     - 🔴 **BU İNEĞİ TANKA SAĞMA!** (Antibiyotikli)
     - 🟢 **SAĞIMA UYGUN** (Temiz)
   - Tanka sağılması yasak olan tüm ineklerin anlık canlı listesi.

---

## 💾 Çevrimdışı Veri Güvenliği
- Tüm kayıtlar telefonun veya bilgisayarın dahili hafızasında (`localStorage`) saklanır.
- İnternet gitse de, telefon uçak moduna alınsa da hiçbir veri kaybolmaz.
