# 🐂 Besi Sağlık Rehberi (Offline-First & PWA)

🌐 **Canlı Yayın (Web & Mobil PWA):** [https://mserman90.github.io/besi-saglik-rehberi/](https://mserman90.github.io/besi-saglik-rehberi/)  
📦 **GitHub Deposu:** [https://github.com/mserman90/besi-saglik-rehberi](https://github.com/mserman90/besi-saglik-rehberi)  
📖 **Detaylı Kullanım Kılavuzu:** [KULLANIM_KILAVUZU.md](./KULLANIM_KILAVUZU.md)

Bu uygulama, **en eski ve en basit akıllı telefonlardan masaüstü/dizüstü bilgisayarlara kadar** her cihazda **hiçbir internet bağlantısı veya sunucu kurulumu gerektirmeden** çalışan, Progressive Web App (PWA) mimarili çevrimdışı bir **besi danacılığı, 21 günlük karşılama, CAAG kilo artışı, Et İKAS mezbaha kilitleri ve acil müdahale** asistanıdır.

---

## 🚀 Nasıl Çalıştırılır & Kurulur?

1. **Cep Telefonunda (Android / iOS):**
   - [https://mserman90.github.io/besi-saglik-rehberi/](https://mserman90.github.io/besi-saglik-rehberi/) adresini açın.
   - Tarayıcı menüsünden *"Ana Ekrana Ekle"* (Add to Home Screen) veya *"Uygulamayı Yükle"* seçeneğine dokunun.
   - Uygulama telefonun hafızasına yüklenir. İnternetsiz dağda, yaylada ve bodrum ahırda bağımsız çalışır.

2. **Bilgisayarda:**
   - [`index.html`](./index.html) dosyasına çift tıklayarak tarayıcınızda doğrudan çalıştırabilirsiniz.

---

## 🧭 Saha Öncelikli Buton ve Menü Hiyerarşisi

Uygulama arayüzü, besi ahırı şartlarındaki **klinik aciliyet** ve eldivenli kullanıma göre optimize edilmiştir:
- **Alt Menü (Bottom Navigation):** `📊 Besi Özeti` $\rightarrow$ `🆘 İlk Yardım` $\rightarrow$ `🩺 Muayene` $\rightarrow$ `🚛 21 Gün Giriş` $\rightarrow$ `⚖️ Kilo / CAAG` $\rightarrow$ `🥩 Et İKAS` $\rightarrow$ `🌾 Yemlik & Asidoz` $\rightarrow$ `📅 Aşı & Parazit` $\rightarrow$ `💰 Masraf Defteri`.
- **Durum Merkezleri (Status Hubs):**
  1. 🚨 **HASTA / ACİL DANA:** İlk yardım, BRD solunum muayenesi ve Et İKAS kilidi.
  2. 🚛 **YENİ DANA GİRİŞ & 21 GÜN KARŞILAMA:** Kamyondan indirme, dinlenme suyu, 21 günlük yem geçişi.
  3. ⚖️ **KİLO, CAAG & MEZBAHA GELİRİ:** Kantar/şerit metre tartımı, günlük canlı ağırlık artışı, %58 karkas randımanı.
  4. 🌾 **YEMLİK, ASİDOZ & MASRAF DEFTERİ:** Tezek skoru, tampon karbonat, aşı takvimi ve fire defteri.

---

## 📱 Barındırdığı Temel Saha Modülleri

0. **📷 Kamerayla Küpe Okuma (Barkod & QR):**
   - Dana arama, muayene, ilaç/İKAS, tartım ve yeni hayvan ekleme ekranlarında yerel kamera kütüphanesiyle küpeleri otomatik okur (%100 offline).

1. **📊 Gösterge Paneli (Dashboard):**
   - Toplam besi mevcudu, mezbaha/kesim kilitleri (Et İKAS), 21 günlük karantina/alıştırma takibi, günü gelen aşılar ve hayvan bazlı kritik alarmlar.

2. **🆘 Acil İlk Yardım & Besi Hastalıkları (Merck Vet Entegreli):**
   - **Besi Danası CCN / Polio:** Yüksek tahıl ve asidoz sonrası B1 Tiamin eksikliği, yıldız gözleme ilk yardımı.
   - **İdrar Taşı & Sidik Zoru (Ürolitiyazis):** Peniste tuz kristalleri, amonyum klorür ve idrar kesesi patlamasını (su karnı) önleme.
   - **Besi Laminitisi (Arpa Vurması / Ayak Yanması):** Akut asidoz ve histamin felcinde yemliği boşaltma, karbonat içirme, yangı giderici ve soğuk su banyosu.
   - **İşkembe Gazı (Timpani):** Mide sondası salma, bitkisel sıvı yağ içirme ve trokarla şişleme.
   - **Yemek Borusu Tıkanması:** Patates/pancar boğulmasında boğaz oluğu masajı.
   - **Canlı Ağırlık Adrenalin Hesaplayıcı:** Aşı şoku durumunda anında mL dozu verir.

3. **🩺 Muayene & DART Solunum Triyajı:**
   - Rektal ateş ölçümü (38.0–39.3°C), nabız, solunum ve DART algoritmasıyla otomatik nakliye humması / zatürre derecelendirmesi.

4. **🚛 Yeni Dana Giriş & 21 Günlük Karşılama Protokolü:**
   - Kamyondan iner inmez ilk 24 saatte kesinlikle kesif yem verilmemesi, ılık can suyu (tuz + karbonat + pekmez), metafilaksi ciğer kalkanı, iç-dış parazit ve kademeli 21 günlük rasyon tablosu.

5. **⚖️ Canlı Ağırlık & CAAG (Günlük Kilo Artışı) Motoru:**
   - Kantar/baskül tartımı veya mezurayla şerit metre ölçümü (Schaeffer formülü: $G^2 \times U / 108.38$).
   - İki tartım arası Günlük Canlı Ağırlık Artışı (CAAG kg/gün).
   - Canlı ağırlığa göre otomatik klinik ilaç dozajı ve kuru madde ihtiyacı.
   - %58 Karkas Randımanı Simülatörü ve mezbaha satış geliri hesabı.

6. **🥩 Et İKAS & Mezbaha / Kesim Kilitleri:**
   - Vurulan antibiyotik ve ilaçların et arınma sürelerini takip eder. Kesim kilidi bitene kadar dananın kesime veya kasaba gönderilmesini engeller.

7. **🌾 Yemlik Yönetimi, Tezek Skoru & Tampon Dozlama:**
   - Yatan danaların geviş getirme indeksi ($\ge \%58$ kuralı).
   - 1–5 Tezek kıvamı ve bütün tahıl tanesi kaçağı denetimi.
   - Bunk skoru (artık yem %3–5).
   - Dana başına günlük 150–250 gr tampon karbonat (sodyum bikarbonat) dozlayıcı.

8. **📅 Aşı & Parazit Takvimi:**
   - Şap, LSD Çiçek, Enterotoksemi (Çelerme / Yem Çarpması), BRD karma solunum aşısı ve İvermektin iç-dış parazit takvimi.

9. **💰 Besi Masraf & Fire Defteri:**
   - Veteriner ve ilaç harcamalarıyla birlikte, hastalık yüzünden yaşanan canlı ağırlık kaybı / duraklama firesini hesaplayıp toplam ekonomik zararı kuruşu kuruşuna gösterir.

10. **💾 Güvenli JSON Yedekleme & Geri Yükleme:**
    - Tüm çiftlik verilerini tek tıkla cihazınıza JSON olarak indirin veya yeni telefona aktarın. %100 yerel ve güvenli.
