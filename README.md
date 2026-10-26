# Web Sitesi Erişilebilirlik Rehberi (WCAG 2.2)

Görme, işitme, hareket ya da algı güçlüğü olan kişilerin bir web sitesini ve mobil uygulamayı kullanabilmesi için yapılması gerekenleri anlatan Türkçe rehber. Site sahibi, e-ticaret satıcısı, haber sitesi editörü, tasarımcı ve yeni başlayan geliştirici için yazıldı.

Rehberde kod yok. Her başlık "ne", "neden" ve "nasıl kontrol ederim" sorularına cevap verir.

> Bu rehber eğitim amaçlıdır, hukuki görüş değildir. Yükümlülüğünüzü yürürlükteki metinden ve ilgili kurumdan teyit edin.

Son güncelleme: 2026-10-26

---

## İçindekiler

1. Erişilebilirlik kimin işine yarar?
2. Türkiye'de durum: 2025/10 sayılı Genelge
3. WCAG 2.2'yi beş dakikada anlamak
4. Görseller ve alternatif metin
5. Renk ve kontrast
6. Klavye ile kullanım ve odak
7. Başlıklar, sayfa yapısı ve bağlantılar
8. Formlar ve hata mesajları
9. Giriş ekranı, doğrulama kodu ve CAPTCHA
10. Video, ses ve canlı yayın
11. Dokunmatik ekran ve mobil uygulama
12. E-ticaret sitesine özel noktalar
13. Haber sitesine özel noktalar
14. Nasıl test edilir?
15. Erişilebilirlik beyanı
16. Sık yapılan 12 hata
17. Kontrol listesi (20 madde)
18. Resmî kaynaklar

---

## 1. Erişilebilirlik kimin işine yarar?

Erişilebilirlik yalnız ekran okuyucu kullanan görme engelli kişiler için değildir. Şu kişiler de aynı düzenlemelerden yararlanır:

- Elinde kırık olan ve fareyi kullanamayan biri,
- Güneş altında telefonuna bakan ve soluk gri yazıyı okuyamayan biri,
- Kalabalık bir otobüste sesi kapalı video izleyen biri,
- Yaşı ilerlemiş, küçük düğmelere basmakta zorlanan biri,
- Türkçeyi yeni öğrenen ve sade metne ihtiyaç duyan biri.

Bir siteyi erişilebilir yapmak çoğu zaman siteyi herkes için daha düzenli ve daha hızlı kullanılır hâle getirir. Arama motorları da düzgün başlık yapısı, anlamlı bağlantı metni ve görsel açıklaması gibi aynı sinyallerden yararlanır.

## 2. Türkiye'de durum: 2025/10 sayılı Genelge

Web Siteleri ve Mobil Uygulamaların Erişilebilirliği ile ilgili **2025/10 sayılı Cumhurbaşkanlığı Genelgesi**, 21 Haziran 2025 tarihli Resmî Gazete'de yayımlandı. Genelgedeki ana noktalar:

- Ölçüt: **"Web Siteleri ve Mobil Uygulamaların Erişilebilirliği Kontrol Listesi – A Seviyesi"** ile **Web İçeriği Erişilebilirlik Kılavuzu (WCAG 2.2)**. Her ikisi Aile ve Sosyal Hizmetler Bakanlığı'nın sitesinde yayımlanır.
- Kamu kurum ve kuruluşları, üniversiteler, belediyeler ve şirketleri, kamu kurumu niteliğindeki meslek kuruluşları, bankalar, özel hastaneler, özel öğretim kurumları, belirli ulaşım ve turizm işletmeleri ile 200.000'in üzerinde abonesi olan elektronik haberleşme işletmecileri için süre **1 yıl**.
- 6563 sayılı Kanun kapsamında **elektronik ticaret yapan hizmet sağlayıcılar** için süre **2 yıl**.
- İzleme sonucunda erişilebilir bulunan kurumlar **2 yıl** süreyle "Erişilebilirlik Logosu" kullanabilir.

Genelge 20 Haziran 2025 tarihlidir; sürelerin nasıl hesaplanacağı ve uygulama ayrıntıları için Bakanlığın duyurularını takip edin.

