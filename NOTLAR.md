# Mais Grup Yeni Web Sitesi: Analiz ve Yol Haritası

Taslak: `index.html` (tarayıcıda çift tıklayarak açılır). Logo: `assets/logo.png`

---

## 1. Mevcut sitede (maisgrup.com) bulunan sorunlar

### Güveni doğrudan zedeleyenler (öncelikli)
- **Sayaçlar "0+" gösteriyor.** Tamamlanan proje, aktif proje ve grup şirketi sayılarının hepsi 0. Ziyaretçi bunu "hiç proje yok" diye okur. En kritik hata bu.
- **Projelerimiz sayfası boş.** /projelerimiz/ adresinde tek bir proje listelenmiyor.
- **"Bizimle İletişieme geç" butonu** hem yazım hatalı hem de iletişim sayfası yerine bir Vimeo linkine gidiyor.
- **Ana sayfada aynı proje (Şamlar Özel Malikane) iki kez listelenmiş.**
- Projelerde **durum bilgisi yok** (devam ediyor / teslim edildi), konum, daire sayısı ve teslim tarihi de yazmıyor.
- Kurucular sayfası olmasına rağmen **isim ve yüz görünmüyor**. İnşaatta insanlar ev değil güven satın alır, güven de yüz ister.
- **E-posta adresi, WhatsApp ve sosyal medya linkleri yok.**
- Grup şirketlerinin logoları (Mebalife, Şanlıbayrak, Navy) **açıklamasız ve linksiz**.

### İçerik ve dil
- Vizyon ve Misyon bölümlerinde aynı paragraf tekrar ediyor.
- Breadcrumb'da "Home" yazıyor (Türkçe sitede İngilizce), footer'da "A.ş." yazıyor (doğrusu "A.Ş.").
- Başlıklarda büyük/küçük harf kullanımı tutarsız.
- Hizmetler (tasarım, konsept, iç mekân) genel ve sıradan. Mais'i rakiplerden ayıran bir şey anlatılmıyor.

### Teknik / SEO
- Hazır bir WordPress temasının ("ruizarch") üzerine Elementor ile kurulmuş. Ağır, yavaş ve kurumsal kimliğe özgü değil.
- **Meta description ve Open Graph etiketleri yok.** Google'da ve WhatsApp'ta paylaşıldığında düzgün bir önizleme çıkmıyor.
- 4 farklı font yükleniyor (Sora, Syne, Caveat, Satisfy). Bu hem yavaşlatıyor hem de görsel bütünlüğü bozuyor.
- Görsellerin alt metinleri "image", "icon" gibi değerler ya da hiç yok. Dosya adları "Group-20.png" gibi. Hem erişilebilirlik hem SEO zarar görüyor.
- Menüde tekrar var: "Hakkımızda > Hakkımızda", "Mais Blog > Mais Blog".
- Yabancı dil seçeneği yok.
- KVKK / çerez metni görünmüyor. **Bu yasal bir risk.**

---

## 2. Renk paleti ve psikolojisi

Logo **gri bina silüeti** ile **turuncu el yazısı** ("Yaşamın Ötesine") kombinasyonundan oluşuyor. Paleti bu ikisinden türettim, ancak turuncuyu göz yormayacak şekilde yumuşattım.

