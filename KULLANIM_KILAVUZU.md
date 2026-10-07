# 🐄 Sığır Sağlık Rehberi - Kullanım Kılavuzu

**Sığır Sağlık Rehberi**, internet bağlantısı ve sunucu kurulumu gerektirmeyen, doğrudan telefon ve bilgisayar tarayıcısında çalışan çevrimdışı (%100 offline) bir büyükbaş sürü sağlığı ve yönetim asistanıdır.

---

## 🚀 1. Hızlı Başlangıç & Kurulum

### Telefonunuza Yükleme (Android / iOS):
1. İnternetiniz varken [https://mserman90.github.io/sigir-saglik-rehberi/](https://mserman90.github.io/sigir-saglik-rehberi/) adresini açın.
2. Tarayıcı menüsünden (üç nokta veya paylaş butonu) **"Ana Ekrana Ekle"** veya **"Uygulamayı Yükle"** seçeneğine dokunun.
3. Telefonunuzun ana ekranına uygulama ikonu eklenir. Artık dağda, merada, internetin hiç çekmediği bodrum ahırlarda dahi tam ekran çalışır.

### Bilgisayarda Açma:
- Doğrudan web adresini açabilir veya depodaki `index.html` dosyasına çift tıklayarak tarayıcınızda çalıştırabilirsiniz.

---

## 📱 2. Temel Modüllerin Kullanımı

### 0. 📷 Kamerayla Küpe Okuma (Barkod / QR)
- Hayvan arama, muayene, ilaç yapma, tohumlama ve sağım ekranlarında yer alan sarı **"📷 Oku"** butonuna basın.
- Kamerayı hayvanın sarı kulak küpesindeki barkod veya karekoda doğrultun.
- Küpe numarası otomatik doldurulur, telefon hafifçe titrer ve ilgili hayvanın sağlık kaydı ekrana gelir.

---

### 1. 📊 Ahır Durumu & Hayvan Kaydı
- **Yeni Hayvan Ekleme:** Ekrandaki **"+ Yeni Ekle"** butonuna basarak küpe numarası, cinsiyeti, yaşı ve kondisyon durumunu girin.
- **Pazardan Yeni Alınanlar:** *"Pazardan yeni alındı, ayrı bölmede bekleyecek (Karantina)"* kutucuğunu işaretlerseniz sürüye hastalık bulaşmaması için sistem hayvanı sarı alarm durumuna alır.
- **Hayvan Silme:** Listeden satırın sonundaki *"Sil"* butonuna basarak kaydı silebilirsiniz.

---

### 2. 🩺 Hasta Muayene Et (Saha Triyajı)
Bir ineğin hastalandığından şüphelendiğinizde bu ekrana girin:
1. **Makat Ateşi (°C):** Dereceyle ölçtüğünüz ateşi yazın (Normal: 38.0–39.3 °C. 39.5 °C ve üzeri kırmızı alarmdır).
2. **Nabız & Nefes:** 1 dakikadaki kalp atımı ve nefes sayısını girin.
3. **İşkembe Çalışması:** Sol açlık çukurunu dinleyip dalga sayısını seçin.
4. **Hastalık Puanlama (DART):** Keyifsizlik, iştah durumu ve hırıltılı nefes seçeneklerini 0'dan 3'e kadar işaretleyin.
5. Sistem anında **"DURUMU İYİ"**, **"ORTA DERECE HASTA (İlaç Lazım)"** veya **"ÇOK ACİL & AĞIR HASTA (Veterineri Çağır)"** kararı verir ve ne yapmanız gerektiğini maddeler halinde sıralar.

---

### 3. 💊 İlaç Kaydı & Sütü/Eti Tanka Yasaklama (İKAS)
Antibiyotik veya iğne yaptığınızda sütün tanka karışıp tüm tankı heba etmesini önler:
1. İlaç yapılan hayvanı ve uygulanan ilacı listeden seçin.
2. Vurulan dozu ve saati onaylayıp kaydedin.
3. Sistem yasal arınma süresine göre (Merck Vet standartları) **saat ve dakika bazında geri sayım** başlatır.
4. **Kombine Kuralı:** Hayvana aynı gün 2 farklı ilaç yapıldıysa sistem otomatik olarak süresi en uzun olan ilacın gününü kilitler.

---

### 4. 💰 Hastalık Masrafı & Dökülen Süt Zarar Defteri
Hastalıkların çiftliğinize maliyetini kuruşu kuruşuna gösterir:
1. Üst kısımdan çiğ süt satış fiyatınızı (Örn: 16.5 TL/Litre) yazın.
2. Tedavi gören hayvanı, hastalığını, veterinere ve ilaca ödenen parayı girin.
3. İlaç yüzünden lavaboya dökülen günlük süt miktarını ve kaç gün döküldüğünü yazın.
4. Sistem hem dökülen sütün parasal zararını hem de toplam tedavi maliyetini hesaplayıp deftere kaydeder.

---

### 5. 🌾 Yemlik Düzeni, İşkembe Ekşimesi & Geviş Sayacı
1. **Geviş Getirme Sayacı:** Yem döküldükten 2 saat sonra ahırdaki yerde yatan inekleri ve geviş getirenleri sayıp yazın. Hedef en az %58-60'tır. Altında kalırsa işkembe ekşimesi (asidoz) uyarısı verir.
2. **Tezek Kıvamı (1-5):** Tezeğin cıvıklığına bakarak rasyondaki saman veya fabrika yemi dengesini test edin.
3. **Karbonat Dozu:** Sağılan inek sayısını girerek yem karma makinesine kaç kilo karbonat (sodyum bikarbonat) katmanız gerektiğini otomatik hesaplayın.

---

### 6. 🩸 Tohumlama, Gebelik & Doğum Çarkı
1. Tohumlanan ineği, tohumlama tarihini ve boğa kodunu yazıp kaydedin.
2. Otomatik zaman çizelgesi hesaplanır:
   - **21. Gün:** Kızgınlık dönüş kontrolü (Tutmadıysa tekrar boğaya gelir).
   - **40. Gün:** Ultrason / rektal gebelik muayenesi günü.
   - **220. Gün:** Kuruya alma ve kuru dönem tüpü günü (Doğuma 60 gün kala).
   - **280. Gün:** Beklenen doğum günü.

---

### 7. ⚖️ Şerit Metreyle Canlı Ağırlık Ölçer (Kantar Yokken!)
Ahırda veya yaylada baskül yokken terzi mezurası veya şerit metreyle kilo hesaplar:
1. **Göğüs Çevresi (cm):** Ön ayakların hemen arkasından mezurayla sarın.
2. **Vücut Uzunluğu (cm):** Omuz başı ile kalça çıkıntısı arasını ölçün.
3. Bilimsel *Schaeffer Formülü* ile canlı ağırlık hesaplanır ve hayvana vurulacak adrenalin, meloksikam, fluniksin dozları ile günlük saman/kuru madde ihtiyacı ekrana gelir.

---

### 8. 🍼 Buzağı Hayatta Tutma & İlk Ağız Sütü (Kolostrum)
1. **Altın Kural:** Doğumdan sonraki **ilk 2 saat içinde** ananın koyu ağız sütünden en az 3–4 litre mutlaka içirilmelidir!
2. **Brix Kalite Ölçer:** Işıklı optik camla (refraktometre) ölçülen yüzdeyi girin. %22 ve üstü mükemmel kalitedir.
3. **Buzağı İshali Serum Hesabı:** Buzağının kilosunu ve göz çökme derecesini seçin. 24 saatte kaç litre ağızdan veya damardan serum verilmesi gerektiği anında hesaplanır.

---

### 9. 🆘 Acil İlk Yardım
Veteriner hekim ahıra ulaşana kadar hayat kurtaracak ilk adımlar:
- **İğne / Aşı Şoku (Anafilaksi):** Kilo bazında otomatik adrenalin dozu ve müdahale.
- **İşkembe Şişmesi (Timpani):** Sıvı yağ içirme ve trokar şişleme tekniği.
- **Rahim Düşmesi:** Döl yatağını ıslak bezle havaya kaldırma kuralı.
- **Doğum Felci (Süt Humması):** Kalsiyum serumu uygulama uyarısı.

---

### 10. 🥛 Sağımcı Ekranı (Büyük Harfli Hızlı Kontrol)
Sağımhanede çalışan personelin tek bakışta görmesi için hazırlanmıştır:
- Küpe numarasını yazın veya kamerayla okutun.
- Eğer hayvana antibiyotik vurulmuşsa ekran **kocaman kırmızı alarm** verir ve kaç saat kaldığını gösterir.
- İlaçsız ineklerde **"🟢 SAĞIMA UYGUN"** yeşil onayı çıkar.

---

## 💾 3. Veri Yedekleme & Telefona Aktarma
- Sağımcı ekranının en altında yer alan **"📥 Yedeği İndir (JSON)"** butonuna basarak tüm hayvan ve aşı kayıtlarınızı tek bir yedek dosyası olarak indirebilirsiniz.
- Başka bir telefona geçtiğinizde **"📤 Yedeği Yükle"** diyerek saniyeler içinde tüm çiftlik verilerinizi geri yükleyebilirsiniz.