Yurt dışına, özellikle Avrupa Birliği'ndeki tüketicilere satış yapıyorsanız **Avrupa Erişilebilirlik Yasası** (Direktif 2019/882) 28 Haziran 2025'ten beri uygulanıyor; e-ticaret hizmetleri de kapsamda. Hangi işletmelerin muaf olduğu ülke düzenlemesine göre değişir.

## 3. WCAG 2.2'yi beş dakikada anlamak

WCAG, W3C'nin yayımladığı uluslararası erişilebilirlik ölçütüdür. Güncel sürüm 2.2'dir. Ölçütler dört ilke altında toplanır:

| İlke | Soru | Örnek |
|---|---|---|
| Algılanabilir | Kullanıcı içeriği görebiliyor ya da duyabiliyor mu? | Görsel açıklaması, altyazı, yeterli kontrast |
| Çalıştırılabilir | Kullanıcı her şeyi kullanabiliyor mu? | Klavye ile gezinme, yeterli süre, büyük dokunma alanı |
| Anlaşılabilir | Kullanıcı ne olduğunu anlıyor mu? | Açık hata mesajı, tutarlı menü, sayfa dili |
| Sağlam | Yardımcı teknolojiler sayfayı doğru okuyabiliyor mu? | Düğmenin gerçekten düğme olarak tanımlanması |

Her ölçütün bir seviyesi vardır: **A** (en temel), **AA** (çoğu kurumun hedeflediği seviye), **AAA** (en ileri). Türkiye'deki kontrol listesi A seviyesini esas alır; AA seviyesini hedeflemek iyi bir pratiktir.

2.2 sürümüyle gelen yeni ölçütler:

| No | Ölçüt | Seviye |
|---|---|---|
| 2.4.11 | Odak gizlenmemeli (asgari) | AA |
| 2.4.12 | Odak gizlenmemeli (ileri) | AAA |
| 2.4.13 | Odak görünümü | AAA |
| 2.5.7 | Sürükleme hareketine alternatif | AA |
| 2.5.8 | Dokunma alanı boyutu (asgari) | AA |
| 3.2.6 | Yardım bağlantısı her sayfada aynı yerde | A |
| 3.3.7 | Aynı bilgiyi tekrar istememe | A |
| 3.3.8 | Erişilebilir kimlik doğrulama (asgari) | AA |
| 3.3.9 | Erişilebilir kimlik doğrulama (ileri) | AAA |

Eski "4.1.1 Ayrıştırma" ölçütü 2.2'de kaldırıldı.

## 4. Görseller ve alternatif metin

Ekran okuyucu bir görseli göremez; görselin alternatif metnini (alt metin) okur.

- **Bilgi taşıyan görsel:** Görselin söylediğini yazın. "Ürün fotoğrafı" yerine "Lacivert, uzun kollu, düğmeli pamuk gömlek".
- **Süs görseli:** Alt metni boş bırakın. Böylece ekran okuyucu onu atlar. Alt metin hiç yazılmazsa birçok ekran okuyucu dosya adını okur ("IMG_4471 nokta jpg").
- **Bağlantı ya da düğme olan görsel:** Görseli değil, gideceği yeri anlatın. Sepet simgesi için "Sepet (3 ürün)".
- **Yazı içeren görsel:** Kampanya afişindeki yazının tamamı alt metinde ya da sayfada metin olarak bulunmalı.
- **Grafik ve tablo görseli:** Kısa alt metin + yanında ya da altında verinin metin özeti.

Haber sitelerinde fotoğrafın altındaki "Fotoğraf: AA" gibi kaynak bilgisi alt metin değildir; alt metin fotoğrafta ne olduğunu anlatır.

## 5. Renk ve kontrast

