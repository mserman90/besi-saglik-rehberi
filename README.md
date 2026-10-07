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

## 📱 Barındırdığı Temel Saha Modülleri

0. **📷 Cep Telefonu Kamerasıyla Küpe Okuma (Barkod & QR):**
   - Hayvan arama, Saha Triyajı, İlaç/İKAS girişi, Sağımcı kontrolü ve Yeni Hayvan ekleme ekranlarında yer alan **"📷 Oku"** butonuyla telefon kamerası anında açılır.
   - Kulak küpesindeki barkod veya QR kod okunduğu anda küpe numarası ekrana otomatik aktarılır, titreşimli bildirim verilir ve ilgili hayvanın sağlık durumu anında ekrana gelir.
   - Harici internet bağlantısı gerekmez; yerel kütüphane sayesinde **%100 çevrimdışı** çalışır.

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

4. **💰 Hastalık, Dökülen Süt & Tedavi Maliyet Defteri (Ekonomik Zarar Analizi):**
   - **Gerçek Çiftlik Maliyet Takibi:** Veteriner hekim vizitesi, kullanılan ilaç bedeli ve **antibiyotik nedeniyle imha edilen/dökülen sütün parasal kaybı**.
   - **Kayıp Formülü:** $\text{Zarar} = \text{Veteriner} + \text{İlaç} + (\text{Günlük Süt Litresi} \times \text{Dökülen Gün} \times \text{Süt Satış Fiyatı})$.
   - **Kümülatif Çiftlik Özeti:** Sürü genelinde hastalıklara harcanan toplam para, dökülen toplam süt litresi ve ciro kaybı göstergeleri.

5. **🌾 Yemlik Yönetimi, Rumen & Asidoz (SARA) Takipçisi (Merck Vet 11th Ed.):**
   - **Geviş Getirme (Gefer) İndeksi:** Yatan ineklerde geviş getirme oranı kontrolü (Altın Kural: $\ge \%58$). Tükürük tamponu yetersiz kaldığında erken SARA alarmı.
   - **Dışkı Kıvamı & Sindirilmemiş Tane Analizi (1-5 Skoru):** Zaaijer & Noordhuizen 1-5 dışkı skoru değerlendirmesi ve sindirilmemiş yem/mısır tanesi kaçışı uyarısı.
   - **Yemlik Kalan Yem (Ortus) & Seçme (Sorting) Kontrolü:** İdeal %3-5 kalan yem oranı, açlık veya yem seçme riski analizi.
   - **Sodyum Bikarbonat Tamponlayıcı Doz Hesaplayıcı:** Sürü mevcuduna göre günlük TMR'ye ilave edilecek çuval ve kg bazlı karbonat dozu (150-250 g/baş/gün).

6. **🩸 Üreme, Tohumlama ve Doğum Çarkı (Akıllı Takvim):**
   - **21 Gün Kızgınlık Gözlemi (18–24. Günler):** Tohumlanan ineğin tutmama ihtimaline karşı tekrar kızgınlık döngüsü uyarısı.
   - **40 Gün Gebelik Muayenesi (35–45. Günler):** Ultrason veya rektal muayene hatırlatıcısı.
   - **220 Gün Kuruya Çıkarma (Doğuma 60 Gün):** Sağımı durdurma ve kuru dönem meme içi antibiyotik protokolü alarmı.
   - **245 Gün Kolostrum Aşı Hazırlığı (Doğuma 5–3 Hafta):** Buzağı ishal aşısı uygulama zamanı.
   - **280 Gün Beklenen Doğum & Geri Sayım:** Canlı gün sayacı ve doğum padoğu hazırlık ikazı.

7. **🍼 Buzağı Hayatta Tutma & Kolostrum Kalite Motoru:**
   - **İlk 2 Saat Altın Kuralı:** Doğumdan sonraki ilk 2 saatte canlı ağırlığın %10'u kadar (3–4 Litre) ağız sütü içirilmesi takibi.
   - **Brix Refraktometre Hesaplayıcı:** Ölçülen Brix değerine göre kalite sınıflandırması ($\ge \%22$ Mükemmel antikor - IgG $>50\text{ g/L}$, $\%18-21$ Orta, $<\%18$ Yetersiz/Düşük - dondurulmuş kolostrum çözdür ikazı).
   - **Buzağı İshali Sıvı & Elektrolit Hesaplayıcı:** Dehidrasyon yüzdesi ve buzağı kilosuna göre 24 saatlik sıvı açığı, yaşama payı ve oral/IV serum karar motoru.
   - **Göbek İpi Dezenfeksiyon Protokolü:** Doğum anında ve 1-2 saat sonra %7'lik tentürdiyota daldırma kontrol listesi.

8. **⚖️ Şerit Metre ile Canlı Ağırlık (Kantar Yokken Kilo) Ölçer:**
   - **Schaeffer Formülü:** Mezurayla göğüs çevresi (cm) ve vücut uzunluğu (cm) girildiğinde tahmini ağırlığı ($\pm \%5$ hata payıyla) kg cinsinden hesaplar:
     $$\text{Ağırlık (kg)} = \frac{\text{Göğüs Çevresi}^2 \times \text{Vücut Uzunluğu}}{10838}$$
   - **Otomatik Dozaj & Besleme Çıktıları:** Hesaplanan kiloya göre otomatik olarak Adrenalin ($1\text{ mL} / 45\text{ kg}$), Meloksikam, Fluniksin, Tulatromisin dozlarını ve günlük tahmini kuru madde (KM) tüketim miktarını listeler.
   - **Tek Tıkla Aktarım:** Hesaplanan canlı ağırlık tek butonla acil müdahale formlarına otomatik aktarılır.

7. **📅 Akıllı Aşı Takvimi & Rapel Motoru:**
   - Şap (FMD), Bruselloz (S19 - Dişi 3-6 ay), Sığır Çiçeği (LSD), BRD karma ve Buzağı İshali aşıları.
   - Rapel (tekrar) tarihini otomatik hesaplama (30 gün, 21 gün kuralı).
   - TÜRKVET resmi kayıt ve sevk 21 gün kuralı hatırlatması.

8. **🆘 Acil İlk Yardım Rehberi & Protokoller (Merck Vet 11th Ed.):**
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
