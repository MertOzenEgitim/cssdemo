# 1-Giriş ve Temeller

## CSS nedir? Ne için kullanılır?
CSS (Cascading Style Sheets - Basamaklı Stil Şablonları), web sayfalarının görünümünü ve düzenini belirlemek için kullanılan bir stil dilidir.
CSS'in Kullanım Amaçları:
* HTML öğelerine stil kazandırır (renk, font, arka plan vb.).
* Sayfanın düzenini kontrol eder (konumlandırma, hizalama, boşluklar).
* Kullanıcı deneyimini artırır.
* Web sayfalarının tutarlı ve estetik görünmesini sağlar.
* Farklı cihazlar için uyumlu tasarımlar (responsive design) oluşturur.

## CSS Tarihçesi
CSS’in Gelişim Süreci:

* 1994: Håkon Wium Lie tarafından önerildi.
* 1996: W3C tarafından CSS1 standardı yayınlandı.
* 1998: CSS2 yayınlandı ve daha fazla stil seçeneği eklendi.
* 2000’ler: Tarayıcı uyumsuzlukları nedeniyle CSS’in kullanımında zorluklar yaşandı.
* 2011: CSS3 ile modüler yapı getirildi, animasyonlar ve yeni özellikler eklendi.
* Günümüz: CSS’in gelişimi devam etmekte olup, Grid, Flexbox gibi modern teknikler yaygın olarak kullanılmaktadır.

Öne Çıkan CSS Versiyonları:

* CSS1: Temel stil özellikleri (renk, font, arka plan vb.) içerir.
* CSS2: Sayfa düzenleri için gelişmiş özellikler eklenmiştir.
* CSS3: Modüler yapı, animasyonlar, medya sorguları gibi modern özellikler sunar.
* CSS4: Tam olarak bağımsız bir versiyon olarak değil, CSS3'ün geliştirilmiş sürümleri olarak ele alınmaktadır.

## CSS’in HTML ile entegrasyonu
CSS, HTML ile üç farklı şekilde entegre edilebilir:
1. Inline CSS (Satır İçi CSS)
HTML öğelerinin style özelliği içinde tanımlanır. Avantajı: Hızlı ve tekil değişiklikler için uygundur. Dezavantajı: Kodu karmaşık hale getirir, tekrar kullanım zordur.
2. Internal CSS (Dahili CSS)
HTML dosyasının `<head>` bölümünde `<style>` etiketi içinde tanımlanır. Avantajı: Belge içinde tüm HTML öğelerine stil verebilir. Dezavantajı: Sayfa boyutunu artırır, tekrar kullanım sınırlıdır.
3. External CSS (Harici CSS)
Ayrı bir .css dosyası içinde tanımlanır ve `<link>` etiketi ile HTML dosyasına bağlanır. Avantajı: Tek bir dosyada tüm siteye stil verebilir, kod tekrarını önler. Dezavantajı: Harici bir dosya olduğu için ek HTTP isteği gerektirir.

## CSS sözdizimi: Seçiciler, Özellikler ve Değerler
1. Seçiciler (Selectors)
CSS’in hangi HTML öğelerine stil uygulayacağını belirler. (Element (p), Id (#header-title), Class (.title))
2. Özellikler (Properties)
CSS’te öğelere uygulanabilecek stil kurallarını belirler. (color, font-size, margin, padding)
3. Değerler (Values)
Özelliklerin alabileceği durumlardır. (color:red; font-size: 18px; margin:10px; padding:20px;)

# 2-Ölçü Birimleri
## 2.1-Mutlak Ölçü Birimleri
Mutlak ölçü birimleri sabit değerlerdir ve ekrana veya ortama bağlı olarak değişmezler. Bunlar şunlardır;
* cm
* mm
* in
* pc
* pt
* px
## 2.2-Göreceli Ölçü Birimleri
Belirli bir referansa bağlı olarak değişkenlik gösteren ölçü birimleridir. Bunlar şunlardır;
* Metne göre;
* * em,
* * rem
* * ex
* * ch
* Kapsayıcıya göre;
* * vw
* * vh
* * vmin
* * vmax

# 3-Renkler
## 3.1-Renk Tanımlama Yöntemleri
* Renk İsimleri
* RGB (Red,Green,Blue)
* RGBA (Red,Green,Blue,Alpha)
* HEX
* HSL (Hue,Saturation,Lightness)
* HSLA (Hue,Saturation,Lightness,Alpha)
## 3.2-Renk Paletleri ve Araçlar
* W3Schools Color Names: https://www.w3schools.com/colors/colors_names.asp
* Color Hunt: https://colorhunt.co/
* Brand Colors: https://brandcolors.net/
* ColorZilla Chrome Extensions: https://chromewebstore.google.com/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp?hl=tr

# 4-CSS Box Model (Kutu Modeli)

![css-box-model](/readmeimage/css-box-model.png)

Varsayılan olarak, bir kutunun genişliği ve yüksekliği sadece içeriği kapsar, `padding` ve `border` bu 
genişliğe dahil edilmez. Ancak box-sizing: `border-box;` kullanarak `padding` ve `border`’ın genişlik ve 
yüksekliğe dahil edilmesini sağlayabiliriz.

* width: Kutunun genişliği belirler
* height: Kutunun yüksekliği belirler

* max-width: Kutunun maksimum genişliğini belirler.
* min-width: Kutunun minimum genişliğini belirler.

* max-height: Kutunun maksimum yüksekliğini belirler.
* min-height: Kutunun minimum yüksekliğini belirler.

# 5-CSS Selectors (Seçiciler)
* Element
* ID
* Class
* Specificity Kavramı
* !important
[Specificity Calculator](https://specificity.keegan.st/)

# 6-CSS Inheritance (Kalıtım)
* Kalıtılan Özellikler
* * color, font-family, line-height vs.
* Kalıtılmayan Özellikler
* * margin, padding, border, background vs.
* Inherit Kullanımı
* Global Değerler
* * initial, unset, revert
* Inheritance ve Specificity İlişkisi

# 7-CSS Combinator Selectors
* Descendant combinator (space)
* Child combinator (>)
* Next sibling combinator (+)
* Subsequent-sibling combinator (~)