- Normal metinde yazı ile zemin arasındaki kontrast oranı en az **4.5:1**, büyük metinde en az **3:1** olmalı (WCAG 1.4.3, AA).
- Düğme kenarı, form kutusu çerçevesi, simge gibi metin dışı ögelerde oran en az **3:1** (WCAG 1.4.11, AA).
- **Bilgi yalnız renkle verilmemeli.** "Kırmızı alanlar zorunludur" yerine alanın yanına "zorunlu" yazın. Stokta yok bilgisini yalnız gri renkle değil, metinle de gösterin.
- Açık gri zemin üzerine açık gri yazı, fotoğraf üzerine beyaz yazı ve logonun renginden seçilmiş soluk vurgu rengi en sık rastlanan kontrast sorunlarıdır.

Tarayıcıların geliştirici araçlarında ve ücretsiz kontrast hesaplayıcılarda iki rengin oranı birkaç saniyede ölçülür.

## 6. Klavye ile kullanım ve odak

Fare kullanamayan kişi siteyi Tab, Shift+Tab, Enter, boşluk ve ok tuşlarıyla kullanır.

- Bağlantı, düğme, menü, form alanı, açılır pencere: hepsine klavyeyle ulaşılabilmeli.
- **Odak görünmeli.** Hangi ögenin seçili olduğu belirgin bir çerçeveyle gösterilmeli. Tasarım temizliği için odak çerçevesini kaldırmak en yaygın hatadır.
- **Odak gizlenmemeli** (2.4.11). Sayfanın altına yapışan çerez bandı ya da üstte sabit duran menü, odaktaki ögenin üzerini kapatmamalı.
- **Sıra mantıklı olmalı.** Tab ile ilerlerken odak sayfada zıplamamalı.
- **Açılır pencereye odak taşınmalı**, pencere kapanınca odak açan düğmeye geri dönmeli. Esc tuşu pencereyi kapatmalı.
- **Klavye tuzağı olmamalı.** Bir harita, video oynatıcı ya da gömülü içerikte odak sıkışıp kalmamalı.
- Sayfanın başına "İçeriğe geç" bağlantısı koymak, her sayfada uzun menüyü tekrar dolaşmayı önler.

## 7. Başlıklar, sayfa yapısı ve bağlantılar

- Her sayfada bir **ana başlık** olmalı; alt bölümler sıralı başlıklarla (2. düzey, 3. düzey) ayrılmalı. Ekran okuyucu kullanıcıları sayfada başlıktan başlığa atlayarak gezinir.
- Başlık, yazıyı büyütmek için değil, bölümü adlandırmak için kullanılmalı.
- **Sayfa dili** tanımlı olmalı. Türkçe bir sayfa İngilizce olarak tanımlanırsa ekran okuyucu metni İngilizce telaffuzla okur.
- **Sayfa başlığı** (tarayıcı sekmesinde görünen) her sayfada farklı ve açıklayıcı olmalı.
- **Bağlantı metni** gideceği yeri anlatmalı. Bir sayfada on tane "buraya tıklayın" ya da "devamı" bağlantısı, ekran okuyucunun bağlantı listesinde anlamsız bir tekrar olur.
- Yeni sekmede açılan bağlantı ve PDF gibi dosya bağlantıları bunu metinde belirtmeli ("Fiyat listesi, PDF, 2 MB").
- **Yardım bağlantısı tutarlı olmalı** (3.2.6). İletişim, canlı destek ya da SSS bağlantısı her sayfada aynı yerde durmalı.

## 8. Formlar ve hata mesajları

Formlar, erişilebilirlik sorunlarının en çok biriktiği yerdir.

- Her alanın görünür ve alana bağlı bir **etiketi** olmalı. Kutunun içindeki silik örnek metin (yer tutucu) etiket yerine geçmez; yazmaya başlayınca kaybolur.
- **Zorunlu alan** metinle belirtilmeli, yalnız yıldız ya da renk yetmez.
- **Hata mesajı** hangi alanda, ne yanlış olduğunu ve nasıl düzeltileceğini söylemeli: "Telefon numarası 10 haneli olmalı, başında 0 olmadan yazın."
- Hata olduğunda form boşaltılmamalı; kullanıcının yazdıkları korunmalı.
- **Aynı bilgi tekrar istenmemeli** (3.3.7). Teslimat adresini yazan kullanıcıya fatura adresi için "teslimat adresiyle aynı" seçeneği sunulmalı.
- Süre sınırı olan işlemde (ödeme sayfası, oturum) kullanıcı uyarılmalı ve süreyi uzatabilmeli.
- Ödeme ve sözleşme onayı gibi geri alınamayan adımlardan önce bir özet ekranı gösterilmeli.

