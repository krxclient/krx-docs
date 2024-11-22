---
icon: stopwatch
---

# TAS (Tool-Assisted Speedrun) ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)

KRX Client Ultimate sürümündeki **TAS** sekmesi, hassas ve tekrarlanabilir girişler sağlayan gelişmiş araç destekli oyun için tasarlanmış bir beta özelliğidir. 
En sorunsuz TAS deneyimi için, bir sunucuya katıldıktan sonra `/showall` komutunu kullanmanızı öneririz. 
*Not: Bu özellik şu anda geliştirilme aşamasındadır ve işlevselliği gelecekte değişebilir.*
---

## **Ekran Görüntüsü**
![TAS Menu](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/tas-menu.png)

---
## **TAS**
- **Enable**: TAS'ı etkinleştirir ve sizi TAS dünyasına ışınlar. 
- **TPS (Ticks Per Second)**: Destekli girişler için tick oranını ayarlar (Teeworlds için varsayılan TPS: 50). 
- **Dummy Replay**: TAS modunda dummy desteğini etkinleştirir.
- **Player Prediction**: TAS dünyasına diğer oyuncuları ekler.
- **Ignore Start Warnings**: TAS'ın başındaki uyarı mesajlarını bastırır.
- **Stop Mouse When Paused**: Fare durduğunda TAS çalışmaz ve bu da legit çalıştırmalara izin verir.
- **Use Rewind Input**: Daha gerçekçi tekrarlar için fareyi geri sarılmış girişle eşleşecek şekilde ayarlar.  
- **Show Real Aim**: TAS yeniden oynatma sırasında gerçek aim yönünü görüntüler.
---

## Tools
- **Auto Rewind**: Donmadan önce otomatik olarak son güvenli işarete geri sarar.  
- **Auto Forward**: Dondurma işleminden önce otomatik olarak ilk tik işaretine ilerler.  
- **Rewind Ticks**: Geri sarılacak tick sayısını ayarlar (varsayılan: 1 tick).  
- **Forward Ticks**: İletilecek tick sayısını ayarlar (varsayılan: 1 tick).  
- **Pause**: Otomatik geri sarma veya otomatik iletme sonrasında TAS'ı duraklatır.  
- **Step**: Her bir tick için hassas hareket seçimi sağlayarak tam olarak bir tick geri veya ileri sarar.

---

## **Fake Aim**
- **Enable**: Sahte aim için sahte hedef modunu etkinleştirir.  
- **Mode**: Sahte hedef türünü seçer (örn. Robot Aim).

---

## **Auto Replay**
- **Enable**: Tekrarları otomatik olarak yükler ve yeniden başlatır.  
- **Reset on Freeze**: Donma gerçekleştiğinde yeniden oynatmayı yeniden başlatır.  
- **Kill on Reset**: Yeniden oynatma sona erdiğinde oyuncuyu öldürür.

---

## **God Mode**
- **Super**: TAS dünyasında RCON komutunu `super` olarak değiştirir.  
- **Weapon**: Kendinize bir silah vermenizi sağlar (bilinen sorunlar nedeniyle Ninja hariç).  
- **Give Weapon**: Seçilen silahı verir.

---

## **Hotkeys**
- **Enable TAS**: TAS'ı etkinleştirmek için bir tuş atar.  
- **Record Replay**: Yeniden oynatmayı kaydetmeye başlamak için bir tuş atar.  
- **Load Replay**: Bir yeniden oynatmayı yüklemek için bir tuş atar.  
- **Respawn TAS**: TAS modunda yeniden doğmak için bir tuş atar.  
- **Pause TAS**: TAS'ı duraklatmak için bir tuş atar.  
- **Rewind TAS**: TAS sırasında geri sarmak için bir tuş atar.  
- **Forward TAS**: TAS sırasında ilerletmek için bir tuş atar.

---

## **Additional Options**
- **Replays Folder**: TAS tekrarlarının depolandığı klasörü açar.  
- **Load/Save**: Tekrarları yükler veya kaydeder.  
- **Continue**: Seçilen bir yeniden oynatmanın son tikinden itibaren oynatmayı sürdürür.  
- **Custom Name Field**: Tekrarları özel bir adla kaydeder (örneğin, `my_tas`).  

---

## **SORU**
1. **S:** TAS'da neden silahları göremiyorum?
   **C:** `/showall` komutunu çalıştırmadınız.  

2. **S:** Bir harita değişikliğinden sonra koşuma neden devam edemiyorum?
   **C:** Maalesef harita değişikliklerinde devam etmek desteklenmiyor. Kaydı durdurun, farklı bir sunucuda haritaya katılın ve oradan devam edin.  

3. **S:** `Verify TAS Integrity failed...` gibi bu uyarılar nedir?
   **C:** Bu uyarılar TAS'ın sorunsuz çalışmasını sağlar. Genellikle bunları görmezden gelebilirsiniz, ancak hata ayıklama sorunlarına yardımcı olurlar - sorunlarla karşılaşırsanız lütfen bunları bizimle paylaşın.  

4. **S:** TAS'ım neden çalışmanın ortasında başarısız oldu?
   **C:** TAS hataları genellikle gecikme nedeniyle meydana gelir. Uygun `cl_prediction_margin` ayarını kullanın ve yeniden oynatmayı doğru başlangıç konumundan yeniden başlatın. Sorun devam ederse destek ekibiyle iletişime geçin.  

5. **S:** TAS'da neden hareket edemiyorum?
   **C:** Büyük olasılıkla TAS duraklatılmış veya `krx_tasrespawn` 1 olarak ayarlanmıştır. Bunu düzeltmek için TAS'ı duraklatın veya konsolda `krx_tasrespawn 0` komutunu çalıştırın.  

6. **S:** TAS'a girerken neden hiçbir şey görmüyorum?
   **C:** Yeniden doğmanız gerekiyor. Bunu çözmek için Yeniden Doğma kısayol tuşunu kullanın.  

7. **S:** Neden geri veya ileri saramıyorum?
   **C:** Geri veya ileri sarma özelliğini kullanmak için TAS'ta kayda başlamanız gerekir. Adım geri/ileri sarma etkinse, değişiklikler fark edilemeyecek kadar ince olabilir; gerekirse devre dışı bırakın.  