| Rol | Renk | Hex | Psikolojik etkisi |
|---|---|---|---|
| Ana / koyu | Derin arduvaz | `#1E2A32` | Lacivert ile antrasit arası bir ton. Mavi, en çok **güven ve istikrar** ile ilişkilendirilen renktir. Saf siyah kadar sert durmaz. Bankalar ve sigorta şirketleri bu yüzden mavi kullanır. |
| Zemin | Sıcak taş | `#F5F2EC` | Saf beyaz gibi parlamaz, göz yormaz. Taş ve beton gibi **doğal yapı malzemelerini** çağrıştırır. Hissi "ev" ve sıcaklıktır. |
| Vurgu (CTA) | Yumuşak bakır | `#B8743A` | Logodaki turuncunun olgun hali. Turuncu **harekete geçirir** (buton rengi), bakır tonu ise **premium ve kalıcılık** hissi verir. Yalnızca butonlarda ve önemli kelimelerde kullanılır. Az kullanıldığı için göz hemen onu bulur (von Restorff etkisi). |
| Marka gri | Grafit | `#6E7378` | Logonun kendi grisi. İkincil metinlerde kullanılır. |
| Güvenlik | Adaçayı yeşili | `#5F7A6B` | "Teslim edildi", "tamamlandı" ve sürdürülebilirlik bölümlerinde kullanılır. Yeşil beyinde **"güvenli, onaylandı"** sinyali verir. |

**Kural:** Ekranın yaklaşık %60'ı taş zemin, %30'u arduvaz, %10'u bakır olmalı (60-30-10 kuralı). Kırmızı ve parlak sarı **hiç kullanılmadı**, çünkü bu renkler alarm ve tehlike çağrıştırır. Deprem kaygısı olan bir alıcıya bu sinyal verilmemeli.

## 2.1 Yazı dili kuralı

Sitede **az ve net yazı** olacak. Başlık kısa, altında en fazla bir cümle. Uzun açıklamalar alt sayfalara ya da SSS'ye taşınır.

## 3. Fontlar

- **Manrope:** Başlık ve gövde metinlerinde. Geometrik ve modern bir font. Logodaki ince, yuvarlak harflere ("Yaşamın Ötesine…") çok yakın. Türkçe karakterleri (ş, ğ, ı, İ) eksiksiz destekliyor.
- **Fraunces Italic:** Yalnızca vurgu kelimelerinde ("sağlam temeller", "yaşam alanı"). Logonun beyaz versiyonundaki el yazısı sloganına bir gönderme. Premium ve "el işçiliği" hissi verir.
- Toplam 2 font var (mevcut sitede 4). Sitenin hızı ve görsel bütünlüğü bundan fayda görür.

---

## 4. Bölüm sıralaması ve mantığı

Ziyaretçinin kafasındaki sorular hangi sırayla geliyorsa bölümler de o sırayla dizildi:

1. **Hero:** "Bu kim, ne yapıyor?" sorusunun cevabı. Tek mesaj ve tek ana buton var. Sağdaki **canlı inşaat kartı** ilk saniyede "bu firma gerçekten iş yapıyor" kanıtını veriyor.
2. **Güven şeridi:** Deprem yönetmeliği, zamanında teslim, yapı denetimi. Türkiye'de ev alırken en büyük kaygı bu olduğu için en üste konuldu.
3. **Projeler:** İnsanlar siteye en çok projeleri görmek için gelir, bu yüzden Hakkımızda'dan **önce** geliyor. Filtre seçenekleri: Devam Eden / Tamamlanan / Yakında.
4. **Sık Sorulan Sorular:** Projeyi beğenen alıcının aklına hemen deprem, tapu, kredi ve teslim soruları gelir. Açılır-kapanır liste olduğu için kalabalık görünmez. Google'da soru-cevap olarak çıkması için FAQ şeması eklendi.
5. **Hakkımızda ve rakamlar:** Projeleri beğenen kişi "kim bunlar?" diye sorar.
6. **Güvenlik ve kalite (bento ızgara):** Zemin etüdü, temel ve beton testleri gibi "görünmeyen mühendislik" burada anlatılıyor.
7. **Canlı inşaat takibi:** Yenilikçi özellik (aşağıda detaylı).
8. **Satın alma süreci:** 4 adım. Belirsizliği azaltır.
9. **Grup şirketleri:** Kayan logo bandı. Mebalife logosu mebalife.com.tr'ye gidiyor.
10. **Kurucular:** Gerçek yüzler ve isimler.
11. **Blog:** SEO trafiğinin ana kaynağı.
12. **İletişim:** Form, harita, telefon. Ayrıca her sayfada sabit bir **WhatsApp butonu** var.