## 9. Giriş ekranı, doğrulama kodu ve CAPTCHA

WCAG 2.2'deki 3.3.8 ölçütü, giriş yaparken kullanıcıdan **hafıza ya da bulmaca testi** istenmemesini ister; bunun yerine bir alternatif sunulmalıdır.

- Parola alanına **yapıştırmayı engellemeyin.** Parola yöneticisi kullanan ya da parolayı not eden kişi giriş yapamaz hâle gelir.
- SMS ya da e-posta ile gelen kodu kopyalayıp yapıştırmak mümkün olmalı.
- Resimli bulmaca türü doğrulama kullanıyorsanız sesli alternatif ya da bulmacasız bir yöntem sunun.
- "Beni hatırla" seçeneği ve parola sıfırlama bağlantısı görünür yerde olmalı.

## 10. Video, ses ve canlı yayın

- Kayıtlı videoda **altyazı** olmalı. Otomatik altyazı başlangıç olarak işe yarar ama özel isim, rakam ve yer adlarında sık hata yapar; yayından önce kontrol edin.
- Yalnız sesten oluşan içerikte (podcast, sesli haber) **metin dökümü** verin.
- Videoda görüntüyle verilen önemli bilgi (ekrandaki yazı, grafik) seslendirme ya da açıklama metniyle de verilmeli.
- **Otomatik oynayan ses** 3 saniyeden uzunsa durdurma ya da sesi kapatma düğmesi olmalı.
- Saniyede üçten fazla yanıp sönen içerik ışığa duyarlı epilepsi riski taşır; kullanmayın.
- Kayan haber bandı, otomatik dönen slayt gibi hareketli içerik durdurulabilmeli.

## 11. Dokunmatik ekran ve mobil uygulama

- **Dokunma alanı** en az **24×24 CSS pikseli** olmalı ya da çevresinde yeterli boşluk bulunmalı (2.5.8, AA). Mobilde yan yana dizilmiş küçük paylaşım simgeleri en sık hatadır.
- **Sürükleme hareketine alternatif** sunulmalı (2.5.7). Fiyat aralığı kaydırıcısının yanında elle yazılabilen kutu, sıralama listesinde "yukarı/aşağı taşı" düğmesi gibi.
- Ekran yatay ve dikey yönde kullanılabilmeli; uygulama tek yöne kilitlenmemeli (zorunlu durumlar hariç).
- Yazı büyütüldüğünde (telefonun yazı boyutu ayarı ya da tarayıcıda %200 yakınlaştırma) içerik kesilmemeli, üst üste binmemeli.
- Mobil uygulamada düğmelerin ekran okuyucu için adı olmalı. Yalnız simgeden oluşan düğme adsızsa ekran okuyucu "düğme" der, ne yaptığını söylemez.

## 12. E-ticaret sitesine özel noktalar

- Ürün görsellerinde renk, desen, malzeme gibi satın alma kararını etkileyen bilgi alt metinde ya da açıklamada bulunmalı.
- Beden ve renk seçimi yalnız renkli kutucuklarla yapılıyorsa her kutucuğun adı olmalı ("Kırmızı", "M beden").
- Süzgeç ve sıralama klavyeyle kullanılabilmeli; süzgeç uygulandığında kaç ürün listelendiği bildirilmeli.
- Sepete ekleme sonrasında çıkan bildirim kısa sürede kaybolmamalı ya da ekran okuyucuya duyurulmalı.
- Ödeme adımları numaralı ve adlandırılmış olmalı ("3/4: Teslimat bilgileri").
- Kampanya ve indirim bilgisi yalnız görselde değil, metinde de yer almalı.
- Ön bilgilendirme formu ve mesafeli satış sözleşmesi okunabilir metin olarak sunulmalı; taranmış görüntü PDF ekran okuyucuyla okunamaz.

## 13. Haber sitesine özel noktalar

