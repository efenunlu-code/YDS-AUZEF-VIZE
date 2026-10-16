# YDS Kelime Bankası + AUZEF Vize Çalışma (v6)

Bu proje, önceki YDS Kelime Bankası uygulamasının ayrı bir GitHub deposunda yayınlanabilecek geliştirilmiş sürümüdür. YDS kelime bankası, aralıklı tekrar, kelime çalışma oturumu ve YDS kelime denemesi korunmuştur.

## Yeni AUZEF bölümü
- Word dosyasından aktarılan 170 çoktan seçmeli soru
- 8 ders/soru seti
- Ders seçerek veya tüm derslerden karışık çalışma
- 10, 20, 40 ya da seçili dersin tüm soruları
- Doğru/yanlış geri bildirimi, sonuç yüzdesi ve yanlışların özeti
- AUZEF çalışma geçmişi ve cevaplanan sorular cihazın localStorage alanında tutulur
- İnternet/ücretli API gerektirmez; statik GitHub Pages olarak çalışır

## Dosyalar
- `index.html`: uygulama arayüzü ve işlevleri
- `words.js`: mevcut YDS kelime verisi (korunmuştur)
- `auzef.js`: Word belgesinden yapılandırılmış AUZEF soruları
- `AUZEF Konuları ve soru bankası.docx`: orijinal kaynak dosya
- `sw.js`: çevrimdışı/PWA önbelleği

## Yeni GitHub projesi olarak yayınlama
1. GitHub'da **New repository** seçip örneğin `yds-auzef-calisma` adını ver. Eski depoyu değiştirme.
2. Bu ZIP dosyasının içindeki klasörün dosyalarını (klasörün kendisini değil) yeni deponun ana dizinine yükle. `index.html` ana dizinde olmalı.
3. `Settings → Pages → Build and deployment` altında `Deploy from a branch`, branch `main`, folder `/(root)` seçip kaydet.
4. Pages bağlantısı oluşunca açıp YDS sekmelerini ve AUZEF Vize bölümünü test et.

## Not
AUZEF soruları sağlanan DOCX dosyasındaki soru ve cevap anahtarından aktarılmıştır. Kaynak belgede bulunabilecek cevap hataları otomatik olarak doğrulanmış değildir; özellikle sınav öncesinde ders materyalleriyle karşılaştır. Cihazdaki eski YDS ilerleme verisi, yeni uygulamada aynı tarayıcı ve aynı yerel depolama anahtarı kullanıldığı sürece korunur. AUZEF ilerlemesi ayrı anahtarda saklanır.