---

## 5. Yenilikçi özellikler (rakiplerin çoğunda olmayanlar)

### Taslakta çalışır halde olanlar
- **Canlı inşaat takibi:** Proje seçilince aşama zaman çizelgesi ve ilerleme yüzdesi görünüyor. Gerçek sitede her aşamaya **şantiye fotoğrafları ve drone videosu** eklenmeli. Daire satın almış müşteri buradan evini takip eder. Bu, güven ve sadakat açısından çok güçlü bir araç.
- **Proje filtreleme** ve her kartta ilerleme çubuğu.
- **Hero'da canlı proje kartı:** Yanıp sönen yeşil nokta ile "şu an inşa ediliyor" bilgisi gösteriliyor.
- **Sabit WhatsApp butonu**, KVKK onaylı form ve harita.

### Bir sonraki aşamada eklenebilecekler
1. **Etkileşimli daire seçici:** Bina görselinin üzerinde kata ve daireye tıklayınca kat planı, m², cephe ve satış durumu (müsait / satıldı) açılır. Büyük markaların (Nef, Sinpaş) kullandığı ama küçük firmalarda neredeyse hiç görülmeyen bir özellik.
2. **360° sanal tur / örnek daire:** Matterport veya benzeri bir araçla yapılabilir.
3. **Müşteri paneli:** Daire sahipleri giriş yapıp ödeme takvimini, belgelerini ve inşaat fotoğraflarını görür.
4. **"Güvenlik dosyası" indirme:** Her projenin zemin etüdü, beton test sonuçları ve yapı denetim raporlarının özeti PDF olarak paylaşılır. Deprem sonrası dönemde bu şeffaflık **büyük bir rekabet avantajı**.
5. **Proje haritası:** Tüm projeler İstanbul haritası üzerinde gösterilir, yakındaki okul, metro ve hastane bilgileriyle birlikte.
6. **Çoklu dil (EN / AR / RU):** Yabancı yatırımcılar ve vatandaşlık yoluyla yatırım yapanlar için.
7. **Önce / sonra kaydırıcısı:** Arsa hali ile bitmiş proje karşılaştırması.
8. **Video arka planlı hero:** Drone çekimi.
9. **Gerçek müşteri yorumları (video):** Uydurma yorum kesinlikle kullanılmamalı. Gerçek teslim almış ailelerden kısa videolar çekilmeli.
10. **Randevu sistemi:** Ofis veya şantiye ziyareti için takvimden saat seçilebilir.

---

## 6. 21st.dev tarzı bileşenler (taslakta kullanılanlar)

Taslakta 21st.dev'de popüler olan modern bileşen kalıplarını sade HTML/CSS ile uyguladım. Gerçek projede React/Next.js'e geçildiğinde 21st.dev'den doğrudan alınabilecekler:

| Taslaktaki bölüm | 21st.dev'de aranacak bileşen / prompt |
|---|---|
| Yüzen, buzlu cam navbar | "floating glass navbar", "navbar with scroll blur" |
| Hero + canlı kart | "hero section with image background and floating stat card" |
| Güvenlik bölümü | "bento grid", "features bento" |
| Logo bandı | "logo marquee", "logo cloud infinite scroll" |
| Rakamlar | "animated number counter", "stats section" |
| İnşaat takibi | "timeline", "vertical stepper", "progress ring" |
| Proje kartları | "project card with hover zoom", "filterable gallery" |
| Satın alma süreci | "feature steps", "process section" |
| İletişim | "contact section with form and map" |