- Manşet ve slayt alanı durdurulabilmeli; okur haberin başlığını okumadan slayt değişmemeli.
- Haber fotoğrafında alt metin fotoğrafı anlatmalı; fotoğraf galerisinde her fotoğrafın kendi açıklaması olmalı.
- Haberin içine yerleştirilen reklamlar okuma akışını bölüyorsa ekran okuyucu için "reklam" olarak işaretlenmeli ve klavye odağını yakalamamalı.
- Video haberde altyazı ya da metin özeti bulunmalı.
- Yayın ve güncelleme tarihi metin olarak yazılmalı ("26 Ekim 2026, 11.40"); yalnız "3 saat önce" gibi göreli ifade ekran okuyucuda ve arşivde yanıltıcıdır.
- Son dakika bandı ve açılır bildirimler okurun odağını çalmamalı.

## 14. Nasıl test edilir?

Otomatik araçlar sorunların yalnız bir kısmını bulur. Kontrast, eksik alt metin, etiketsiz form alanı gibi hataları yakalarlar; alt metnin doğru olup olmadığını ya da klavye sırasının mantıklı olup olmadığını anlayamazlar. Önerilen sıra:

1. **Otomatik tarama:** Tarayıcının geliştirici araçlarındaki erişilebilirlik denetimi ya da ücretsiz bir tarama eklentisi.
2. **Klavye testi:** Fareyi kenara koyun, ana sayfadan başlayıp bir ürünü satın almaya ya da bir formu göndermeye kadar yalnız klavyeyle ilerleyin.
3. **Yakınlaştırma testi:** Tarayıcıda %200 yakınlaştırın; içerik kesiliyor mu, yatay kaydırma çıkıyor mu?
4. **Ekran okuyucu testi:** Windows'ta ücretsiz NVDA ya da Ekran Okuyucusu, telefonda TalkBack (Android) ve VoiceOver (iOS) ile birkaç temel işlemi deneyin.
5. **Gerçek kullanıcı:** Mümkünse yardımcı teknoloji kullanan birinden geri bildirim alın. En değerli test budur.

Testi bir kez yapıp bırakmayın. Yeni tema, yeni form ya da yeni kampanya sayfası eklendiğinde aynı adımları tekrarlayın.

## 15. Erişilebilirlik beyanı

Sitenizin altına bir "Erişilebilirlik" sayfası koymak iyi bir uygulamadır. İçinde şunlar bulunabilir:

- Hedeflenen standart ve seviye (örneğin WCAG 2.2 AA),
- Bilinen eksikler ve ne zaman giderileceği,
- Son değerlendirme tarihi,
- Erişilebilirlik sorunu bildirmek için bir iletişim yolu (e-posta ya da form) ve yanıt süresi,
- Alternatif erişim yolu (telefonla sipariş gibi).

Gerçek durumu yansıtmayan "sitemiz tamamen erişilebilirdir" beyanı, hiç beyan olmamasından daha kötüdür.

## 16. Sık yapılan 12 hata

| Hata | Sonuç | Çözüm |
|---|---|---|
| Odak çerçevesi kaldırılmış | Klavye kullanan nerede olduğunu bilemez | Belirgin, yüksek kontrastlı odak göstergesi |
| Alt metin yok ya da "resim" yazıyor | Görsel bilgisi kaybolur | Görselin söylediğini yazın, süs görselinde boş bırakın |
| Yer tutucu metin etiket yerine kullanılmış | Yazmaya başlayınca alanın ne olduğu unutulur | Görünür etiket |
| Soluk gri yazı | Güneşte ve az görenlerde okunmaz | 4.5:1 kontrast |
| Yalnız renkle verilen bilgi | Renk ayırt edemeyen anlamaz | Metin ya da simge ekleyin |
| "Buraya tıklayın" bağlantıları | Bağlantı listesi anlamsız olur | Gideceği yeri anlatan metin |
| Çerez bandı odağı kapatıyor | Klavye kullanıcısı ne seçtiğini göremez | Bandı içerikle çakıştırmayın |
| Açılır pencere klavyeyle kapanmıyor | Kullanıcı sayfada mahsur kalır | Esc ile kapanma, odağı geri verme |
| Parola alanına yapıştırma kapalı | Parola yöneticisi kullananlar giriş yapamaz | Yapıştırmaya izin verin |
| Küçük, sık dizilmiş dokunma alanları | Yanlış düğmeye basılır | En az 24×24 piksel ya da boşluk |
| Otomatik dönen slayt durdurulamıyor | Okumaya yetişilemez | Durdur düğmesi |
| Taranmış görüntü PDF | Ekran okuyucu tek kelime okuyamaz | Metin tabanlı belge |

