---
icon: fire
---

# Blatant ![Ultimate](https://img.shields.io/badge/Ultimate-%23f76d6d?style=flat-square)
KRX İstemcisindeki **Blatant** Gores botu, kolaydan ekstrem olana kadar her türlü Gores haritasıyla başa çıkmanıza yardımcı olmak için ustalıkla tasarlanmıştır.  
*Not: Botlardan kaçınırken, lütfen daha yüksek bir `cl_prediction_margin` kullanın [settings](../settings.md) bölümüne bakın ve ping'e göre tahmin marjını seçin*

---

## **Ekran Görüntüsü**
![Blatant Menu - Önerilen Ayarlar](https://raw.githubusercontent.com/Krixx1337/krxclient-docs/refs/heads/main/images/blatant-menu.png)

---

## **Avoid**
- **Enable**: Kaçınma işlevini etkinleştirir.
- **Player Prediction**: Diğer oyuncuların hareketlerini tahmin eder.
- **NSIF**: Önceki giriş dizilerini izleyen ve mevcut bariz giriş yeterince uzun süre devam etmediğinde NSIF'e geçen gelişmiş bir özellik.
- **Afk Protection**: Kullanıcı belirtilen **Afk Time** sonrasında AFK olarak algılandığında Gores botunu otomatik olarak devre dışı bırakır.
  - **Afk Time**: Saniye cinsinden yapılandırılabilir.

## **Settings**
- **Hook Assistance**: Gores botu için kanca girişlerini etkinleştirir.
- **Direction Assistance**: Gores botu için yön girişini etkinleştirir.
- **Check Ticks**: Açık taramaların ne kadar ileriyi tahmin ettiğini belirtir.
- **Kick in Ticks**: Blatant'ın etkinleştirilmemesi için mevcut girdinin minimum ömrünü belirler.
- **Action Ticks**: Kontrol tiklerine benzer ancak bariz taramalar sırasında bireysel eylemlere uygulanır.

## **Ratelimiting**
- **Enable**: Çeşitli eylemler için hız sınırlamayı etkinleştirir.
- **Hook/Unhook**: Kanca ve kanca açma eylemlerinin sıklığını sınırlar.
- **Direction/No Direction**: Yönle ilgili hız sınırlamayı kontrol eder.
- **Hook Check**: Yön sınırlamalarını yalnızca kanca takılmadığında uygular.
  - **Hook Ticks**: Kanca hız sınırlamasının süresini tik olarak ayarlar.
  - **Unhook Ticks**: Kanca açma hızı sınırlamasının süresini tik cinsinden tanımlar.
  - **Move Ticks**: Yönlü hareket için hız sınırlama süresini yapılandırır.
  - **Stand Ticks**: Sabit eylemler için hız sınırlama süresini ayarlar.

## **Misc**
- **Drag Support**: Aimbot'a ek veriler sağlayarak tee'nizin donmasına neden olabilecek yönlerden kaçınmanıza yardımcı olur.
- **Track Point**: Geçerli yönü izler ve kancalanabilirse, tüm tarama süresi boyunca hedefler.
- **Rehook Action**: Bariz taramada yeniden kancalama senaryolarını dikkate alır.
- **Safe Aim Tracking**: Yalnızca izlenen yön tüm tarama süresi boyunca geçerli kalırsa izlemeyi sağlar.
-**Tile Distance**: Kaçınılan karoların boyutunu ayarlar, bariz eylemlerin daha meşru görünmesini sağlamak için tasarlanmıştır.

## **Tiles**
- **Teles**: Işınlanma karolarından kaçınır.
- **Unfreeze**: Çözme karelerinden kaçınır.
  - **Ticks**: Çözülmemiş karolar için yapılandırılabilir kontrol süresi.
- **Death**: Ölüm karelerinden kaçınır.

## **Aimbot**
- **Enable**: Kaçınma aimbotunu etkinleştirir.
- **Auto Aim**: Tüm yönleri tarar ve en uzun uygulanabilir olanı seçer.
- **Aim Assist**: Farenize en yakın olan ve en uzun süre geçerli kalan yönü hedefler.
- **Upward Aim**: En uzun süre geçerli olan yukarı yönlere öncelik verir.
- **Points**: Segment başına değerlendirilecek nokta sayısını belirtir.
- **Segments**: Taranacak segment sayısını tanımlar.
- **FOV**: Hedefleme için yapılandırılabilir görüş alanı.
- **Check Ticks**: Aimbot hesaplamaları için taramaların süresini ayarlar.

## **Visuals**
- **Track Points**: İzlenen noktaları görsel olarak görüntüler.
- **Aimbot**: Aimbot hedef noktalarını vurgular.
- **Path**: Bot tarafından izlenen geçerli yolu gösterir.

## **Configuration**
- Bu botu yapılandırmak önemsiz değildir, bu ayarların her birini denemeniz gerekir, işte size başlamak için bazı temel yapılandırma:
- **NSIF**: AÇIK
- **Hook Assistance**: AÇIK
- **Direction Assistance**: AÇIK
- **Check Ticks**: 26
- **Kick on Ticks**: 20
- **Action Ticks**: 26
- **Drag Support**: AÇIK
- **Track Point**: AÇIK
- **Rehook Action**: AÇIK
- **Safe Aim Tracking**: Maksimum güvenlik için AÇIK, aksi takdirde KAPALI