Örnek prompt (21st.dev Magic veya başka bir AI için):
> "Premium real estate hero section, full-bleed architectural photo with dark slate gradient overlay, large headline with one italic serif accent word in muted copper (#B8743A), two CTAs (filled copper + ghost), and a glassmorphism card on the right showing live construction progress with a pulsing green dot and animated progress bar. Font: Manrope + Fraunces italic. Calm, trustworthy, no bright colors."

---

## 7. Teknik öneriler (sıfırdan yaparken)

- **Altyapı:** Next.js + Tailwind CSS ile headless bir CMS (Sanity veya Strapi). Projeler, blog ve inşaat aşamaları panelden kod yazmadan güncellenebilir. Alternatif olarak WordPress kalmak istenirse hazır tema ve Elementor kullanılmamalı, özel bir tema yazılmalı.
- **Hız:** Görseller WebP/AVIF formatında olmalı, lazy-load kullanılmalı. Hedef: Lighthouse skoru 90+.
- **SEO:**
  - Her projeye ayrı sayfa açılmalı (`/projeler/yenimahalle-toplu-konut`).
  - Schema.org işaretlemesi eklenmeli (`RealEstateListing`, `Organization`, `LocalBusiness`).
  - Google Business profili siteye bağlanmalı.
  - Blogda "Başakşehir'de satılık villa" gibi yerel anahtar kelimeler hedeflenmeli.
- **Yasal:** KVKK aydınlatma metni, çerez bandı ve formlarda onay kutusu.
- **Ölçüm:** GA4 ve Meta Pixel kurulmalı, form ve WhatsApp tıklamaları dönüşüm olarak takip edilmeli.
- **Erişilebilirlik:** Renk kontrastı WCAG AA seviyesinde, anlamlı alt metinler, klavye ile gezinme.

---

## 8. ⚠️ Taslakta ÖRNEK olan, doğrulanması gereken veriler

Aşağıdakileri ben uydurdum ya da tahmin ettim. Gerçek bilgilerle değiştirilmeli:
- Proje durumları, ilerleme yüzdeleri, daire sayıları ve teslim tarihleri
- "35+ proje", "1200+ mutlu aile" rakamları (17 yıl bilgisi mevcut siteden alındı)
- "2009'dan beri" ifadesi (17 yıldan hesaplandı)
- Şamlar ve Yarımburgaz projelerinin ilçe bilgisi (Başakşehir olarak tahmin edildi)
- Güvenlik bölümündeki teknik detaylar (C35 beton, radye temel vb.)
- E-posta adresi (info@maisgrup.com) ve WhatsApp numarası
- Kurucu isimleri ve fotoğrafları
- Blog başlıkları
- Hakkımızda bölümündeki gökdelen fotoğrafı Unsplash'ten alınmış bir stok görsel (ücretsiz lisanslı). Mais'in kendi projesi değil, ileride kendi çekimimizle değiştirilmeli.
- SSS cevapları genel bilgi niteliğinde. Kredi anlaşmaları, garanti kapsamı ve yabancıya satış bilgileri firmaya göre teyit edilmeli.
- **Grup şirketleri bağlantıları:** Mebalife → mebalife.com.tr bağlandı. Şanlıbayrak ve Naavy için resmi bir site bulamadım. sanlibayrak.com.tr adresi var, ama orası Beylikdüzü'nde başka bir çelik konstrüksiyon firması ve logosu farklı, bu yüzden bağlamadım. naavy.com ise bilinmeyen bir yere yönlendiriyor. Adresleri varsa bildirin, eklenir.
- Görseller şu an mevcut siteden çekiliyor. Yeni sitede **profesyonel çekim ve drone görüntüleri** şart.

## 9. Sizden ihtiyacım olanlar
1. Logonun vektör hali (SVG / AI)
2. Gerçek proje listesi ve her projenin bilgileri
3. Kurucuların bilgileri ve fotoğrafları
4. Grup şirketlerinin ne iş yaptığı
5. Sosyal medya hesapları ve e-posta adresi
6. Altyapı tercihi: Next.js mi, WordPress mi?