## 17. Kontrol listesi (20 madde)

- [ ] Her sayfada açıklayıcı bir sekme başlığı ve tek ana başlık var.
- [ ] Sayfa dili doğru tanımlı.
- [ ] Başlık düzeyleri sıralı, bölümleri adlandırıyor.
- [ ] Bilgi taşıyan her görselin alt metni var, süs görsellerinde boş.
- [ ] Normal metin kontrastı en az 4.5:1, büyük metin en az 3:1.
- [ ] Bilgi yalnız renkle verilmiyor.
- [ ] Sitenin tamamı klavyeyle kullanılabiliyor.
- [ ] Odak her zaman görünür ve sabit bantların altında kalmıyor.
- [ ] "İçeriğe geç" bağlantısı var.
- [ ] Açılır pencereler Esc ile kapanıyor, odak geri dönüyor.
- [ ] Her form alanının görünür etiketi var, zorunlu alan metinle belirtiliyor.
- [ ] Hata mesajları alanı ve çözümü söylüyor, girilen veri korunuyor.
- [ ] Aynı bilgi aynı işlemde iki kez istenmiyor.
- [ ] Parola ve doğrulama kodu alanlarına yapıştırma serbest.
- [ ] Bulmaca tipi doğrulamanın alternatifi var.
- [ ] Videolarda kontrol edilmiş altyazı, ses içeriğinde metin dökümü var.
- [ ] Otomatik oynayan ses ve hareketli içerik durdurulabiliyor.
- [ ] Dokunma alanları yeterli büyüklükte, sürükleme işleminin alternatifi var.
- [ ] %200 yakınlaştırmada içerik kesilmiyor.
- [ ] Erişilebilirlik beyanı ve sorun bildirme yolu var.

## 18. Resmî kaynaklar

- W3C — Web İçeriği Erişilebilirlik Kılavuzu (WCAG) 2.2: https://www.w3.org/TR/WCAG22/
- W3C WAI — WCAG 2.2'de yenilikler: https://www.w3.org/WAI/standards-guidelines/wcag/new-in-22/
- W3C WAI — Erişilebilirliğe giriş: https://www.w3.org/WAI/fundamentals/accessibility-intro/
- Resmî Gazete — 2025/10 sayılı Cumhurbaşkanlığı Genelgesi (21.06.2025): https://www.resmigazete.gov.tr/eskiler/2025/06/20250621-17.pdf
- Aile ve Sosyal Hizmetler Bakanlığı — Genelge duyurusu: https://aile.gov.tr/eyhgm/haberler/web-siteleri-ve-mobil-uygulamalarin-erisilebilirligi-cumhurbaskanligi-genelgesi-yayimlandi/
- Avrupa Birliği — Avrupa Erişilebilirlik Yasası (Direktif 2019/882): https://eur-lex.europa.eu/eli/dir/2019/882/oj

---

## İlgili rehberler

- [KVKK için web geliştirici rehberi](https://github.com/alestaweb/kvkk-icin-web-gelistirici-rehberi)
- [E-ticaret hukuki uyum rehberi](https://github.com/alestaweb/eticaret-hukuki-uyum-rehberi)
- [Haber sitesi SEO rehberi](https://github.com/alestaweb/haber-sitesi-seo-rehberi)
- [Türkçe web yazılım rehberi](https://github.com/alestaweb/turkce-web-yazilim-rehberi)

## Katkı

Düzeltme ve eklemeler için issue açabilir, sorularınızı **Discussions** bölümünde sorabilirsiniz.

## Lisans

MIT

---

Hazırlayan: Alesta WEB — İzmir
