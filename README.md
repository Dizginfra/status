# N52 TV Durum

N52 TV hizmetlerinin anlık durumu: **https://status.n52tv.com**

- Denetimler GitHub Actions'ta 5 dakikada bir çalışır ([Upptime](https://upptime.js.org)). GitHub zamanlayıcısı sık işleri geciktirebildiği için `zincir.yml` denetimi her beş dakikada kendisi yeniden başlatır.
- Sayfa GitHub Pages'te yayımlanır, yani N52 TV sunucusundan bağımsızdır; sunucu çökse de açık kalır.
- Denetlenen adresler ve sayfanın metinleri `.upptimerc.yml` dosyasındadır.

## Olay duyurusu

Bir kesinti algılanınca bu depoda kendiliğinden bir issue açılır ve durum sayfasında "Süren olaylar" altında görünür. Hizmet düzelince issue kendiliğinden kapanır.

Elle duyuru yapmak için `status` etiketli yeni bir issue açın. Başlığa olayı, içeriğe ayrıntıları yazın. Etiket olarak etkilenen hizmetin adını ekleyin (ör. `haber-sitesi`). Güncellemeleri yorum olarak yazın; bittiğinde issue'yu kapatın.

## Planlı bakım

`maintenance` etiketli bir issue açın. İçeriğin başına başlangıç ve süreyi yazın:

```
<!--
start: 2026-11-01T02:00:00+03:00
end: 2026-11-01T03:00:00+03:00
expectedDown: haber-sitesi, yonetim-paneli
-->
Sunucu bakımı.
```
